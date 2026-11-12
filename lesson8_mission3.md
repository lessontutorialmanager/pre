# LESSON3 エージェントに図形をつくらせよう
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
    agent.setItem(GOLD_BLOCK, 4, 1)
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
・エージェントをうごかしてブロックをおかせて、長方形をつくる<br>
・おくブロックの数のちがうプログラムの２つのアイテムをつかう<br>
・**【ニンジン付きの棒】**と**【棒】**をつかう<br>
<img style="width:100%" src="https://i.ibb.co/kDsPkw2/q3-example.gif"><br>

## かんがえよう
２つ目のパズルでエージェントに金ブロックをおかせて、同じブロックの数の棒（ぼう）を４つならべて正方形をつくりました<br>
では長方形をつくるにはどんな棒（ぼう）がいくつ必要（ひつよう）か、かんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/5WxN1wZ/2024-07-26-140345.png"><br>

## かんがえよう
長方形は**長い２つの棒（ぼう）とみじかい２つの棒（ぼう）を組み合わせる**とできます<br>
つぎは長い棒（ぼう）とみじかい棒（ぼう）をつくるには、それぞれエージェントに金ブロックをいくつわたせばいいか、数えましょう<br>
<img style="width:100%" src="https://i.ibb.co/wd8RQ37/4.png"><br>

## かんがえよう
長い棒（ぼう）に必要なブロックの数は**６つ**、みじかい棒（ぼう）に必要なブロックの数は**４つ**でした<br>
【ニンジン付きの棒】を使うと、エージェントに金ブロックを６つわたした後に、ブロックを下におかせる⇒前に１ブロックすすむを６回くりかえす<br>
【棒】を使うと、エージェントに金ブロックを４つわたした後に、ブロックを下におかせる⇒前に１ブロックすすむを４回くりかえす<br>
というプログラムをつくればよさそうです<br>
つぎのページからプログラムをつくっていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/txm5cGV/6.png"><br>

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
つぎの棒（ぼう）をつくるために、エージェントを右にむかせましょう<br>
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
つぎは【棒】**をもって、右クリックすると**エージェントが４つのブロックをおきながら、前にすすむ**プログラムをつくりましょう<br>
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
`||agent.エージェントに前に置かせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下に入れましょう<br>
**前▼**をクリックして、**下**にしましょう<br>
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||agent.エージェントに下に置かせる||`の下に入れましょう<br>

## プログラミングをしよう
つぎの棒（ぼう）をつくるために、エージェントを右にむかせましょう<br>
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
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、**アイテムを持って右クリック**をしてプログラムをうごかしてみましょう
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
    agent.setItem(GOLD_BLOCK, 4, 1)
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