## User Accounts

User Accounts is a suite of packages for the Meteor.js platform. It provides highly customizable user accounts UI templates for many different front-end frameworks. At the moment it includes forms for sign in, sign up, forgot password, reset password, change password, enroll account, and link or remove of many 3rd party services.

User Accounts是一套为Meteor量身定制的用户系统扩展。它给不同的前端框架提供了可定制化的用户账户UI模板，包括Bootstrap3，Semantic UI等。它包含用户注册、登录、忘记密码、重置密码、修改密码、激活账户等功能，并且可以轻松的和第三方OAuth服务结合。

### 特色功能

* 完全可定制化
* 注重安全性
internationalization support thanks to accounts-t9n
* 基于accounts-t9n的国际化支持
custom sign-up fields
* 自定义注册字段
robust server side sign-up field validation
* 健壮的服务端注册字段验证
easy content protection
* 简单的内容保护
return to previous route after sign-in (even for random sign in choice and not only after required sign-in)
* 登录后回到之前的链接
fully reactive, Blaze fast!
* 完全的reactive，非常快速
no use of Session object
* 不使用 Session
very easily stylizable for different font-end frameworks
* 非常轻松的为不同前端框架定制
...wrap it up for famo.us with a simple meteor line!


### Available Versions

useraccounts:bootstrap styled for Twitter Bootstrap
useraccounts:foundation styled for Zurb Foundation
useraccounts:ionic styled for Ionic
useraccounts:materialize styled for Materialize
useraccounts:polymer styled for Polymer (WIP)
useraccounts:ratchet styled for Ratchet
useraccounts:semantic-ui styled for Semantic UI
useraccounts:unstyled with plain html and no CSS rules
plus others coming soon...


### 安装
```
meteor add useraccounts:bootstrap
```
下面至少选一个认证方式，当然需要集成第三方认证的话可以增加任意多个。
```
meteor add accounts-password
meteor add accounts-facebook
meteor add accounts-google
```


### 模板
值得注意的是，只需要一个模板用来展示所有功能，有点类似于单页面的用户管理中心。比如可以把功能类的都放在一个模板里，把注册登录单独拿出来。
sign in, sign up, forgot password, reset password, change password, and enroll account forms

```
{{> atForm}}
```

```
{{> atForm state='signUp'}}
```

### 国际化支持 TODO: have a problem
```
T9n.setLanguage('<lang>');
```