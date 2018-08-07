## Ubuntu 用? ポモドーロタイマー
* 効果音： [効果音ラボ](https://soundeffect-lab.info/)
* ポモドーロテクニックとは: [link](http://d.hatena.ne.jp/keyword/%A5%DD%A5%E2%A5%C9%A1%BC%A5%ED%A5%C6%A5%AF%A5%CB%A5%C3%A5%AF)
* pomo では、休憩用の効果音は無い。  


1. 音声再生用に mpv のインストール
```bash
$ sudo apt install mpv
```

2. リポジトリをクローン
```bash
$ git clone git@github.com:matt-note/pomo.git
```

3. pomo-sound ディレクトリをホームディレクトリにコピー
```bash
$ cd pomo
$ cp -r pomo-sound $HOME
```

4. pomo スクリプトをPATHに移動
```bash
$ chmod +x pomo
$ sudo cp pomo /usr/local/bin

# 確認
$ whereis pomo
```

5. pomo を実行
```bash
# デフォルトで 15分に設定してある
$ pomo
```

6. pomo に引数を与えて実行
```bash
# 25分後に終了の合図が鳴る
$ pomo 25

# 効果音確認用に1分後に設定
$ pomo 1
```

### 補足事項
* デフォルトの時間設定が15分である理由:

> 人間は最低十五分はどんなに辛い仕事でも集中して取り組むことができる。  
> 「理科系の読書術」 p.21 
