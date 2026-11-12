# LESSON2 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.move(UP, 8)
})
```

```template
player.onChat("run", function () {
	
})
```

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、上にある赤いくだものに行くようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/r0ftBxg/agentup.gif"><br>

## かんがえよう
エージェントを**上に何ブロックうごかせばよいか**をおぼえていますか？<br>
<img style="width:100%" src="https://i.ibb.co/3SPTcD0/8q.png"><br>

## かんがえよう
しょうにんが**８ブロック**とおしえてくれていましたね<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
まずは`||agent.エージェントを前に1ブロックうごかす||`プログラムをつくります<br>
<img style="width:100%" src="https://i.ibb.co/JptVN0T/2024-06-03-162044.png"><br>

## プログラミングをしよう
エージェントをうごかすためのプログラムブロックを出します<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントをうごくむきを上にしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`をクリックして`||loops.上||`にしましょう<br>
```block
player.onChat("run", function () {
    agent.move(UP, 1)
})
```

## プログラミングをしよう
エージェントをうごかす数を入力しましょう<br>
`||agent.エージェントを上▼に１ブロック移動（いどう）させる||`の`||loops.1||`を`||loops.8||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(UP, 8)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう