# アイテムを使ってエージェントをうごかそう
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
```

## アイテムを使ってエージェントをうごかそう
**【ブレイズロッド】をもって、右クリックするとエージェントが右をむく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/thjC7gQ/migi.gif"><br>


## アイテムを使ってエージェントをうごかそう
このレッスンでは`||player.チャットコマンド"run"を入力した時||`をつかいません<br>
`||player.チャットコマンド"run"を入力した時||`をツールボックスまでドラッグして、けしましょう<br>
<img style="width:100%" src="https://i.ibb.co/0C6zb4b/runsuteru.gif"><br>

## アイテムを使ってエージェントをうごかそう
プレイヤーにアイテムをわたしましょう<br>
`||mobs.アイテムを与える 対象 一番近いプレイヤー(@p) アイテム/ブロック 数１||`を`||loops.最初（さいしょ）だけ||`の中にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/GpTXNBJ/tut1-1.gif"><br>
```block
mobs.give(
mobs.target(NEAREST_PLAYER),
GRASS,
1
)
```

## アイテムを使ってエージェントをうごかそう
プレイヤーにわたすアイテムをかえましょう<br>
`||blocks.ブロック||`の中の`||blocks.アイテム||`を`||mobs.アイテムを与える 対象 一番近いプレイヤー(@p) アイテム/ブロック 数１||`の**ブロック**にかさねましょう<br>
**鉄のシャベル**をクリックして、**ブレイズロッド**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/vsdVM4t/tut3-2.gif"><br>
```block
mobs.give(
mobs.target(NEAREST_PLAYER),
BLAZE_ROD,
1
)
```

## アイテムを使ってエージェントをうごかそう
プレイヤーがアイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.プレイヤー||`の中の`||player.次（つぎ）のアイテムが使（つか）われたとき||`をドラッグして、だしましょう<br>
**鉄のシャベル**をクリックして、**ブレイズロッド**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/xfZfvC2/tut3-3.gif"><br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
	
})
mobs.give(
mobs.target(NEAREST_PLAYER),
BLAZE_ROD,
1
)
```

## アイテムを使ってエージェントをうごかそう
`||agent.エージェントの向（む）きを左に変（か）える||`をドラッグして、`||player.次（つぎ）のアイテムが使（つか）われたとき||`の中にいれましょう<br>
`||agent.左||`をクリックして、`||agent.右||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/xqLQ8d7/tut3-4.gif"><br>
```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
mobs.give(
mobs.target(NEAREST_PLAYER),
BLAZE_ROD,
1
)
```

## アイテムを使ってエージェントをうごかそう
これで、**アイテムを使うとエージェントが右にむく**プログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**キーボードの『Tキー』をおして「run」と入力（にゅうりょく）してみましょう**<br>
<img style="width:100%" src="https://i.ibb.co/thjC7gQ/migi.gif"><br>
