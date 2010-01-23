クイックスタートガイド
=====================

Sympal 1.0 クィックスタートガイドにようこそ！このドキュメントはほんの数分で新しい Sympal プロジェクトを稼働させるための手助けをします！

最初に行う必要のあることは中で作業するディレクトリです。ここは Symfony 1.4 をチェックアウトして Sympal インストーラースクリプトでプロジェクトを生成する場所です。

    $ mkdir sympal

では次のステップで使うことになるいくつかのほかのディレクトリを作る必要があります:

    $ cd sympal
    $ mkdir lib
    $ mkdir lib/vendor

`lib/vendor` ディレクトリの内部で symfony 1.4 の最新バージョンをチェックアウトします:

    $ svn co http://svn.symfony-project.org/branches/1.4 lib/vendor/symfony

Sympal 用の Symfony インストーラーをさっと手に入れましょう:

    $ curl http://svn.symfony-project.org/plugins/sfSympalPlugin/trunk/data/bin/installer.php > installer.php

はい、すべての必要なものが手に入りました！ Sympal をインストールしましょう！次のコマンドによって最初のユーザー、データベースクレデンシャルなどをセットアップする対話方式のインストール作業プロセスが始まります。

インストーラースクリプトは新しいプロジェクトを生成し、 Sympal を稼働させることができるのか伝えるためにサーバー環境のチェックを実行します！

![サーバーチェック](http://github.com/masakielastic/sympal-ja/raw/master/images/picture-16.png "サーバーチェック")

チェックが完了した後でこのコマンドは結果を報告し Sympal のインストール作業を続けるのかどうかをあなたに聞きます:

![インストール作業を続ける](http://github.com/masakielastic/sympal-ja/raw/master/images/picture-17.png "インストール作業を続ける")

インストール作業を続ける場合インストール作業を完了させるために情報を入力するようあなたに促します:

![サーバーチェックの結果](http://github.com/masakielastic/sympal-ja/raw/master/images/picture-18.png "サーバーチェックの結果")

これでインストール作業が終わり、 Sympal で遊び始めることができます！遊ぶデフォルトのサイトが表示されます:

![デフォルトのサイト](http://github.com/masakielastic/sympal-ja/raw/master/images/picture-18.png "デフォルトのサイト")
