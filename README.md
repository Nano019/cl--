# 左右反転画像　生成プログラム filp.py
----------------------------------------
# 1.概要
----------------------------------------
# 2.ソースコード
----------------------------------------
```python
#　このプログラムはpython3用です。
#　あらかじめ　pip install pillow でpillow をインストールしておきます。
from PIL import
import sys

#　コマンドライン引数から入力画像と出力画像ファイル名を取得
input_image = sya.argv[1]
output_image = sys.argv[2]

#　画像の読み込み
img = Image.open(input_image)

#　画像の左右反転
img_flip = img.transose(Image.FLIP_LEFT_RIGHT)

#　画像の保存
img_flip.save(output_image)
```
# 3.使い方
------------------------------------------
## 3.1実行例
* コマンドラインフォーマット
```python
python3 flip.py <input_image_path><output_image_path>
```
* 利用例
```python
python3 flip.py input.jpg output.jpg
```
## 3.2出力結果
* 以下のように入力画像の左右反転が出力されます。
|入力画像(input.jpg)|出力画像(output.jpg)|
|　|　|
