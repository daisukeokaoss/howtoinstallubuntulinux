## Ubuntu Desktop Linuxのインストール方法

今回はUbuntu Linuxのインストール方法の紹介をさせていただきます。  

この記事はサイバー大学文化祭「オンやる」での活動の一環として書いてます。  
https://onyaru.com/

* 自己紹介
いつもはオンラインで勉強会開いてます。現在精神疾患のため休職中。IBM Powerシステムでお金稼ぎ画策中です。   

https://connpass.com/user/daisukeokaoss/


Ubuntu Linuxとは、Linuxのディストリビューションの一つで、デスクトップLinuxの中では有名なものの一つです。    

では、Ubuntu Linuxのインストール方法を書いていきます。  

準備するもの
*  PC（古くても良い。あまり新しいものはドライバが対応してないことがある。)
*  USBメモリ

以下のサイトでUbuntu Desktopをダウンロードします。  
https://ubuntu.com/

今だと20.04 LTSが良いかもしれません。ちなみに21.04も使用しましたが、Skypeの画面共有ができなかったです。  
大きなファイルなので少し時間がかかります。  

次にダウンロードしたイメージをインストールのためUSBメモリに焼きましょう。以下のツールを使用します。  

https://www.balena.io/etcher/

balena etcherはオープンソースなので無料でダウンロードできます。  
Linux、Windows、MacOSで使用できます。

USBメモリに焼いたあとは、USBメモリをPCに刺し、BIOS設定を書き換えて再起動します。  
BOOT順序の一番目をUSBにする必要があります。  
そして再び起動すれば、OSのインストーラーが走ります。  
指示に従えば、Ubuntu Linuxがインストールされます。

Ubuntu Linuxのインストールが終わったら、OSのアップデートを必ずしてください。  
「端末」を起動し、以下のコマンドを実行してください。  
(注：GUIでのアップデートのみだと不十分なことがあるようです。かならず端末でもアップデートをお願いします。wifiに不具合起きます。また、端末でアップデートすればGUIでのアップデートは必要ありません）  

```
$ sudo apt update
$ sudo apt dist-upgrade
$ sudo apt autoremove
```

これで使用準備完了です。  

参考文献

https://qiita.com/masoo/items/8ebc51a6a9f32417d4a3
