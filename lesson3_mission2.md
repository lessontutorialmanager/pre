# LESSON2 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
    agent.setItem(EMERALD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがうごいてきまったばしょに金ブロックをおく<br>
・金ブロックをおいたあとに、さらにエージェントがうごいてきまったばしょにエメラルドブロックをおくようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/xHXdqg1/2.gif"><br>

## かんがえよう
エージェントを金ブロックをおくばしょにうごかす**⇒**金ブロックをおく**⇒**エージェントをエメラルドブロックをおくばしょにうごかす**⇒**エメラルドブロックをおく<br>
というプログラムをつくりましょう<br>
まずはエージェントを**金ブロックをおくばしょまで何ブロックうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/GxHCBqN/2024-06-05-204035.png"><br>

## かんがえよう
**前に４⇒左に２⇒前に１⇒上に１**でした<br>
つぎは金ブロックをおいたあとに、**エメラルドブロックをおくばしょまで何ブロックうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/41zSFnS/3.png"><br>

## かんがえよう
**前に１⇒右に４⇒上に３**でした<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/s6DtJVq/4.png"><br>

## プログラミングをしよう
エージェントをうごかすためのプログラムブロックを出します<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
`||loops.1||`を`||loops.4||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に4ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.左||`にしましょう<br>
`||loops.1||`を`||loops.2||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを左▼に2ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に4ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||agent.エージェントを上▼に1ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
おくブロックを金ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.金ブロック||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(金ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

## プログラミングをしよう
ブロックを**左に**おかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(金ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.前▼||`をクリックして、`||loops.左||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
})
```

## かんがえよう
これで**金ブロックをきまったばしょにおくプログラム**ができました<br>
つづいてエメラルドブロックをきまったばしょにおくプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/s6DtJVq/4.png"><br>

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに左に置（お）かせる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に1ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.右||`にしましょう<br>
`||loops.1||`を`||loops.4||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを右▼に4ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.上||`にしましょう<br>
`||loops.1||`を`||loops.3||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
})
```

## プログラミングをしよう
エージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||agent.エージェントを上▼に3ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
おくブロックをエメラルドブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.エメラルドブロック||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
    agent.setItem(EMERALD_BLOCK, 1, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(エメラルドブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 4)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 1)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(LEFT)
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
    agent.setItem(EMERALD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう