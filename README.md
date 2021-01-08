# ROS
2020 RobotSystem Task2

## 概要
ROSを使用したPublisherとSubscriberのプログラム作成

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

terminal１
```bash
roscore
  ```
  
terminal２
  ```bash
roslaunch ros_system pubsub.launch
  ```
  
terminal３

1ずつカウント
```bash
rostopic echo /count_up
  ```
  
2ずつカウント
```bash
rostopic echo /twice
  ```
