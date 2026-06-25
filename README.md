<img width="640" height="468" alt="output" src="https://github.com/user-attachments/assets/ac91efda-7f87-4ef1-b100-bad2198ae441" />
<img width="640" height="468" alt="input" src="https://github.com/user-attachments/assets/84b77690-a6df-40f6-8f47-d2a2aafc7b27" />
<img width="640" height="468" alt="input" src="https://github.com/user-attachments/assets/b6d5a34e-386e-48e6-bbe0-cd80cc27262d" />
<img width="640" height="468" alt="output" src="https://github.com/user-attachments/assets/673c82ff-8011-4ca3-bb8e-f010d2f481f8" />
<img width="640" height="468" alt="input" src="https://github.com/user-attachments/assets/81c9b91f-37a8-430d-8e0a-f72e2cad6600" />
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
|---|---|
|input.jpg|output.jpg|
