# エージェントを右にうごかそう
```block
player.onChat("run", function () {
	agent.move(RIGHT, 1)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントを右に１ブロックうごかそう
チャットで**『run』**と入力したときに、**エージェントを右に１ブロックうごく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/GCr5R2m/tutorialpractice7.gif"><br>

## エージェントを右に１ブロックうごかそう
エージェントをうごかすためのプログラムブロックをだします<br>
`||agent.エージェント||`をクリックして、`||エージェントを前（まえ）▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時（とき）||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/P9MsSxN/tutorialpractice3.gif"><br>
```block
player.onChat("run", function () {
	agent.move(FORWARD, 1)
})
```

## エージェントを右に１ブロックうごかそう
エージェントをうごかすためのプログラムブロックをだします<br>
`||エージェントを前（まえ）▼に１ブロック移動（いどう）させる||`の**前▼**をクリックして、**右▼**にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/vPdVsBm/tutorialpractice5.gif"><br>
```block
player.onChat("run", function () {
	agent.move(RIGHT, 1)
})
```

## エージェントを右に１ブロックうごかそう
これで、エージェントを右に１ブロックうごかすためのプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/GCr5R2m/tutorialpractice7.gif"><br>
