# エージェントを前（まえ）にすすめよう
```block
player.onChat("run", function () {
	agent.move(FORWARD, 1)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントを前（まえ）に１ブロックうごかそう
チャットで**『run』**と入力したときに、**エージェントを前（まえ）に１ブロックうごく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/stgYrhC/tutorialpractice2.gif"><br>

## エージェントを前（まえ）に１ブロックうごかそう
エージェントをうごかすためのプログラムブロックをだします<br>
`||agent.エージェント||`をクリックして、`||エージェントを前（まえ）▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時（とき）||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/P9MsSxN/tutorialpractice3.gif"><br>
```block
player.onChat("run", function () {
	agent.move(FORWARD, 1)
})
```

## エージェントを前（まえ）に１ブロックうごかそう
これで、エージェントを前（まえ）に１ブロックうごかすためのプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/cQRMY6c/tutorialpractice4.gif"><br>
