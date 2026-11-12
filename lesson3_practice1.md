# エージェントの前にブロックをおこう
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントの前にブロックをおこう
チャットで**『run』**と入力したときに、**エージェントの前に金ブロックをおく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/Y2K8G0s/agentsetmae.gif"><br>

## エージェントの前にブロックをおこう
まずはエージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/KrNyzsR/glassset.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS, 1, 1)
})
```

## エージェントの前にブロックをおこう
おくブロックを金ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.金ブロック||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/8zwGB4Z/goldchange.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
})
```

## エージェントの前にブロックをおこう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(金ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/f006yFm/setforward.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

## エージェントの前にブロックをおこう
これで、エージェントの前に金ブロックをおくプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/Y2K8G0s/agentsetmae.gif"><br>
