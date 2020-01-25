# b4のラズパイのプログラム管理用のリポジトリ

## リポジトリの説明
B4用のラズパイである, ホスト名 : amlab･ユーザー : piのホームディレクトリ上にあるspl-meter-with-RPiディレクトリのリモートリポジトリです.  
元々ホームディレクトリ上にあったtestLCD_record2.pyはこちらに入れました.  

## プログラム説明
### 全体の説明
testLCD_record2~.pyは, MEMSマイクから拾った音圧データにA特性重み付けをしてRMSレベルをラズパイ付属の小型ディスプレイに表示しようとしたものです.  
### 各プログラム説明
* testLCD_record2.py : 以前のtestLCD_record2からspl_meter_textのlisten関数を呼び出したものです  
* testLCD_record5.py : spl_meter_textの後ろに, 以前のtestLCD_record2を付け加えたものです(唯一エラーなく動作します)  

## 問題点
### プログラムの問題点
* pip updateを実行してから, pipコマンドにおいてmainが見つかりませんというエラーが発生中(pip3では可能)  
### ラズパイの問題点
* ラズパイのストレージが厳しくなってきており, 追加でパッケージのインストールなどができない可能性が大きい  
* spl_meter_textはローカルでの変更を反映できていない可能性があります

## 課題
### プログラム全体としての課題
* spl-meter-with-RPiパッケージを用いて周波数分析や周波数特性重み付けを実装したい(もしくは, サウンドプログラミング演習のプログラムをベースに同じ機能を実装したい) 
### プログラムの課題詳細
* testLCD_record5.pyのプログラムは読めていないので, 本当にA特性重み付けがされていることを確認できていない  
### ラズパイの課題
* ｢.bash_profile｣ファイルに｢python --version｣を追加し, python3系で実行されていればOK! ただ, ホームディレクトリではpython2系となるはず.

