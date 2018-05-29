# lis180522

ちょまど氏登壇に使用した公開アプリのテスト

[[無料] Xamarin と Azure で、超効率的にクラウドと繋がるモバイルアプリを作ろう！[Azure Mobile Apps][MBaaS]@ちょ窓帳
](https://blogs.msdn.microsoft.com/chomado/xamarin/how-to-create-mobile-apps-connected-with-cloud/)

# memo

## build

初回ビルドは、<Proj>→<Proj>.XXXの順で。

lis180522を先にビルドしとかないと共通モジュールが生成されていない状態で、端末用プロジェクトをビルドすることになっていると思われる(エラる)。


