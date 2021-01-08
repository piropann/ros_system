# ROS
2020 RobotSystem Task2

## 概要
ROSを使用したデータをトピックに送信するPublisherとトピックの情報を受信するSubscriberを組み込んだプログラム

## 動作環境

以下の環境にて動作確認を行っています。

- ROS Melodic
  - OS: Ubuntu 18.04.3 LTS
  - ROS Distribution: Melodic Morenia 1.14.3

## 実装方法

- [ROS Wiki](http://wiki.ros.org/ja/kinetic/Installation/Ubuntu)を参照しROSをインストールします。

- `git`を使用して本パッケージをダウンロードします。

```bash
 cd ~/catkin_ws/src
  git clone https://github.com/piropann/driversystem.git
  ```
  
  - `catkin_make`を使用して本パッケージをビルドします。

  ```bash
  cd ~/catkin_ws && catkin_make
  source ~/catkin_ws/devel/setup.bash
  ```
## 動画
画像をクリックしていただけると動画(YouTube)に飛びます。
[![](https://img.youtube.com/vi/PsRcoulrIgI/0.jpg)](https://www.youtube.com/watch?v=PsRcoulrIgI "")

## プログラム起動方法

### パーミッション設定
初回に起動する場合、パーミッションの設定を行わなければならない。
```bash
cd ~/catkin_ws/src/ros_system/src
chmod +x count.py
chmod +x twice.py
  ```
以下になったことを`ls -l`で確認する。
```bash
-rwxrwxr-x ．．．
  ```

### terminal１
```bash
roscore
  ```
  
### terminal２
  ```bash
roslaunch ros_system pubsub.launch
  ```
  
### terminal３

1ずつカウント
```bash
rostopic echo /count_up
  ```
  
2ずつカウント
```bash
rostopic echo /twice
  ```
## LICENSE
MIT
