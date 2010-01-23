はじめに
========

Sympal は PHP の MVC フレームワークの [Symfony](http://www.symfony-project.org/) をもとに作られた Content Management System です。

Symfony のプラグイン
-------------------

Sympal にはきわめて柔軟性とモジュラー性があります。このおかげで Sympal は Symfony の複数のプラグインで構成されます。次のセクションで Sympal のコアを構成するプラグインの手短なリストを見ることができます。

### Sympal のコアプラグイン

Sympal は少数の Sympal ベースのプラグインで構成されます:

 * sfSympalPlugin - Sympal のコア
 * sfSympalAdminPlugin - バックエンドのアドミン機能
 * sfSympalAssetsPlugin - アセット管理機能
 * sfSympalContentListPlugin - コンテントのリストを簡単に作成するための ContentList content-type
 * sfSympalDataGridPlugin - Doctrine で動くデータグリッドリスト作成用の OO ライブラリ
 * sfSympalFrontendEditorPlugin - フロントエンドインラインエディター機能
 * sfSympalInstallPlugin - Web と CLI インストール機能
 * sfSympalMenuPlugin - Sympal メニュー機能
 * sfSympalPagesPlugin - Default Page content-type
 * sfSympalPluginManagerPlugin - Sympal Plugin Web と CLI のインストール管理機能
 * sfSympalRenderingPlugin - フロントエンドのコンテントのレンダリング
 * sfSympalUpgradePlugin - Sympal アップグレード管理
 * sfSympalUserPlugin - sfDoctrineGuardPlugin と関連の追加機能

### Core Addon Plugins

Sympal コアプラグインに加えてわたしたちはいくつかの便利な Symfony プラグインも組み込んでいます:

 * sfDoctrineGuardPlugin - ユーザー管理
 * sfJqueryReloadedPlugin - jQuery ヘルパーなど
 * sfFeed2Plugin - フィード解析と生成
 * sfWebBrowserPlugin - sfFeed2Plugin に必要
 * sfFormExtraPlugin - 追加のフォームに役立つもの、ウィジェット、バリデーターなど
 * sfTaskExtraPlugin - Symfony の便利な追加タスク

>Note
>上述のプラグインは通常の Symfony プラグインですが Sympal に同梱されます。これらが提供する機能はとても便利で一般的に Sympal に取り組むときは Symfony に取り組むことになるからです。後でこれらが提供する機能を細かく検討します。

これらのプラグインはコンテントマネジメントシステムの基本機能だけでなく拡張可能なインフラストラクチャも一緒に実装するので開発者は独自の Content-Type と Sympal プラグインを簡単に追加できます。これらは後で検討する実装済みのフックとイベント を利用することで Sympal のほかのプラグインと簡単にやりとりおよび操作することもできます。

機能
----

**複数のサイト**

1 つの Sympal プロジェクトの中で複数のサイトを簡単に管理します。

**ページキャッシング**

Sympal のページキャッシングのオンとオフを簡単に切り替えます。レイアウトの有無を指定してページを簡単にキャッシュできます。

**セキュリティ**

ユーザー、グループとパーミッションシステムで誰がコンテントを編集／閲覧できるのかを制御できます。

**国際化**

任意のコンテントの国際化機能を有効にできます。データベースのプロパティはコンフィギュレーションの値を変更するだけで国際化できます。

**サイトメニュー**

すばらしい Web インターフェイスからサイトメニューを管理してほんの少しの作業でサイトのレイアウトの中でこれらを簡単にレンダリングできます。

**パンくずの生成**

サイトマップの現在の位置からもしくは入力値の配列から手動でパンくずを簡単に生成します。

**カスタム content-type**

独自の content-type を追加することで Sympal のコンテントを拡張する (すなわち BlogPost、Article など)

**カスタムスロットタイプ**

より多くのコンテントはユーザーの入力を収める"スロット"を複数定義することができます。コンテンツを編集しレンダリングする方法をカスタマイズすることを可能にする独自のタイプを追加できます。

**CLI & Web ベースのインストーラー**

コマンドラインもしくは Web ベースのインストーラーから Sympal を簡単にインストールする。

**CLI & Web ベースのプラグインのインストーラー**

Web ベースもしくはコマンドラインインストーラーから利用可能な Sympal プラグインを見てインストールできます。

**テンプレート**

Sympal の複数のレベルでコンテントをレンダリングするのに使われるテンプレートのコンフィギュレーションの変更およびオーバーライドが可能です。このおかげで異なるテンプレートで特定のコンテントをレンダリングすることが可能です。

**レイアウト**

テンプレートと同じことがレイアウトにも当てはまります。複数のレベルで使うレイアウトをカスタマイズできます。たとえばグロバールレイアウト、サイトレイアウト、content-type のレイアウトをセットする、もしくは個別のコンテントの記録のレイアウトをカスタマイズすることさえもできます。
