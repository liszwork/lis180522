# lis180522

ちょまど氏登壇の、手順紹介アプリのテスト＋拡張・改造

参考：[[無料] Xamarin と Azure で、超効率的にクラウドと繋がるモバイルアプリを作ろう！[Azure Mobile Apps][MBaaS]@ちょ窓帳
](https://blogs.msdn.microsoft.com/chomado/xamarin/how-to-create-mobile-apps-connected-with-cloud/)

## TODO

- [ ] DLLでPushしていないモノを確認→あればPush
- [x] Gitのせるファイルの精査

ref. http://ytabuchi.hatenablog.com/entry/2017/11/15/123000

## memo

### 同期動作について

能動的な同期

- スマホ：一覧のプルダウン
- Windows：同期ボタン押下

イベントトリガ

- NW状態の変更(接続復帰)

> コンテキストによって追跡された保留中のローカル更新のあるテーブルに対してプルが実行される場合、そのプル操作は前のコンテキストのプッシュを自動的にトリガーします。 このサンプルの項目を更新、追加、完了するとき、明示的な PushAsync の呼び出しを省略できます。<br>
ref. https://docs.microsoft.com/ja-jp/azure/app-service-mobile/app-service-mobile-xamarin-forms-get-started-offline-data#review-the-client-sync-code オフライン同期に関する考慮事項

プル時に未同期の項目を「同期+プッシュ」する必要があるってことかな？<br>
「自動的にトリガーします」ということは、実行時にこの2つを勝手にやってくれるってことかな？
