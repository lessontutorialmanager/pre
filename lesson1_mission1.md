# LESSON1 エージェントをうごかそう
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントを金ブロックまでうごかそう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/J389kJS/agent-forward5.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントが金ブロックの上に行くようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/J389kJS/agent-forward5.gif"><br>

## かんがえよう
エージェントがゴールに行くために**前に何ブロックうごかせばよいか**を数えましょう<br>
<img style="width:100%" src="https://i.ibb.co/8mdJyTQ/2024-05-28-160937.png"><br>

## かんがえよう
ゴールまでは**５ブロック**でした<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
まずは`||agent.エージェントを前に1ブロックうごかす||`プログラムをつくります<br>
<img style="width:100%" src="https://i.ibb.co/y66JFvD/count5.png"><br>

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
つぎは５ブロックうごかすようにプログラムをかえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/J389kJS/agent-forward5.gif"><br>

## プログラミングをしよう
エージェントをうごかす数を入力しましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.1||`を`||loops.5||`に入力しましょう<br>
<img style="width:100%" src="https://i.ibb.co/nc9xGWq/tutorial2.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 5)
})
```

## プログラミングをしよう
**プログラミングをまちがえたときは？**<br>
もしも、エージェントをゴールにうごかせなかったときは、たいちょうに話して**はい**をクリックしましょう<br>
エージェントをスタートにもどしてくれます<br>
<img style="width:100%" src="https://i.ibb.co/4gxpyST/reset.png"><br>

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう
<img style="width:100%" src="https://i.ibb.co/bW6bphv/tutorialpractice1.gif"><br>
