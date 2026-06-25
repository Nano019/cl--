# 左右反転画像　生成プログラム filp.py
----------------------------------------
# 1.概要
----------------------------------------
# 2.ソースコード
----------------------------------------
```python
#　このプログラムはpython3用です。
#　あらかじめ　pip install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

#　コマンドライン引数から入力画像と出力画像ファイル名を取得
input_image = sys.argv[1]
output_image = sys.argv[2]

#　画像の読み込み
img = Image.open(input_image)

#　画像の左右反転
img_flip = img.transpose(Image.FLIP_LEFT_RIGHT)

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
  |---|---|
  |<img width="640" height="468" alt="input" src="https://github.com/user-attachments/assets/2491b1fe-6976-451c-9db6-a5780a461ad9" />|<img width="640" height="468" alt="output_image" src="https://github.com/user-attachments/assets/6bbad64b-2a28-4e7c-b5e2-6a0fbd00de09" />
|

以上
