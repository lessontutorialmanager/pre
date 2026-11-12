# エージェントの左にブロックをおこう
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
})
```

```template
player.onChat("run", function () {
	
})
```
## エージェントの左にブロックをおこう
チャットで**『run』**と入力したときに、**エージェントの左に金ブロックをおく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/wwDhHGr/agentsetleft.gif"><br>

## エージェントの左にブロックをおこう
まずはエージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/KrNyzsR/glassset.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS, 1, 1)
})
```

## エージェントの左にブロックをおこう
おくブロックを金ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.金ブロック||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/8zwGB4Z/goldchange.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
})
```

## エージェントの左にブロックをおこう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(金ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/f006yFm/setforward.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

## エージェントの左にブロックをおこう
ブロックをおくばしょをかえましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`の`||agent.前▼||`をクリックして、`||agent.左▼||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/DM8gDS6/setleft.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
})
```

## エージェントの左にブロックをおこう
これで、エージェントの左に金ブロックをおくプログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/wwDhHGr/agentsetleft.gif"><br>