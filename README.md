# 自作マーカーで歩くキツネを表示する

## 使い方

1. ZIPを展開します。
2. GitHubのリポジトリの一番上に index.html、Fox.glb、fox.patt、README.md、Fox_LICENSE.txt を置きます。
3. GitHub Pagesを有効にし、スマートフォンで公開URLを開きます。
4. marker.pngを印刷するか、別の画面に表示し、スマートフォンのカメラを向けます。

index.htmlの animation-mixer="clip: Walk; loop: repeat" が歩く動きを再生します。WalkをRunに変えると走る動きになります。

## ファイル

- index.html: AR表示のページ
- Fox.glb: アニメーションを含むキツネの3Dモデル
- fox.patt: 自作マーカーの認識用データ
- source.png: マーカーを作る元のキツネのイラスト
- marker.png: カメラに見せる完成マーカー
- model.png: GLBモデル単体の表示画像
- ar.png: 自作マーカーにGLBを重ねた表示画像
- ar_walk.gif: AR表示中の歩行アニメーション
- viewer.html: GLBモデル単体を見るページ
- Fox_LICENSE.txt: モデル配布元の説明と利用条件

## モデルの出典と利用条件

Fox from Khronos glTF Sample Assets
https://github.com/KhronosGroup/glTF-Sample-Assets/tree/main/Models/Fox

- Model: PixelMannen, 2014, CC0 1.0 Universal
  https://creativecommons.org/publicdomain/zero/1.0/
- Rigging and Animation: tomkranis, 2014, CC BY 4.0
- Conversion to glTF: AsoboStudio and scurest, 2017, CC BY 4.0
  https://creativecommons.org/licenses/by/4.0/

Fox.glbは原データのまま収録しています。HTML内で表示倍率、向き、再生するクリップを指定しています。
公開時にもこの出典と利用条件を残してください。

元のマーカー用イラストは、この実習用に生成したものです。
背景は実習用に生成した机の画像を疑似カメラ映像に使用しています。

## 使用ライブラリ

- A-Frame 1.5.0: https://aframe.io/
- AR.js 3.4.7: https://ar-js-org.github.io/AR.js-Docs/
- A-Frame Extras 7.7.0: https://c-frame.github.io/aframe-extras/

AR.jsの公式マーカー生成処理を使用して、source.pngからfox.pattとmarker.pngを作成しています。

