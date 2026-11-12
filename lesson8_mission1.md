# LESSON1 エージェントに図形をつくらせよう
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```


## アイテムをつかってエージェントをうごかして、図形をつくらせよう @unplugged
アイテムをつかってエージェントを自由にうごかして、図形をつくらせよう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/T80Vzjj/q1-example.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントがブロックを下におきながら、前にすすむ**ようにする<br>
<img style="width:100%" src="https://i.ibb.co/T80Vzjj/q1-example.gif"><br>

## かんがえよう
まずはエージェントに金ブロックをいくつわたせばいいか、数えましょう<br>
<img style="width:100%" src="https://i.ibb.co/gSmMZww/2024-07-26-134820.png"><br>

## かんがえよう
必要なブロックの数は**７つ**でした<br>
エージェントに金ブロックを７つわたした後に、ブロックを下におかせる⇒前に１ブロックすすむを７回くりかえせばよさそうです<br>
つぎのページからプログラムをつくっていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/09SBW5g/1.png"><br>

## プログラミングをしよう
アイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
<img style="width:100%" src="https://i.ibb.co/zN7HD84/q1-1.gif"><br>
```block
player.onItemInteracted(IRON_SHOVEL, function () {
	
})
```

## プログラミングをしよう
つかうアイテムをかえましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の**アイテム▼**をクリックして、**ニンジン付きの棒**にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/Rv6YdCR/q1-2.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
	
})
```

## プログラミングをしよう
ニンジン付きの棒をつかったときにエージェントがブロックを下におくプログラムをつくりましょう<br>
`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/vV5N3dF/q1-3.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
**草ブロック**をクリックして、**金ブロック**にして、**１個**を**７個**にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/VY4gVgg/q1-4.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/CnyJm3G/q1-5.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
})
```

## プログラミングをしよう
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/LNWvNjq/q1-6.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/drLp7MR/q1-7.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/k0HxstP/q1-8.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```


## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/2hxFqcL/q1-9.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/dGQRZmb/q1-10.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/Z6zCL5D/q1-11.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/MMGMfmt/q1-12.gif"><br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 7, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、**ニンジン付きの棒を持って右クリック**をしてプログラムをうごかしてみましょう