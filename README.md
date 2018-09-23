## ポモドーロタイマー for bash
* 時間になったら音が鳴るだけのポモドーロタイマー。
* 終了時の効果音は9種類。情報源: [効果音ラボ](https://soundeffect-lab.info/)
* サンプル音: [サンプル](https://raw.githubusercontent.com/matt-note/pomo/master/pomo-sound/start.mp3?raw=true)
* ポモドーロテクニックとは: [link](http://d.hatena.ne.jp/keyword/%A5%DD%A5%E2%A5%C9%A1%BC%A5%ED%A5%C6%A5%AF%A5%CB%A5%C3%A5%AF)

### Usage
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

4. pomo スクリプトを /usr/local/bin にコピー
```bash
$ chmod +x pomo
$ sudo cp pomo /usr/local/bin

# 確認
$ whereis pomo
```

5. pomo を実行
```bash
# デフォルトの設定は 15分
$ pomo
```

6. 作業時間を指定する場合
```bash
# 25分後に終了の合図が鳴る
$ pomo 25

# 効果音の確認用
$ pomo 0

# ラーメンタイマーにも使える
$ pomo 3
```

### 補足事項
* デフォルトの時間設定が15分である理由:

> 人間は最低十五分はどんなに辛い仕事でも集中して取り組むことができる。  
> 「理科系の読書術」 p.21 
