# アイテムを使ってエージェントをうごかそう
```block
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
```


## アイテムを使ってエージェントをうごかそう
**【棒】をもって、右クリックするとエージェントが左をむく**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/LpmjR3d/hidari.gif"><br>


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
**鉄のシャベル**をクリックして、**棒**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/Q6N2HhL/tut2-2.gif"><br>
```block
mobs.give(
mobs.target(NEAREST_PLAYER),
STICK,
1
)
```

## アイテムを使ってエージェントをうごかそう
プレイヤーがアイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.プレイヤー||`の中の`||player.次（つぎ）のアイテムが使（つか）われたとき||`をドラッグして、だしましょう<br>
**鉄のシャベル**をクリックして、**棒**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/xzMs0sy/tut2-3.gif"><br>
```block
player.onItemInteracted(STICK, function () {
	
})
mobs.give(
mobs.target(NEAREST_PLAYER),
STICK,
1
)
```

## アイテムを使ってエージェントをうごかそう
`||agent.エージェントの向（む）きを左に変（か）える||`をドラッグして、`||player.次（つぎ）のアイテムが使（つか）われたとき||`の中にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/3cNfY7g/tut2-4.gif"><br>
```block
player.onItemInteracted(STICK, function () {
    agent.turn(LEFT_TURN)
})
mobs.give(
mobs.target(NEAREST_PLAYER),
STICK,
1
)
```

## アイテムを使ってエージェントをうごかそう
これで、**アイテムを使うとエージェントが左にむく**プログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**アイテムを持って右クリック**してプログラムをうごかしてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/LpmjR3d/hidari.gif"><br>
