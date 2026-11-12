```block
player.onItemInteracted(CARROT_ON_A_STICK, function () {
    agent.setItem(GOLD_BLOCK, 6, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
})
player.onItemInteracted(STICK, function () {
    agent.setItem(GOLD_BLOCK, 3, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.turn(RIGHT_TURN)
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
<img style="width:100%" src="https://i.ibb.co/cbvyX7Y/2024-07-26-140812.png"><br>