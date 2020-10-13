# memo

## ubuntu 20.04 raid-1 installation.

## boot
* BIOSで起動HDDを選択することができるはず。
* 選択したHDDにGrubが入っていれば、Grubの画面が立ち上がる。

## backup linux system users.
* http://hajimenovic.hatenablog.jp/entry/2015/03/20/132845
* /etc 以下の下記ファイルをコピー。ただしユーザIDおよびグループIDに矛盾がないこと。
  * passwd
  * shadow
  * group
  * gshadow
* /home以下を tar でバックアップし、移行先でリストア

## backup ufw settings.
* /lib/ufw/user6.rules を /etc/ufw/user6.rulesへ
* /lib/ufw/user.rules を /etc/ufw/user.rulesへ
* ufw enable

