# LESSON2 エージェントにブロックをこわさせよう
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがうごいて、ブロックをこわすようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/MR5HdR6/quiz2.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/sPhWkfw/2024-07-03-221952.png"><br>

## かんがえよう
**前のブロックをこわす⇒左に1ブロックすすむ⇒前のブロックをこわす⇒前に１ブロック⇒前のブロックをこわす⇒前に１ブロック⇒前のブロックをこわす⇒左に１ブロック⇒前のブロックをこわす**ようにプログラミングをしましょう<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/BsGYTcw/2.png"><br>

## プログラミングをしよう
まずは前のブロックをエージェントにこわさせるプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
})
```

## プログラミングをしよう
エージェントを左にうごかしましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||agent.エージェントの前を破壊（はかい）させる||`の下にいれましょう<br>
`||loop.前||`を`||loop.左||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
})
```

## プログラミングをしよう
つぎの前のブロックをエージェントにこわさせるプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||agent.エージェントを左に1ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
})
```

## プログラミングをしよう
エージェントを前にうごかしましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||agent.エージェントの前を破壊（はかい）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
つぎの前のブロックをエージェントにこわさせるプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||agent.エージェントを前に1ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
})
```

## プログラミングをしよう
エージェントを前にうごかしましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||agent.エージェントの前を破壊（はかい）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
})
```


## プログラミングをしよう
つぎの前のブロックをエージェントにこわさせるプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||agent.エージェントを前に1ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
})
```

## プログラミングをしよう
エージェントを左にうごかしましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||agent.エージェントの前を破壊（はかい）させる||`の下にいれましょう<br>
`||loop.前||`を`||loop.左||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
})
```

## プログラミングをしよう
さいごのブロックをエージェントにこわさせるプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||agent.エージェントを左に1ブロック移動（いどう）させる||`の下にいれましょう<br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
    agent.move(LEFT, 1)
    agent.destroy(FORWARD)
})
```


## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう