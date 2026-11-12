# LESSON2 エージェントに図形をつくらせよう
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
    agent.turn(RIGHT_TURN)
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・エージェントをうごかしてブロックをおかせて、正方形をつくる<br>
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントがブロックを下におきながら、前にすすむ**ようにする<br>
・まっすぐブロックをおいたあと、つぎのブロックをおくために**エージェントを右にむかせる**<br>
<img style="width:100%" src="https://i.ibb.co/jgrg4xK/q2-example.gif"><br>

## かんがえよう
１つ目のパズルでエージェントに金ブロックをおかせて、棒（ぼう）をつくりました<br>
では正方形をつくるには棒（ぼう）がいくつ必要（ひつよう）か、かんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/Lv9L196/2024-07-26-135727.png"><br>

## かんがえよう
正方形は**4つの棒（ぼう）を組み合わせる**とできます<br>
つぎは１本目の棒（ぼう）をおいたあとに、**２本目の棒（ぼう）をおくにはエージェントにどのようにうごかせばよいか**、かんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/c2WcGYr/2.png"><br>

## かんがえよう
つぎの順番（じゅんばん）でエージェントをうごかすと２本目の棒（ぼう）をつくることができます<br>
①１本目の棒（ぼう）をつくらせる<br>
②エージェントを右にむかせる<br>
③２本目の棒（ぼう）をつくらせる<br>
<img style="width:100%" src="https://i.ibb.co/Z8WmXYq/seihoukei.gif"><br>

## かんがえよう
**エージェントに棒（ぼう）をつくらせる⇒右をむかせる**プログラムをアイテムを４回つかってうごかしましょう<br>
つぎのページからプログラムをつくっていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/jgrg4xK/q2-example.gif"><br>

## プログラミングをしよう
アイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の**アイテム▼**をクリックして、**ニンジン付きの棒**にしましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
	
})
```

## プログラミングをしよう
ニンジン付きの棒をつかったときにエージェントがブロックを下におくプログラムをつくりましょう<br>
`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GRASS, 1, 1)
})
```

## プログラミングをしよう
**草ブロック**をクリックして、**金ブロック**にして、**１個**を**５個**にしましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
つぎの棒（ぼう）をつくるために、エージェントを右にむかせましょう<br>
`||agent.エージェントの向きを左に変（か）える||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**左▼**をクリックして、**右**にしましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
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
    agent.turn(RIGHT_TURN)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、**ニンジン付きの棒を持って右クリック**をしてプログラムをうごかしてみましょう