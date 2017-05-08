# UIImageView

## 概要
UIImageViewは画像を表示するクラスです。

## 関連クラス
UIView
UIImage
　
## 実装手順
1. StoryboardにUIViewとそのsubViewとしてUIImageViewを配置します。
2. UIViewControllerとStoryboardのUIView・UIImageViewを関連付けます。
3. png画像をAssets.xcassetsに追加します。
4. StoryboardでUIImageViewに画像をセットします。

## 主要メソッド

|メソッド名|説明|サンプル|
|---|---|---|
|draw(in:) | 指定した範囲内に画像全体を描画する <br> 必要に応じてサイズを変更しフィットさせる | image.draw(in: CGRect(x: 0, y: 0, width: 80, height: 80)) |
| startAnimating() | アニメーションを開始する | imageView.startAnimating() |
| stopAnimating() | アニメーションを停止する<br>animationRepeatCountの設定をしている場合、当メソッドを呼ばなくても止まる | imageView.stopAnimating() |

## 主要プロパティ

|メソッド名|説明|サンプル|
|---|---|---|
| animationImages | アニメーションに使用するUIImageオブジェクトの配列を設定する | UIImageView.animationImages =<br> [UIImage(named: "image1")!, UIImage(named: "image2")! ] |
| animationDuration | アニメーションの再生間隔を設定する(秒単位) | ImageView.animationDuration = 0.5 |
| animationRepeatCount | アニメーションの再生回数を設定する | ImageView.animationRepeatCount = 5 |

## フレームワーク
UIKit.framework

## サポートOSバージョン
iOS2.0以上

## 開発環境
|category | Version|
|---|---|
| Swift | 3.0.2 |
| XCode | 8.2.1 |
| iOS | 10.0〜 |

## 参考
https://developer.apple.com/reference/uikit/uiimageview
