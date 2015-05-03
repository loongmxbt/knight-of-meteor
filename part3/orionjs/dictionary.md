# The Dictionary

Instead of making all the content of your site static, use
__the dictionary__ to make all the content editable in the admin.

## Getting started

To use the dictionary you just have to define the *definition*
and then the administrator will be able to edit the value in admin panel.
It doesn't matter if it's an image, html, numbers, dates, or a simple
string, everything is just as easy.

### Creating Definitions

To create definitions you just have to set the name, the category
and the type.

```js
orion.dictionary.addDefinition(name, category, attributeSchema)
```

- ```name``` **String**. This is the name of the definition.

- ```category``` **String**. The category of the definition.
In the admin the form will be separated by categories.

- ```attributeSchema``` **Attribute**. Here is where you customize the
definition. Set it to String, Image, HTML, or anything!

Example:

```js
orion.dictionary.addDefinition('description', 'site', {
    type: String,
    label: "Description"
});
```

### Using the dictionary

Orion lets you get the value of the definitions easily in javascript or
directly in html.

#### In HTML

In the meteor templates, call the funcion dict. Where the first
attribute is the name of the definition and the second is the value that
will return if the definition is not set or its empty

```html
<template name="example">
  {{ dict 'site.description' 'No description' }}
</template>
```

#### In Javascript

Sometimes you might need to use the dictionary in template helpers
or other javascript files.

```js
var description = orion.dictionary.get('site.description', 'No description');
```
