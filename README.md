Photo Batch Editor (MVP)
iPhone Safari向けの静的Webアプリです。複数画像を選択し、露出と明るさを共通設定で調整してJPEGに書き出します。
GitHub Pagesで公開する
1. GitHubで新しいリポジトリを作成します（例: photo-batch-editor）。
2. index.html をリポジトリの一番上（root）にアップロードします。
3. リポジトリの Settings → Pages を開きます。
4. Deploy from a branch を選び、Branchを main、Folderを /(root) にして保存します。
5. 数分後に表示される https://<ユーザー名>.github.io/photo-batch-editor/ をiPhoneのSafariで開きます。
操作
- 「写真を追加」で写真ライブラリから複数枚を選択します。
- サムネイルをタップすると、その写真を一括処理の対象から外したり戻したりできます。
- 露出・明るさを調整し、「選択した写真を一括加工して保存」を押します。
- iPhoneでファイル共有に対応している場合は共有シートが開きます。そこから「画像を保存」などを選びます。
現在の制限
- Apple純正「写真」アプリの非公開アルゴリズムを再現したものではありません。露出は線形sRGBでのEVゲイン、明るさはsRGB値への加算による近似です。
- 書き出しは新しいJPEGです。元画像は変更しません。
- Canvas書き出しでは通常、元のEXIFメタデータやLive Photos情報は維持されません。
- HEIC/HEIFはSafari側で画像としてデコードできる場合のみ読み込めます。
- 大きな写真を大量に選択するとiPhoneのメモリ制限に達する場合があります。
- 一括処理はブラウザ内で行い、画像をサーバーへ送信しません。
