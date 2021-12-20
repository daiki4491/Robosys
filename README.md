# Robosys
レポジトリをロボットシステム工学の課題１です。


# 今回の課題にあたって

　今回の課題にあたって、


# 概要

　このプログラムは、講義内で上田先生が製作してプログラムを参考に自身で改造し、LEDを点灯・消灯を行うプログラムです。
 
 
 # 動作環境
　
 |　  OS    |  Ubuntu20.04server |
 ---|---
 | Hardware |  Raspberry Pi 4 |
 
 
 # 用意した物
 
  ・Raspberry　Pi 4
  
  ・ブレッドボード
  
  ・LED（赤/黄）*2
  
  ・抵抗(200Ω)*2
  
  ・ジャンパー線*4
  
  
 # 回路
 
 　今回作成した回路は、以下のように回路を組みました。
  
  <img src=
  "https://user-images.githubusercontent.com/96305606/146736978-be1998fc-2739-4b6f-ad2d-b396fbb6202f.jpg" widrh= "320px">
  
  
  # インストール・ビルド・アンインストール方法
  
  　以下の順序で実行してください。
   
   ・インストール手順
   
   　$ git clone https://github.com/daiki4491/Robosys.git
    
     $ cd Robosys
     
     $ make
     
     $ sudo insmod myled.ko
     
     $ sudo chmod 666 /dev/myled0
     
   ・実行手順
   
     $ echo 0 > /dev/myled0
            （LED1を消灯）
     
     $ echo 1 > /dev/myled0
            （LED２を消灯）
     
     $ echo 2 > /dev/myled0
             （LED1を点灯）
             
     $ echo 3 > /dev/myled0
             （LED2を点灯）
             
   ・終了、アンインストール手順
   
      $ sudo rmmod myled
     
   
   
  # 実行結果
  
  　以下のリンクからyoutubeの動画がご覧出来ます。
    
    https://youtu.be/P4NYrSSYEhY
    
    
    
    
    
    
    
    
