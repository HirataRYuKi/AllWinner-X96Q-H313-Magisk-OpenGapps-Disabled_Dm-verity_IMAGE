# AllWinner-X96Q-H313-Magisk-OpenGapps-Disabled_Dm-verity_IMAGE
**x96q 2g/16gバージョンのものになっています。**
Realeaseのほうに全部上げてます
* Magisk-26.4を適応済み
* open_gapps-arm-10.0-tvstock-20220215.zipをMagiskモジュールに変換してインストール済み（ログインもOK）
* MagiskHide Props Configを使用して「NVIDIA SHIELDTV 2019」に偽造してDRMもOK
* Dm-verityもオフになっています。
* Magiskを入れる前からある「su」バイナリは名前を「zu」に変更しています。
* Allwinner製のアプリは一応すべて削除（なぜかアプリ一覧には表示されるが、アプリがないと表示される）
* 一応、デバイスツリーとTWRPも公開しておきます（今のところストレージをうまく認識しない）
* ただ、私の端末のパーティションをddで書き出しているだけなので、動くかよくわかっていません。（自己責任でお願いします）
* super.imgを書き込む際は「flash --disable-verity --disable-verification super super.img」で書き込んでください。
* いろいろ分かったけど、X96Q系のuserdataが見えてる版のイメージが一番TWRPとの相性が良かった。ただ、いろいろ機能が使えなかったりする（CECが使えなかったり）
* opengappsを入れた後、ログインしようとするとログイン画面が落ちることがあるが、adbで「adb shell pm disable-user --user 0 com.google.android.tungsten.setupwraith」を実行すると、落ちなくなる。
* TWRP導入する方は、モジュール化したOpenGappsを使わなくてもインストールは可能。ただ、TWRPにバグがあるので、きちんと書き込めているか不明。

**Allwinner製のライターで書き込めるようにパックしてくれ（願望）**
