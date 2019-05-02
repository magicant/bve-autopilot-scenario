# bve-autopilot-scenario

[![クリエイティブ・コモンズ・ライセンス](https://i.creativecommons.org/l/by/4.0/80x15.png)](http://creativecommons.org/licenses/by/4.0/)

これは [bve-autopilot プラグイン](https://github.com/magicant/bve-autopilot)のテスト用の簡易シナリオです。

このシナリオデータでは [Nagoya_Common 共通ストラクチャパック](https://kumoha12.web.fc2.com/Common.html)を参照しています。Nagoya_Common のファイル群を同じ Scenarios フォルダーに入れてから起動してください。

## クリアカー

シナリオには「クリアカー」という名前の架空車両が含まれています。

 - 起動加速度: 3.0 km/h/s
 - 常用ブレーキ減速度: 4.0 km/h/s
 - 非常ブレーキ減速度: 4.5 km/h/s

試験用車両のため通常の車両とは異なる性能の特性を持ちます。音源素材は含まれていません。

## 試験路線

以下の試験用路線のデータが含まれています。

 1. 基本試験
 2. 制限速度試験
 3. 上り勾配試験
 4. 下り勾配試験
 5. ATS-P 試験

運転方法は[プラグインの Readme](https://github.com/magicant/bve-autopilot) を見てください。

## 他の路線

参考用として、クリアカーを京成千葉線で走らせるためのシナリオファイルが含まれています。京成千葉線データを同じ Scenarios フォルダーに入れてから起動してください。

## ライセンスとクレジット

このシナリオデータは [magicant](https://github.com/magicant) が作成しました。

このレポジトリーに含まれるファイルは[クリエイティブ・コモンズ 表示 4.0 国際 ライセンス](https://creativecommons.org/licenses/by/4.0/)の元で自由に使用できます。ただし、以下のファイルを除きます。

 - bve-autopilot.dll プラグイン本体
   - このファイルのライセンスは [LGPL 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) です。

またシナリオで参照されている Nagoya_Common 共通ストラクチャパック内のファイルや京成千葉線のファイルはこのレポジトリーに含まれるファイルではないためクリエイティブ・コモンズの対象ではありません。
