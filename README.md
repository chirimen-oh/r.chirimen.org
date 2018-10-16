# r.chirimen.org
リダイレクト用ドメイン r.chirimen.org

このサイトは netlify でホストすることで、簡単なテキストファイルの編集だけでリダイレクト専用 URL を一括して作成、管理、ホスト出来るようにしています。

`public/_recirects` ファイルに r.chirimen.org 配下の URL にアクセスしたときのリダイレクト先 URL を定義してください。変更を master ブランチに push すれば即時本番サイトに反映されます。書式の仕様は [Netlify のリダイレクト解説ページ](<https://www.netlify.com/docs/redirects/>) をご覧ください。設定のテストは [Netlify's Playground ページ](https://play.netlify.com/redirects) で確認できます。

Netlify のサイト側ではこの github リポジトリと連携させ、public ディレクトリを Publish directory に指定すること、DNS サーバで r.chirimen.org を netlify に向ける以外の設定は一切していません。

上記の通り、リダイレクトの定義を変更・更新する上では github 側のファイルを変更するだけで済むので netlify 側の管理は一切不要です。サービスが終了しないことだけを祈りつつ、終了したら適当に他のサービスなり自前システムなりに乗り換えましょう。
