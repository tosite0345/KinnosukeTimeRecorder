# Kinnosuke Time Recorder

万屋一家シリーズ web版勤怠管理システム「勤之助 ver.2」のタイムレコーダーを押すためのChrome Extensionです。
勤之助はログインセッションのTTLがすごく短いのですが、このExtensionを使うといちいちログインする必要なく、勤怠ボタンを押したり、勤之助を開いたりできます。

## インストール

Chrome ウェブストアから「[勤之助タイムレコーダー](https://chrome.google.com/webstore/detail/%E5%8B%A4%E4%B9%8B%E5%8A%A9%E3%82%BF%E3%82%A4%E3%83%A0%E3%83%AC%E3%82%B3%E3%83%BC%E3%83%80%E3%83%BC/onohbjcjcdlmfheogadpfopadlmpicmk)」をインストールしてください。


## 使い方

- まずはメニューから「オプション」を開き、勤之助のログイン情報を入力します。
- 出社、退社したらメニューの「出社」や「退社」をクリックしてください。
- ![勤之助](https://github.com/irok/KinnosukeTimeRecorder/raw/master/images/icon19.png) のところに表示される小さな ■ は現在の状態を表しています。
  - 黄：未出社
  - 緑：出社
  - 青：退社

## 安全性について

- ログイン情報はlocalStorageに保存します。どこかのサーバーに送信したりはしません。（勤之助には送信します。）
- パスワードは暗号化した状態で保存しますが、暗号キーもlocalStorageに保存するので、マスターキーなしでブラウザにパスワード保存しているのと大して変わりません。（デベロッパーツールでうっかりlocalStorageを開いても生のパスワードは見られずにすむ、程度の効果です。）

