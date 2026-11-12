# LESSON1 エージェントにブロックをこわせよう
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
})
```

```template
player.onChat("run", function () {
	
})
```

## エージェントをプログラミングでうごかしてみよう @unplugged
エージェントをうごかして、ブロックをこわせよう<br>
<img style="display: block; margin: auto;" height="50%" width="90%" src="https://i.ibb.co/VtTkqMY/quiz1.gif">

## めあて
**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントがうごいて、ブロックをこわすようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/VtTkqMY/quiz1.gif"><br>

## かんがえよう
まずはエージェントを**どのようにうごかせばよいか**をかんがえてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/tQTBpr0/2024-07-03-221815.png"><br>

## かんがえよう
**ブロックをこわす⇒前に１ブロックうごく⇒ブロックをこわす**ようにプログラミングをしましょう<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
<img style="width:100%" src="https://i.ibb.co/Nsqsf4v/1.png"><br>

## プログラミングをしよう
エージェントがブロックをこわすプログラムをつくりましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
<img style="width:100%" src="https://i.ibb.co/d6z32sG/tut1.gif"><br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
})
```

## プログラミングをしよう
エージェントをうごかすプログラムをつくりましょう<br>
`||agent.エージェントを前に1ブロック移動（いどう）させる||`を`||agent.エージェントの前を破壊（はかい）させる||`の下にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/GkX9Cxf/quiz1-2.gif"><br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう
もう一つのブロックをエージェントにこわさせましょう<br>
`||agent.エージェントの前を破壊（はかい）させる||`を`||agent.エージェントを前に1ブロック移動（いどう）させる||`の下にいれましょう<br>
<img style="width:100%" src="https://i.ibb.co/V9f9n1f/quiz1-3.gif"><br>
```block
player.onChat("run", function () {
    agent.destroy(FORWARD)
    agent.move(FORWARD, 1)
    agent.destroy(FORWARD)
})
```

## プログラムをうごかしてみよう
がめんの右下にあるみどり色の『▶』ボタンをクリックして、チャットコマンドで`||player.run||`と入力してみましょう