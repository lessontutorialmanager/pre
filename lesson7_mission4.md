```block
player.onItemInteracted(BLAZE_ROD, function () {
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(IRON_PICKAXE, function () {
    agent.destroy(FORWARD)
    agent.collectAll()
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

# プログラムをつかってみよう

## エクストラステージにチャレンジ！
きょう、学んだプログラムをつかってみましょう<br>
エージェントをどのようにうごかせばいいでしょうか？<br>
<img style="width:100%" src="hhttps://i.ibb.co/6vSMpB8/2024-07-10-223506.png"><br>