# アイテムを使ってエージェントをうごかそう
```block
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
    agent.collectAll()
})
```

## アイテムを使ってエージェントをうごかそう
**【鉄のツルハシ】をもって、右クリックするとエージェントが目の前のブロックをこわして、アイテムをひろう**ようにプログラミングをしましょう<br>
<img style="width:100%" src="https://i.ibb.co/qgCqLjm/hirou.gif"><br>


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
**鉄のシャベル**をクリックして、**鉄のツルハシ**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/p443fzL/tut4-2.gif"><br>
```block
mobs.give(
mobs.target(NEAREST_PLAYER),
IRON_PICKAXE,
1
)
```

## アイテムを使ってエージェントをうごかそう
プレイヤーがアイテムをつかったときにうごくプログラムをつくりましょう<br>
`||player.プレイヤー||`の中の`||player.次（つぎ）のアイテムが使（つか）われたとき||`をドラッグして、だしましょう<br>
**鉄のシャベル**をクリックして、**鉄のツルハシ**をえらびます<br>
<img style="width:100%" src="https://i.ibb.co/sJFfcS5/tut4-3.gif"><br>
```block
player.onItemInteracted(IRON_PICKAXE, function () {
	
})
mobs.give(
mobs.target(NEAREST_PLAYER),
IRON_PICKAXE,
1
)
```

## アイテムを使ってエージェントをうごかそう
`||agent.エージェントに前を破壊（はかい）させる||`をドラッグして、`||player.次（つぎ）のアイテムが使（つか）われたとき||`の中にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/JvG2Q4q/tut4-4.gif"><br>
```block
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
})
mobs.give(
mobs.target(NEAREST_PLAYER),
IRON_PICKAXE,
1
)
```

## アイテムを使ってエージェントをうごかそう
`||agent.エージェントに全（すべ）て拾（ひろ）わせる||`をドラッグして、`||agent.エージェントに前を破壊（はかい）させる||`の下にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/qjV25vn/tut4-5.gif"><br>
```block
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
    agent.collectAll()
})
mobs.give(
mobs.target(NEAREST_PLAYER),
IRON_PICKAXE,
1
)

```

## アイテムを使ってエージェントをうごかそう
これで、**アイテムを使うとエージェントがブロックをこわして、アイテムをひろう**プログラムができました<br>
右下の実行（じっこう）ボタンをおして、プログラムを実行（じっこう）したあとに**アイテムを持って右クリック**してプログラムをうごかしてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/qgCqLjm/hirou.gif"><br>
