# bve-autopilot-scenario

[![クリエイティブ・コモンズ・ライセンス](https://i.creativecommons.org/l/by/4.0/80x15.png)](http://creativecommons.org/licenses/by/4.0/)

これは [bve-autopilot プラグイン](https://github.com/magicant/bve-autopilot)のテスト用の簡易シナリオです。

## 必要なもの

このシナリオデータは BVE 5.8 & 6 用です。

このシナリオデータでは [Nagoya_Common 共通ストラクチャパック](https://kumoha12.web.fc2.com/Common.html)を参照しています。Nagoya_Common のファイル群を同じ Scenarios フォルダーに入れてから起動してください。

自動運転プラグインが起動しない ("Cannot load" というエラーメッセージが表示される) 場合は [Visual C++ 再頒布可能ランタイムライブラリー](https://support.microsoft.com/ja-jp/help/2977003/the-latest-supported-visual-c-downloads) (vc_redist.x86.exe, vc_redist.x64.exe) をダウンロードしてインストールしてください。

## クリアカー

シナリオには「クリアカー」という名前の架空車両が含まれています。

 - 起動加速度: 3.5 km/h/s
 - 常用ブレーキ減速度: 4.0 km/h/s (80 → 0 km/h の平均, 乗車率 100% 時)
 - 非常ブレーキ減速度: 4.5 km/h/s (同)

試験用車両のため通常の車両とは異なる性能の特性を持ちます。

### 自動運転の操作方法

車両のドアが閉まったら、マスコンレバーを N にしてから保安装置 15 (L) のキー (BVE5 のデフォルト設定では、テンキーでない方の `0`) を押すと自動運転が始まります。

シナリオ開始時は ATO が有効になっていますが、レバーサー切かつ非常ブレーキの状態で保安装置 15 (L) のキーを押すと「ATO 有効」「TASC のみ有効」「どちらも無効」の順に状態が切り替わります。

## 試験路線

以下の試験用路線のデータが含まれています。

 1. 基本試験
    * 1a. 応荷重制御試験
    * 1b. 減速度変更試験
    * 1c. 到達時刻試験
 2. 制限速度試験
    * 2a. 超過試験
 3. 上り勾配試験
 4. 下り勾配試験
 5. 信号試験
    * 5a. ATC 試験
    * 5b. swp2 試験
    * 5c. 自動発進試験 (ATC)
    * 5d. 出発時刻設定試験
    * 5e. 自動発進試験 (非 ATC)
    * 5f. D-ATS-P 試験
    * 5g. ATC 試験 (小田急プラグイン用)
    * 5h. ATC 試験 (メトロ TASC プラグイン用)
 6. ORP 試験
 7. 停止位置修正試験

試験用路線のシナリオは自動運転の準備が整っているので、シナリオを開けばすぐに自動運転が試せます。

## 他の路線

参考用として、クリアカーを京成千葉線で走らせるためのシナリオファイルが含まれています。京成千葉線データを同じ Scenarios フォルダーに入れてから起動してください。ただし、自動運転用の地上子を自分で追加しないと自動運転はできません。地上子の追加方法は[チュートリアル](https://github.com/magicant/bve-autopilot/wiki/チュートリアル)を参考にしてください。

## ライセンスとクレジット

このシナリオデータは [magicant](https://github.com/magicant) が作成しました。

このレポジトリーに含まれるファイルは[クリエイティブ・コモンズ 表示 4.0 国際 ライセンス](https://creativecommons.org/licenses/by/4.0/)の元で自由に使用できます。ただし、以下のファイルを除きます。

 - bve-autopilot.dll, bve-autopilot64.dll プラグイン本体
   - このファイルのライセンスは [LGPL 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) です。

またシナリオで参照されている Nagoya_Common 共通ストラクチャパック内のファイルや京成千葉線のファイルはこのレポジトリーに含まれるファイルではないためクリエイティブ・コモンズの対象ではありません。

## 質問・問い合わせ

- [ツイッター](https://twitter.com/tnacigam)で
- [メール](mailto:magicant@wonderwand.net)で
- [Issues](https://github.com/magicant/bve-autopilot-scenario/issues/new) で
