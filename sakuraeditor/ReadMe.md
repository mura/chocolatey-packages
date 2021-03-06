﻿# sakuraeditor
![サクラエディタ](icon.ico)
サクラエディタ

## About icon.ico
under zlib/libpng License
https://sourceforge.net/p/sakura-editor/code/HEAD/tree/sakura/trunk2/resource/icon_std.ico

See also : http://sakura.qp.land.to/?Develop%2FLicenses
##### 10 #####
A free Japanese text editor for Windows (Unicode Edition).

**Package Installer Version** 2.2.0.1

日本語の説明文が下にあります。(The Japanese explanation is below.)

# Features
* Syntax Highlight
* Outline analyze
* grep
* macro
* Japanese Support
etc...

## Params
You can choose which task do you want to use.

Example:

```
cinst -y sakuraeditor --params "'/Tasks:!quicklaunch,fileassoc'"
```

## tasks

* `startmenu`   : (default)
* `quicklaunch` : (default)
* `proglist`    : (default)
* `desktopicon` : 
* `fileassoc`   : add a 「SAKURAで開く」 context menu to explorer
* `startup`     : Resident at startup
* `sendto`      : 

See also (/TASKS)  
[Inno Setup Help](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline)



# 日本語利用者の方へ (For Japanese)
## サクラエディタについて
さくらエディタは日本語に対応した無料のテキストエディタです。詳細は以下のURLを参照してください。

* [サクラエディタ](http://sakura-editor.sourceforge.net/)
* [SakuraEditorWiki](http://sakura.qp.land.to/?FrontPage)

## このChocolateyパッケージについて
サクラエディタのパッケージインストーラ2.2.0.1をインストール後、sakura.exeを最新のものに上書きしています。  
正規表現ライブラリや強調表示ファイルは含まれています。

なお、このパッケージはサクラエディタプロジェクト公式のものでは無いので、要望や質問は@KageShironのTwitterかGitHubまでお寄せください。  
この関連ツールも同時インストールして欲しいといった需要がありそうなら極力対応します。

## インストール時の設定
インストーラで行う設定の一部が指定できます。--paramsに続けて以下のように指定します。"(ダブルクォート)の中に'(シングルクォート)が入ることに注意してください。

Quick Launchに追加せず、エクスプローラの右クリックに「SAKURAで開く」を追加する例:

```
cinst -y sakuraeditor --params "'/Tasks:!quicklaunch,fileassoc'"
```

`/Tasks:`に続けてカンマで区切って利用する機能を指定します。  
(デフォルト)となっている機能は勝手に適用されますが、`!startmenu`のように指定することで無効化できます。

* `startmenu`   : (デフォルト)スタートメニューを作成 
* `quicklaunch` : (デフォルト)Quick Launchにアイコン作成
* `proglist`    : (デフォルト)プログラム一覧に追加
* `desktopicon` : デスクトップにアイコン作成"
* `fileassoc`   : 「SAKURAで開く」メニューの追加"
* `startup`     : 起動時に常駐
* `sendto`      : 送るに追加

このオプションで指定した内容が以下のInno Setupの/TASKSに指定されます。  
[Inno Setup Help](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline)