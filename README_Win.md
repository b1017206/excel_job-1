# excel_jobツールを使い始めるまで[Windows編]


## Python3をインストール
- 以下の辺りからダウンロードしてインストール
  https://www.python.org/downloads/windows/
- インストールが完了したら、コマンドプロンプトを起動して、以下のコマンド実行で想定したバージョンのPythonが使えるようになったか確認
  `python -V`
- うまくいっていない場合は PATH の設定を確認(PATHの中にPythonぽいのが入っているか)

## Pythonのパッケージをインストール
- コマンドプロンプトで以下のコマンドを実行し、インストール済みのパッケージを確認
  `pip list`
- 下記のパッケージがすべて揃うまで、`pip install パッケージ名` を続ける

  pandas
  xlrd
  openpyxl
  Pillow
  numpy
  matplotlib

## IPAフォントのインストール
- 以下の場所からIPAexフォントをダウンロードし、zipファイルを展開する
  https://ipafont.ipa.go.jp
- コントロールパネルからインストール済みフォント一覧を表示させ、展開した2つの.ttfファイルをフォント一覧にドラッグする(ドラッグ後に勝手にインストールされる)

## Excelデータの準備
- 未来大事務局の学生名簿Excelをstudentlistフォルダの中に置く
	- 置くファイルは一つだけ、ファイル名は何でもよい
- アンケート回答Excel(複数可)をanswersdataフォルダの中に置く
	- ファイル名はアンケート実施年月を含む 202004.xlsx などのようにする

## 実行
- コマンドプロンプトで以下のように実行
  `python output.py 学年 クラス`
  (学年は1か2、クラスはAからZのどれか一文字)
- 同じフォルダに output.xlsx が生成されるので、中身を確認

### テンプレの確認
- 各シートの元データは template.xlsx に入っています。説明文などの軽微な変更はここで
