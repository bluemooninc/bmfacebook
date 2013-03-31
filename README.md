bmfacebook
==========

facebook login for XOOPS Cube V2.2

What this: Add Facebook Authentification to your XOOPS Cube site.
usage: Add smarty for your theme below.

[ja]
これは何：XOOPS Cube で構築したサイトに Facebook のログイン認証機能を付加します。
使い方：smarty 変数を貴方のテーマに以下を追加する事
[/ja]

1:Get App ID and Secret code
----------------------------

login to https://developers.facebook.com/
Display Name : your service name. ( ex:XoopsEC )
Namespace : your service name space. ( ex:xoopsec )
App Domains : your domain ( ex:xoopsec.com )
Sandbox Mode : "DISABLE" ( if set enable, it works ONLY your account )
Login site url : site url for facebook login ( ex:https://www.xoopsec.com/modules/bmfacebook/ )

2:Install bmfacebook module on your site
----------------------------------------

!!! Module update after install !!!
Update program will make a user_facebook field on user table.

3:set AppID/Secret on module admin panel
----------------------------------------
   [image]: http://dl.dropbox.com/u/31666676/github/facebookAppId.gif "Admin panel"

4:add <{$facbookLogin}> to your theme html
------------------------------------------

```
<if $facbookLogin>
<{$facbookLogin}>
<{/if}>
```

Example theme
https://github.com/bluemooninc/xoopstrap
