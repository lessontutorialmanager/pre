# LESSON1 エージェントをうごかしてスイッチをおさせよう
```block
player.onChat("run", function () {
    agent.move(FORWARD, 6)
    agent.interact(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントをスイッチの前にうごかして、スイッチをおさせよう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/SJgvfJx/quiz1.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがスイッチの前にうごいて、スイッチをおすようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/SJgvfJx/quiz1.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/PMSL4x3/2024-07-02-213431.png"><br>

## かんがえよう
**前に６ブロックうごく⇒スイッチをおす**ようにプログラミングをしましょう<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/SJyXjYS/1.png"><br>

## プログラミングをしよう
エージェントをうごかすプログラムをつくりましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/ZYgxhHk/quiz1pg1.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
エージェントをうごかす数をいれましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`の`||loops.１ブロック||`を`||loops.6ブロック||`にしましょう<br>
<img style="width:100%" src="https://i.ibb.co/9vcbNP1/quiz1pg2.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 6)
})
```

## プログラミングをしよう
エージェントにスイッチをおさせましょう<br>
`||agent.エージェントを前に向けてインタラクトさせる||`を`||agent.エージェントを前に６ブロック移動（いどう）させる||`の下にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/mXX7MBm/quiz1pg3.gif"><br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 6)
    agent.interact(FORWARD)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう