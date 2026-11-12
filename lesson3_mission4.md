```block
player.onChat("run", function () {
    agent.move(RIGHT, 4)
    agent.move(UP, 3)
    agent.setItem(GOLD_BLOCK, 1, 1)
    agent.place(RIGHT)
    agent.move(FORWARD, 3)
    agent.move(LEFT, 2)
    agent.move(DOWN, 2)
    agent.move(LEFT, 2)
    agent.setItem(EMERALD_BLOCK, 1, 1)
    agent.place(RIGHT)
    agent.move(LEFT, 2)
    agent.move(FORWARD, 2)
    agent.move(RIGHT, 2)
    agent.move(UP, 3)
    agent.setItem(DIAMOND_BLOCK, 1, 1)
    agent.place(RIGHT)
})
```

```template
player.onChat("run", function () {
	
})
```

# プログラムをつかってみよう

## エクストラステージにチャレンジ！
きょう、学んだプログラムをつかってみましょう<br>
ゴールに行くためにはエージェントをどのようにうごかせばいいでしょうか？<br>
<img style="width:100%" src="https://i.ibb.co/StvcxpT/2024-06-13-135650.png"><br>