# Orion

Orion is an open source framework built on meteor that makes complex as well as simple apps possible with minimal effort. It’s built, modified, used, and supported by an active community of people around the world.

Orion 猎户星是一款基于Meteor打造的高级框架，它可以打造从简单到复杂的一系列APP。

### 开始

开始使用 Orion 你需要安装核心包和管理模板。Orion有两套默认的模板可供选择，分别是bootstrap和materialize。

```
meteor add orionjs:core
```
现在你可以自由选择使用哪套：
```
meteor add twbs:bootstrap
meteor add orionjs:bootstrap
```
```
materialize:materialize
meteor add orionjs:materialize
```
这里教程中我们选择bootstrap。

## 用户系统 Accounts

Orion allows for you to create accounts with different roles so that users can login and manage app content and configuration.

Orion 允许你创建不同角色的账户，从而用户可以登录和管理APP内容和设置。

### 创建账户 Creating accounts

Orion has 3 ways to create accounts:
Orion 有3种创建账户的方式：

Admin account. By default account creation is closed, but when there is no admin (no user that has the admin role), Orion will allow you to create an account that will be automatically granted an admin role.
管理员账户。默认情况下管理员创建是关闭的。

Invitations. The admin can invite users, you must navigate to the accounts tab and press +. This will generate a invitation link which you need to pass to the new user. If you set an email address on the invitation, the new user must have access to that email address.
邀请账户。管理员可以邀请用户。

Open Registration. With Open Registration, you can allow anyone to publicly register.
开放注册。

### 开放注册 Public registration

Enabling Public Registration
To allow anyone to register an account for your app, make sure to set the 'forbidClientAccountCreation' option to false.
```
Options.set('forbidClientAccountCreation', false);
```

### 默认角色 Default Roles
New users will not have any roles by default, unless you specify default roles:
新用户默认不会有任何角色，除非你设定了默认角色。
```
Options.set('defaultRoles', ['role1', 'role2']);
```