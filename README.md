# DjangoTutorial

[公式チュートリアル](https://docs.djangoproject.com/ja/3.2/intro/tutorial01/)の投票アプリケーション

## 環境

VScode Remote Container推奨

## タスクランナー

VScodeのExplorerViewにあるTASK RUNNERからDjangoの管理コマンドを実行可能

- `makemigrations`
    - `python manage.py makemigrations`を実行
    - 入力ダイアログで新規追加or更新するモデルを指定(空白で全ての追加済みモデルを更新)
- `migrate`
    - `python manage.py migrate`を実行
- `runserver`
    - `python manage.py runserver`を実行
- `test`
    - `python manage.py test`を実行
    - 入力ダイアログで対象のテストを指定(空白で全てのテストを実行)

## git cloneからブラウザ表示まで

1. Remote Cntainerで開く
1. TASK RUNNERのrunserver実行
1. ローカルのブラウザで`localhost:<port>/polls/`にアクセス
     - ローカルの8000番が未使用であれば8000:8000でポートフォワーディング
     - 使用中の場合VSCode側で自動的に空きポートに割り当て
     - そもそもOpen in Browserのダイアログが出るはず(この場合アクセス先はトップページ(未作成)なので注意)

## データベース管理
- ログインページ：`/admin/`
- ユーザー名：`admin`
- パスワード：`password`
