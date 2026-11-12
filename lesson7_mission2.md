# LESSON2 アイテムをつかってエージェントをうごかそう
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
    agent.collectAll()
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

```template
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントが前にすすむ**ようにする<br>
・**【棒】**をもって、右クリックすると**エージェントが左をむく**ようにする<br>
・**【ブレイズロッド】**をもって、右クリックすると*エージェントが右をむく*ようにする<br>
・**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**ようにする<br>
<img style="width:100%" src="https://i.ibb.co/r42DjT8/q2.gif"><br>

## かんがえよう
このミッションでは**エージェントにエメラルドを５つ以上集めて**もらいましょう<br>
練習（れんしゅう）ミッションを思いだして、つぎの３つのプログラムをつくってみよう<br>
①**【棒】**をもって、右クリックすると**エージェントが左をむく**ようにする<br>
②**【ブレイズロッド】**をもって、右クリックすると*エージェントが右をむく*ようにする<br>
③**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**プログラム<br>
<img style="width:100%" src="https://i.ibb.co/LpmjR3d/hidari.gif"><br>
<img style="width:100%" src="https://i.ibb.co/thjC7gQ/migi.gif"><br>

## プログラミングをしよう
まずは**【棒】**をもって、右クリックすると**エージェントが左をむく**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**棒**にしましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
	
})
```

## プログラミングをしよう
`||agent.エージェントの向（む）きを左に変（か）える||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

## プログラミングをしよう
つぎは**【ブレイズロッド】**をもって、右クリックすると**エージェントが右をむく**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**ブレイズロッド**にしましょう<br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
	
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})

```

## プログラミングをしよう
`||agent.エージェントの向（む）きを左に変（か）える||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
**左▼**をクリックして、**右**にしましょう<br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

## プログラミングをしよう
さいごに**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**鉄のツルハシ**にしましょう<br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_PICKAXE, function () {
	
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})

```


## プログラミングをしよう
`||agent.エージェントに前を破壊（はかい）させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

## プログラミングをしよう
`||agent.エージェントに全（すべ）て拾（ひろ）わせる||`を`||agent.エージェントに前を破壊（はかい）させる||`の下に入れましょう<br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
    agent.collectAll()
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、**アイテムを持って右クリック**してプログラムをうごかしてみましょう