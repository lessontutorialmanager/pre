# エージェントにブロックをこわさせよう
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントにブロックをこわさせよう
チャットで**『run』**と入力したときに、**エージェントの前にあるブロックをこわさせる**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/VLnnH2T/break.gif"><br>


## エージェントにブロックをこわさせよう
エージェントにブロックをこわさせるプログラムをつくりましょう<br>
`||agent.エージェントに前を破壊（はかい）させる||`を`||player.チャットコマンド"run"を入力した時||`の中にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/d6z32sG/tut1.gif"><br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
})
```

## エージェントにブロックをこわさせよう
これで、エージェントの前のブロックをこわさせるプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/VLnnH2T/break.gif"><br>
