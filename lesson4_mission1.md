# LESSON1 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントをうごかして、土の道（みち）ブロックをおこう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/Hxg9jnx/q1re.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがつづけてブロックをおくようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/qBCMrmK/q1re2.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/pb9v041/1.png"><br>

## かんがえよう
**前に１ブロックうごく⇒下にブロックをおく**を３回くりかえせばよさそうです<br>
プログラムのはじめにブロックを３つわたすことを、わすれないようにしましょう<br>
<img style="width:100%" src="https://i.ibb.co/HgV8dMc/2.png"><br>

## プログラミングをしよう
エージェントにブロックをもたせましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/N1X2Fgb/q1-1.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
おくブロックを土の道（みち）ブロックにしましょう<br>
`||agent.エージェントに(草ブロック▼)を１個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の`||loops.草ブロック||`をクリックして、`||loops.土の道（みち）||`にしましょう<br>
`||loops.１個||`を`||loops.3個||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/1KF2gvF/q1-2.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
})
```

## プログラミングをしよう
エージェントをうごかしてブロックをうごかすプログラムを３回くりかえしましょう<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに(土の道▼)を3個（こ）、自分（じぶん）のスロット１番（ばん）に設定（せってい）させる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/vhgJZkv/q1-3.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントにブロックをおかせましょう<br>
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/RYtQfww/q1-4.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに下▼へ置（お）かせる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/nMXB9DQ/q1-5.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/Lptwkns/q1-6.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントに下▼へ置（お）かせる||`の下にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/6wxvh8Y/q1-7.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前▼へ置（お）かせる||`を`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.前▼||`をクリックして`||agent.下||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/NCfFQ3m/q1-8.gif"><br>
```block
player.onChat("run", function () {
    agent.setItem(GRASS_PATH, 3, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう