# robosys2020_work2

### 概要
ロボットシステム学の授業で作成したROSパッケージを動かす．

### 動作環境  
・Rasberry Pi Model 3    
・Ubuntu 20.04  
・ROS noetic
（ROSのインストールについて）
[ros_setup_scripts_Ubuntu20.04](http://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server)を参照

### インストール
`cd ~/catkin_ws/src`  
`git clone https://github.com/yusuke-taki/robosys2020_work2.git`  

### 実行
ノードを立ち上げてトピックとしてデータを得るまで

端末１  
`cd ~/catkin_ws`  
`catkin_make`  
`source ~/bashrc`  
`roscore`  

端末２  
`chmod +x count.py`
`rosrun mypkg count.py`  

端末３  
`chmod +x twice.py`
`rosrun mypkg twice.py`  

端末４  
`rostopic echo /twice`  

### デモ動画
