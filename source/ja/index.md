<!--toc=about-->

# 開発者マニュアルについて

[[PRODUCTNAME]]プラットフォームは、開発者やデザイナーがデジタルサイネージのクリエイティブなプロセスに関与するためのさまざまな機会を提供します。この開発者向けドキュメントは、プラットフォームの技術的な要素を含むすべての部分についてのガイダンスを提供することを目的としています。

> このドキュメントは、技術的な読者に向けて書かれています。[ユーザーマニュアル](/manual/ja/index.html)や[管理者マニュアル](/admin-manual/ja/index.html)をお探しの場合は、提供されているリンクをご利用ください。

これらの文書は、より一般的な活動を最初に説明するような順序になっていますが、どの部分が必要かは、あなたが何を達成したいかによって決まります。

| **セクション** | ** 説明** | ** 例** |
|:-----------|:-----------|:------------|
|ウィジェット |レイアウトデザイナーを使用して、埋め込み型またはパッケージ型の HTML ウィジェットを作成する方法、または独自のモジュールを作成する方法を説明します。 |レイアウトで使用するための新しいビジュアライゼーションを作成します。サードパーティからデータを取得することもできます。 |
|プレイヤー制御 |ウィジェットで利用できるプレイヤーの情報、継続時間の制御方法、Webhook の送受信方法など、プレイヤー側でできることを発見してください。 |光センサーによるコンテンツのトリガーなど、プレイヤーでのインタラクションを実現します。 |
|テーマ |CMS のルック＆フィールを変更します。 |色を変更したり、ロゴを追加したりして、CMS の外観を変更します。|
|連携 |Xibo APIを呼び出して、サードパーティシステムと連携できます。 oAuthによる認証方法と、利用可能なAPIコールについてはこちらをご覧ください。|サードパーティは、CMSにコンテンツをプッシュします。Canva アプリはこの良い例です。 |
|拡張 |CMSに機能を追加して拡張します。CMS のアーキテクチャと、ミドルウェアを使用して独自の PHP コードを組み込む方法について学びます。	サードパーティからコンテンツを取得したり、CMS を変更してダッシュボードに別の方法でデータを表示したりします。 |サードパーティが呼び出す専用の API ルートを作成します。 |
|プレイヤーを作成する |非常に特殊なユースケースやニッチなハードウェア要件がある場合、またはオープン ソース プレイヤーの 1 つに貢献したい場合に便利です。 |プレイヤーがCMSとどのように通信し、コンテンツをどのようにレンダリングするかを学びます。|

## DOOHに関するメモ

XiboをDOOHプラットフォームとうまく統合し、スケジュール、表示、プレイ証明のすべてを適切に処理することは、複雑な要件が必要です。そこでXiboは、SSPとDSPを兼ねたDOOHプラットフォーム「Adspace」を提供することにしました。AdspaceはXibo CMSやXiboプレイヤー（現在Android/Windows、順次対応予定）と緊密に連携しています。

CMSの代わりにAdspaceと直接統合することで、より簡単に、より強力になる可能性があります。詳しくは、[xibo-adspace.com](https://xibo-adspace.com/)をご覧ください。

## オープンソースに関する注意事項

私たちは弁護士でもなければ、ソフトウェア法の専門家でもありません。疑問がある場合は、必ず専門家に相談してください。

[[PRODUCTNAME]]はオープンソースであり、それはある種の活動に対して何らかの影響を及ぼします。一般論として、ユーザーインターフェースからCMSにコードを入力する場合、パッケージHTMLとしてアップロードする場合、Webhookを送信する場合、API経由で接続する場合は、「arms length」であり、コードのライセンスを希望通りに取得できます。テーマやカスタムモジュールを開発したり、Xiboを拡張する場合、あなたのコードはAGPLv3に該当します。

## 貢献に関する注意

もし、あなたが何かクールなことをしていて、それをコアソフトウェアに取り入れるべきだと思うのであれば、私たちはいつでも手を差し伸べ、耳を傾けることができます。[コントリビューション](contributing.html)に関するガイドラインがありますので、始める前に参照してください。