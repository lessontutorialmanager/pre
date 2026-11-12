# LESSON1 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントをうごかして、きまったばしょに金ブロックをおこう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/nP3ZSjW/1.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがうごいてきまったばしょに金ブロックをおくようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/nP3ZSjW/1.gif"><br>

## かんがえよう
まずはエージェントを**金ブロックをおくばしょまで何ブロックうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/fGThfcg/2024-06-05-203935.png"><br>

## かんがえよう
金ブロックまでは**前に７ブロック**でした<br>
つぎは**金ブロックをおくたかさ**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/X4FXM2V/go1.png"><br>

## かんがえよう
たかさは**２ブロック**でしたね<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
まずは`||agent.エージェントを金ブロックをおくばしょまでうごかす||`プログラムをつくります<br>
<img style="width:100%" src="https://i.ibb.co/yNBRvWq/go2.png"><br>

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
`||loops.1||`を`||loops.7||`に入力しましょう<br>
<img style="width:100%" src="https://i.ibb.co/wBF0f1D/a.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に7ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.上||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/8NfrJCW/b.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントを金ブロックをおくばしょにうごかすプログラムができました<br>
つぎはエージェントに金ブロックをわたして、おくようにプログラミングをしてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/ZzVqyD3/put.gif"><br>

## プログラミングをしよう
エージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||agent.エージェントを上▼に1ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/kHdsdyz/c.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
    agent.move(UP, 1)
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
おくブロックを金ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.金ブロック||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/cQh3MMf/d.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントに(金ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にどらっぐしましょう<br>
<img style="width:100%" src="https://i.ibb.co/Mpy4V9H/e.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 7)
    agent.move(UP, 1)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(FORWARD)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう