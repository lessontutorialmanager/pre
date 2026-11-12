# LESSON2 エージェントをうごかしてスイッチをおさせよう
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
    agent.move(UP, 4)
    agent.move(FORWARD, 1)
    agent.interact(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがスイッチの前にうごいて、スイッチをおすようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/m555NcM/quiz2.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/2624Gd4/2.png"><br>

## かんがえよう
**前に５ブロックうごく⇒スイッチをおす⇒上に４ブロック⇒前に１ブロック⇒スイッチをおす**ようにプログラミングをしましょう<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/G7gN7rf/3.png"><br>

## プログラミングをしよう
まずは１つめのスイッチをエージェントにおさせるプログラムをつくりましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントをうごかす数をいれましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||loops.１ブロック||`を`||loops.5ブロック||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
})
```

## プログラミングをしよう
エージェントにスイッチをおさせましょう<br>
`||agent.エージェントを前に向けてインタラクトさせる||`を`||agent.エージェントを前に５ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
})
```

## プログラミングをしよう
つぎに２つめのスイッチをエージェントにおさせるプログラムをつくりましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`を`||agent.エージェントを前に向けてインタラクトさせる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントをうごかす数をいれましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.上||`にしましょう<br>
つぎに`||loops.１ブロック||`を`||loops.４ブロック||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
    agent.move(UP, 4)
})
```

## プログラミングをしよう
`||agent.エージェントを前に1ブロック移動（いどう）させる||`を`||agent.エージェントを上に４ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
    agent.move(UP, 4)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントにスイッチをおさせましょう<br>
`||agent.エージェントを前に向けてインタラクトさせる||`を`||agent.エージェントを前に１ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
    agent.interact(FORWARD)
    agent.move(UP, 4)
    agent.move(FORWARD, 1)
    agent.interact(FORWARD)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう