# SoundDropUNIT

<img src="https://github.com/akita11/SoundDropUNIT/blob/main/SoundDropUNIT.jpg" width="240px">



音声再生IC JQ8400を使用した音声再生モジュールです。4MBのフラッシュメモリを搭載しており、PCにmicroUSBケーブルで接続するとUSBメモリとして認識され、そこにMP3音声データ等をコピーします。その音声データをGrove端子のシリアル(UART)通信で再生制御できます。（UIFlow(v1)用のブロックも用意する予定）

※JQ8400に関する情報はWebページ等で検索してください。例えば[aitendoのモジュール](https://www.aitendo.com/product/15641)があります。

## 使い方

<img src="https://github.com/akita11/SoundDropUNIT/blob/main/SoundDropUNIT_terminal.jpg" width="240px">

以下のようにスピーカやアンプを接続し、Grove端子からの制御で音声を再生します。


### アンプ付きスピーカに接続する場合

3.5mmジャック（ステレオ：上部中央）に3.5mmステレオケーブル等でアンプに接続します。


### スピーカを直接接続する場合

基板上部にある1.25mmピッチコネクタ(Molex 53047-0210用)をとりつける端子があり、市販の小型スピーカ（M5Stack本体に使われているものなど。AliExpressやTaobaoでも同等品があります）を接続することができます。


### 3.5mmジャックに直接スピーカを接続する方法

3.5mmジャックに直接スピーカを接続することもできます。その場合は、基板裏面のハンダジャンパを以下のように修正してください。（スピーカはモノラル再生となります）

<img src="https://github.com/akita11/SoundDropUNIT/blob/main/SoundDropUNIT_back.jpg" width="240px">

- JP1をカット
- JP2・JP3の中央と△マーク側をカットし、中央と反対側（△マークがない側）をショート


## Author

Junichi Akita (@akita11) / akita@ifdl.jp
