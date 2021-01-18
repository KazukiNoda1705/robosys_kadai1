# robosys_kadai1
ロボットシステム学の課題１です

# 概要
講義内で作成したデバイスドライバのプログラム. 

# 環境
Raspberry Pi4  
Ubuntu 20.04　LTS

# 使用した物
LED 緑色　1個  
青色バーLED　1個  
抵抗　330Ω　3個  
ブレッドボード　1個  
ジャンパー線  
  
![Image]
# 実行手順
## インストール
`git clone`  
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
