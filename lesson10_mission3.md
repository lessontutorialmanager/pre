# エージェントをアイテムをつかってうごかそう
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

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・アイテムをつかってエージェントにダイヤモンドブロックをこわさせるようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/7YZyhbs/q3-ex.gif"><br>

## かんがえよう
まずはLesson７を思いだして、**自分でプログラミングしてみましょう**<br>
もし、思いだせないときは**次（つぎ）へ**をおして、プログラミングのつくり方を見てみましょう<br>

## かんがえよう
・**【ニンジン付きの棒】**をもって、右クリックすると**エージェントが前にすすむ**ようにする<br>
・**【棒】**をもって、右クリックすると**エージェントが左をむく**ようにする<br>
・**【ブレイズロッド】**をもって、右クリックすると*エージェントが右をむく*ようにする<br>
・**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわす**ようにする<br>
つぎのページからプログラムをつくっていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/8cgv5sR/2024-07-28-153115.png"><br>


## プログラミングをしよう
まずは【ニンジン付きの棒】**をもって、右クリックすると**エージェントが前にすすむ**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**ニンジン付きの棒**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントを前に１ブロック移動（いどう）させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>

## プログラミングをしよう
つぎは**【棒】**をもって、右クリックすると**エージェントが左をむく**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**棒**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントの向（む）きを左に変（か）える||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>

## プログラミングをしよう
つぎは**【ブレイズロッド】**をもって、右クリックすると**エージェントが右をむく**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**ブレイズロッド**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントの向（む）きを左に変（か）える||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>
**左▼**をクリックして、**右**にしましょう<br>

## プログラミングをしよう
さいごに**【鉄のツルハシ】**をもって、右クリックすると**エージェントが目の前のブロックをこわして、アイテムをひろう**プログラムをつくりましょう<br>
`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`をドラッグしてだしましょう<br>
**アイテム▼**をクリックして、**鉄のツルハシ**にしましょう<br>

## プログラミングをしよう
`||agent.エージェントに前を破壊（はかい）させる||`を`||player.次（つぎ）のアイテムが使（つか）われた時（とき）||`の中に入れましょう<br>


## かくにんしよう
できたプログラムが正しいか、💡ボタンをおしてかくにんしましょう<br>
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

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう
<img style="width:100%" src="https://i.ibb.co/bW6bphv/tutorialpractice1.gif"><br>