facebook login for XOOPS Cube V2.2

What this: Add Facebook Authentification to your XOOPS Cube site.
usage: Add smarty for your theme below.

[ja]
これは何：XOOPS Cube で構築したサイトに Facebook のログイン認証機能を付加します。
使い方：smarty 変数を貴方のテーマに以下を追加する事
[/ja]

```
<if $facbookLogin>
	<{$facbookLogin}>
<{/if}>
```