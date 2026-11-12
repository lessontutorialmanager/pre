# LESSON1 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.move(DOWN, 13)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントを井戸（いど）のいちばん下までうごかそう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/MnQFxm3/agentdown.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントが井戸（いど）のいちばん下に行くようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/MnQFxm3/agentdown.gif"><br>

## かんがえよう
エージェントを**下に何ブロックうごかせばよいか**をおぼえていますか？<br>
<img style="width:100%" src="https://i.ibb.co/ky3n44L/13q.png"><br>

## かんがえよう
しょうにんが**１３ブロック**とおしえてくれていましたね<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
まずは`||agent.エージェントを前に1ブロックうごかす||`プログラムをつくります<br>
<img style="width:100%" src="https://i.ibb.co/t2vnYY0/2024-06-03-161957.png"><br>

## プログラミングをしよう
エージェントをうごかすためのプログラムブロックを出します<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/rGyz20M/tutorial1.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントを前に1ブロックうごかすプログラムができました<br>
つぎはエージェントを下にうごかすようにプログラムをかえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/Smkcg4r/agentdown1.png"><br>

## プログラミングをしよう
エージェントをうごくむきを下にしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`をクリックして`||loops.下||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/tBJpSNw/downpg.gif"><br>
```block
player.onChat("run", function () {
    agent.move(DOWN, 1)
})
```

## プログラミングをしよう
エージェントをうごかす数を入力しましょう<br>
`||agent.エージェントを下▼に１ブロック移動（いどう）させる||`の`||loops.1||`を`||loops.13||`に入力しましょう<br>
<img style="width:100%" src="https://i.ibb.co/s9dsM5M/downpg13.gif"><br>
```block
player.onChat("run", function () {
    agent.move(DOWN, 13)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう