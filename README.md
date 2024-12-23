# SandyLP Duo（サンディ エルピー デュオ）

![SandyLP Duo keyboard]()  

"SandyLP Duo" is a Split 40% keyboard with symmetrical row staggered layout and key height optimization.

Layered PCB will make height differences for each key.
This covers the lack of optimization to physical key layout in two dimensions that only adjust x-y plane.

---

SandyLP Duoは、スイッチの配置を立体的にして高さ方向への最適化を加えた、左右対称ロースタッガード配列の分割型40%キーボードです。  

平面上のキーレイアウトだけでは最適化しきれない部分を、キーの位置に応じてスイッチを配置する高さを変えることで補っています。

開発の元となった[SandyLP](https://github.com/jpskenn/SandyLP)の機能や特徴を踏襲しつつ、肩や腕を開いたより自然なポジションでの打鍵と、テンティングによる手首や腕の負荷軽減を目指しています。

SandyLPのコンセプトをそのまま引きついだバリエーションモデルとして、分割型の特徴である左右ふたつのペアを思わせる言葉の「Duo」を後ろにつけ、「SandyLP Duo」としました。  
元の元であるSandyから説明すると、スイッチを立体的（3D）に配置したキーボードの、ロープロファイル版、分割型バリエーションモデルということになります。

## 特徴

### 分割型

見てのとおり、右手用と左手用のふたつに分かれた、分割型キーボードです。
右手用または左手用のどちらかをPCやMacに接続し、もう一方へUSB Type-Cケーブルで接続します。

右手用と左手用を好みの場所に配置し、好みのポジションで打鍵できます。
前作の一体型キーボードSandyLP（中央部に2u分の間隔）に比べ、肩や腕を大きく開いたポジションをとることが可能で、肩や腕の負荷軽減が見込まれます。

また、ゴム足等を使ったテンティング（キーボードの内側を持ち上げて、親指側と小指側の高さを変える）をおこなうことで、手首や腕の負荷軽減が見込まれます。

### 左右対称のキーレイアウト  

[Jones](https://github.com/jpskenn/Jones)と同様の、2行目と3行目にずれのない、左右対称なシンメトリカル ロースタッガードのレイアウトです。  
![左右対称のキーレイアウト](./assets/Readme/DSCF5300.jpeg)

一般的なロースタッガードなレイアウトとの共通性を残しつつ、左右対称で打鍵しやすくなるよう、[SemiErgo Layout](https://github.com/mtei/SemiErgo_Layout)に準ずるキーマッピングで使用することを念頭に設計しています。  
Z行の左右端にシフトキーを用意していないので、スペースキーを「Space and Shift」として使うと便利です。

このレイアウトは、市販の各種キーキャップセットのうち「Base Kit」と呼ばれる基本的なキットですべてを埋めることができます。また、104キーの英語キーキャップセットでも十分実用が可能です。
〓Base Kitと104の検証
![左右対称のキーレイアウト](./assets/Readme/layout_for_base_kit.png)

詳しくは、[Keyboard Layout Editor: SandyLP Duo]()を参照してください。

### キースイッチを立体的に配置  

前機種の[Sandy](https://github.com/jpskenn/Sandy)と同じく、キースイッチを3段階の高さで立体的に配置しています。  
平面上ではキーを配置できる範囲が限られるため、一部のキーはどうしても指が届きにくくなってしまいます。例えば、[Jones](https://github.com/jpskenn/Jones)では左右対称のレイアウトを採用することで右手小指の`P`や`Back Space`、`Enter`などは打鍵しやすくなりましたが、右手人差し指の`Y`は少し遠く感じられました。  
このような箇所について、キーの配置を高くすることで打鍵しやすさを向上させています。  

![キースイッチの高さ（中央部分）](./assets/Readme/DSCF5294.jpeg)
![キースイッチの高さ（横から）](./assets/Readme/DSCF5296.jpeg)

キーの高さはLow（基準高＝0mm）, Middle（3.6mm）, High（8.7mm）の3段階で、以下のように配置されます。  
![キーの高さ](./assets/Readme/layout_height_map.png)

### キーボード自体が低い（薄い）  

ロープロファイルの`Choc V2`スイッチを採用することでキーボード自体が低くなりました。  
前機種のSandyからは7.2mm（※1）低くなり、パームレストを使わずとも、手首をあまり反らさないポジションで打鍵できます。

※1 ボトムプレートから1段目のスイッチ軸の天面までの高さを比較。なお、Sandyは理論上あと0.8mm低くすることが可能です。

![キースイッチの高さ](./assets/Readme/DSCF5284.jpeg)

### RP2040を採用した構成により、多機能なファームウェアを使用可能

RP2040を採用した構成により、キーボード向けのファームウェアを格納するには十分すぎるほどのフラッシュ容量を得ることができました。  
エンコーダーやオーディオ、その他各種機能の同時有効化や、多数のレイヤーを使用するなど、多機能なファームウェアを使用可能です。

### Remap、Vialによるキー割り当ての変更  

初期書き込み済みのファームウェアは[Remap](https://remap-keys.app/)に対応しており、プログラミング等の知識がなくても、キーマッピングやロータリーエンコーダへの割り当てを、ブラウザ等を使って簡単に変更できます。  

また、Vial対応のファームウェアに書き換えて使用することもできます。

### オプション機能  

- ロータリーエンコーダ
- インジケータLED
- オーディオ

## ビルドガイド


## SNSタグ

[#SandyLP_Duo](https://twitter.com/search?q=%23SandyLP_Duo)

## ギャラリー


## 参考事例


## 開発経緯
