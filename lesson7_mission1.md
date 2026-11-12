# LESSON1 アイテムをつかってエージェントをうごかそう
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

## アイテムをつかってエージェントをうごかしてみよう @unplugged
アイテムをつかってエージェントを自由にうごかせるようになろう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/jfQZwp5/q1.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントが前にすすむ**ようにする<br>
・**【棒】**をもって、右クリックすると**エージェントが左をむく**ようにする<br>
・**【ブレイズロッド】**をもって、右クリックすると*エージェントが右をむく*ようにする<br>
・**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**ようにする<br>
<img style="width:100%" src="https://i.ibb.co/jfQZwp5/q1.gif"><br>

## かんがえよう
このミッションでは**エージェントにラピスラズリを３つ以上集めて**もらいましょう<br>
練習（れんしゅう）ミッションを思いだして、つぎの１つのプログラムをつくってみよう<br>
①**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**プログラム<br>
<img style="width:100%" src="https://i.ibb.co/XZQcPGn/hirou.gif"><br>

## プログラミングをしよう
アイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
<img style="width:100%" src="https://i.ibb.co/cDhgSQT/q1-1.gif"><br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_SHOVEL, function () {
	
})
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.move(FORWARD, 1)
})
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```

## プログラミングをしよう
つかうアイテムをかえましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の**アイテム▼**をクリックして、**鉄のつるはし**にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/V3JVGFG/q1-2.gif"><br>
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
鉄のツルハシをつかったときにエージェントがブロックをこわして、アイテムをひろうプログラムをつくりましょう<br>
`||agent.エージェントに前を破壊（はかい）させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
<img style="width:100%" src="https://i.ibb.co/9Ynbj6X/q1-3.gif"><br>
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
<img style="width:100%" src="https://i.ibb.co/xsRF5hL/q1-4.gif"><br>
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