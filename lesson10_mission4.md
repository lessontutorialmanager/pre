# 図形をつくろう
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 6, 1)
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
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(STICK, function () {
    agent.setItem(GOLD_BLOCK, 3, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・アイテムをつかってエージェントに図形をつくらせるようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/vLSZq2N/q4-ex.gif"><br>

## かんがえよう
まずはLesson８を思いだして、**自分でプログラミングしてみましょう**<br>
もし、思いだせないときは**次（つぎ）へ**をおして、プログラミングのつくり方を見てみましょう<br>

## かんがえよう
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントがブロックを下におきながら、６ブロック前にすすむ**ようにする<br>
・**【棒】**をもって、右クリックすると**エージェントがブロックを下におきながら、３ブロック前にすすむ**ようにする<br>
つぎのページからプログラムをつくっていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/jLswMRf/2024-07-28-155303.png"><br>


## プログラミングをしよう
まずは【ニンジン付きの棒】**をもって、右クリックすると**エージェントが６つのブロックをおきながら、前にすすむ**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**ニンジン付きの棒**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
**草ブロック**をクリックして、**金ブロック**にして、**１個**を**６個**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントの向きを左に変（か）える||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**左▼**をクリックして、**右**にしましょう<br>
**正しくプログラムがつくれているか、しんぱいな人は💡マークをクリックしてプログラムを見てみましょう**<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 6, 1)
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
    agent.turn(RIGHT_TURN)
})
```

## プログラミングをしよう
つぎは【棒】**をもって、右クリックすると**エージェントが３つのブロックをおきながら、前にすすむ**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**棒**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
**草ブロック**をクリックして、**金ブロック**にして、**１個**を**４個**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントにブロックを1個、自分のスロット１番に設定させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
`||agent.エージェントの向きを左に変（か）える||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**左▼**をクリックして、**右**にしましょう<br>
**正しくプログラムがつくれているか、しんぱいな人は💡マークをクリックしてプログラムを見てみましょう**<br>
```block
player.onItemInteracted(STICK, function () {
    agent.setItem(GOLD_BLOCK, 4, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
})
```

## かくにんしよう
できたプログラムが正しいか、💡ボタンをおしてかくにんしましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 6, 1)
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
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(STICK, function () {
    agent.setItem(GOLD_BLOCK, 3, 1)
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
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう
<img style="width:100%" src="https://i.ibb.co/bW6bphv/tutorialpractice1.gif"><br>