# mypkg

# 概要
111～999のゾロ目を連続で表示するプログラムです。

# 動作環境
- Raspberry Pi 4 Model B
- Ubuntu 18.04
- ROS noetic

# 環境構築
ROSの環境が構築されているRaspberry Pi 4 Model B内に、本パッケージを以下のようにインストールします。
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/UDAMAHIRO/mypkg.git
$ cd ~/catkin_ws
$ catkin_make
$ source ~/.bashrc
```
# 実行方法
1.roscoreを立ち上げます。
```
$ roscore
```
2.以下の2つのコードをそれぞれ別の端末上で実行してください。
```
$ rosrun mypkg count.py
$ rosrun mypkg zoro.py
```
3.さらに別の端末上で以下のコードを実行してください。
```
$ rostopic echo /zoro
```
# 動画
https://youtu.be/LsqX5LtWSqQ

# 参照
本コードはこちらの動画内のコードを元に改変を加えたものです。
https://www.youtube.com/watch?v=PL85Pw_zQH0&list=PLbUh9y6MXvjdIB5A9uhrZVrhAaXc61Pzz&index=13&t=4067s

# ライセンス
BSD 3-Clause License
