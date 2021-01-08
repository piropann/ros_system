# ROS
2020 RobotSystem Task2

## 概要
ROSを使用したPublisherとSubscriberのプログラム作成

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
  
  ## プログラム起動方法

```bash
  roscore
  ```
  
