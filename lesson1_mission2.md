# LESSON2 エージェントをうごかそう

```block
player.onChat("run", function () {
    agent.move(FORWARD, 3)
    agent.move(RIGHT, 3)
    agent.move(FORWARD, 4)
    agent.move(LEFT, 5)
})
```

```template
player.onChat("run", function () {

})
```

## めあて

**どんなプログラムになるのかな？**<br>
・チャットで「run」と入力したら、エージェントが金ブロックの上に行くようにプログラミングをする<br>
<img style="width:100%" src="https://i.ibb.co/T20WrQ5/root2.png"><br>

## かんがえよう

エージェントがゴールに行くために**どのじゅんばんで、どのむきにうごかせばよいか**をかんがえましょう<br>
<img style="width:100%" src="https://i.ibb.co/R3VsQZq/2024-05-28-163003.png"><br>

## かんがえよう

**前→右→前→左**のじゅんばんでうごかせばよさそうです<br>
つぎは、エージェントがゴールに行くために**何ブロックずつうごかせばよいか**を数えましょう<br>
<img style="width:100%" src="https://i.ibb.co/r4K8pZG/root-direction.png"><br>

## かんがえよう

ゴールまでは**前３ブロック→右３ブロック→前４ブロック→左５ブロック**でした<br>
さっそくつぎのページからプログラムを作っていきましょう<br>
まずは`||agent.エージェントを前に３ブロックうごかす||`プログラムをつくります<br>
<img style="width:100%" src="https://i.ibb.co/7NTCHdP/root-count3345.png"><br>

## プログラミングをしよう

エージェントをうごかすためのプログラムブロックを出します<br>
`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||player.チャットコマンド run を入力した時||`の中にドラッグしましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 1)
})
```

## プログラミングをしよう

エージェントをうごかす数を入力しましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.1||`を`||loops.3||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 3)
})
```

## プログラミングをしよう

エージェントを前に3ブロックうごかすプログラムができました<br>
つぎはエージェントを右に３ブロックうごかしたいですが<br>
プログラムをうごかす→プログラムをひらいて、むきとうごかす数をかえる→プログラムをうごかす→・・・<br>
このくりかえしは時間がかかるし、とてもめんどうです<br>
<img style="width:100%" src="https://i.ibb.co/stzQNn0/loop.png"><br>

## プログラミングをしよう

プログラムは組み合わせることで、いっせいにうごかすことができます！<br>
プログラムを組み合わせてみましょう<br>
<img style="width:100%" src="https://i.ibb.co/m63Zzrz/combi.gif"><br>

## プログラミングをしよう

`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に３ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.右||`にしましょう<br>
`||loops.1||`を`||loops.3||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 3)
    agent.move(RIGHT, 3)
})
```

## プログラミングをしよう

`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを右▼に３ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||loops.1||`を`||loops.４||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 3)
    agent.move(RIGHT, 3)
    agent.move(FORWARD, 4)
})
```

## プログラミングをしよう

`||agent.エージェント||`をクリックして、`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`を`||agent.エージェントを前▼に４ブロック移動（いどう）させる||`の下にドラッグしましょう<br>
`||agent.エージェントを前▼に１ブロック移動（いどう）させる||`の`||loops.前||`を`||loops.左||`にしましょう<br>
`||loops.1||`を`||loops.５||`に入力しましょう<br>
```block
player.onChat("run", function () {
    agent.move(FORWARD, 3)
    agent.move(RIGHT, 3)
    agent.move(FORWARD, 4)
    agent.move(LEFT, 5)
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
