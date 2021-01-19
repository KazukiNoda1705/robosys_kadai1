# robosys_kadai1
ロボットシステム学の課題１です

# 概要
講義内で作成したデバイスドライバのプログラム.  
LEDバー２つと緑色のLEDライト1つが点灯, 消灯します.  

# 環境
Raspberry Pi4  
Ubuntu 20.04　LTS

# 使用した物
LED 緑色　1個  
青色バーLED　1個  
抵抗　330Ω　3個  
ブレッドボード　1個  
ジャンパー線  
  
![IMG_5697](https://user-images.githubusercontent.com/73329238/104943099-987ca880-59f8-11eb-8ed7-7aa6319cb883.JPG)  
Raspberry PiのGPIO 4番, 17番をLEDバーのアノードに接続  
緑色のLEDは, 17番と繋がっている. 

# 実行手順
## インストール
`git clone https://github.com/KazukiNoda1705/robosys_kadai1.git`  
`make`  
`sudo insmod myled.ko`  
`sudo chmod 666 /dev/myled0`　　
  
## LEDの点灯・消灯方法  
LEDが2つ点灯する  
`echo F > /dev/myled0`  
LEDが1つ点灯する  
`echo H > /dev/myled0`  
LEDが全て消灯する  
`echo E > /dev/myled0`  

# 映像
[youtube](https://youtu.be/YrYsSWS5VXU)
