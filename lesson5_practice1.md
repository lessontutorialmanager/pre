# エージェントにスイッチをおさせよう
```block
player.onChat("run", function () {
    agent.interact(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントにスイッチをおさせよう
チャットで**『run』**と入力したときに、**エージェントの前にあるスイッチをおさせる**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/p0PrVYr/tut1.gif"><br>


## エージェントにスイッチをおさせよう
エージェントにスイッチをおさせるプログラムをつくりましょう<br>
`||agent.エージェントを前にインタラクトさせる||`を`||player.チャットコマンド"run"を入力した時||`の中にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/VSZKkFr/tut1pg1.gif"><br>
```block
player.onChat("run", function () {
    agent.interact(FORWARD)
})
```

## エージェントにスイッチをおさせよう
これで、エージェントの前のスイッチをおさせるプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/p0PrVYr/tut1.gif"><br>
