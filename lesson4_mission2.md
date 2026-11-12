# LESSON2 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがつづけてブロックをおくようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/qRT07kM/q2.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/4YdvTWG/3.png"><br>

## かんがえよう
**上に１ブロックうごく⇒下にブロックをおく**を７回くりかえせばよさそうです<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/XJNFCzb/4.png"><br>

## プログラミングをしよう
エージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
おくブロックをトウヒの原木（げんぼく）ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.トウヒの原木（げんぼく）||`にしましょう<br>
`||loops.１個||`を`||loops.７個||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
})
```

## プログラミングをしよう
エージェントをうごかしてブロックをうごかすプログラムを７回くりかえしましょう<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(トウヒの原木▼)を7個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.setItem(LOG_SPRUCE, 7, 1)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
    agent.move(UP, 1)
    agent.place(DOWN)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう