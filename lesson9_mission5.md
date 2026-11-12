```block
player.onChat("run", function () {
    agent.setItem(GOLD_BLOCK, 5, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(LEFT, 1)
    agent.place(DOWN)
    agent.move(LEFT, 1)
    agent.place(DOWN)
    agent.setItem(EMERALD_BLOCK, 6, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(RIGHT, 1)
    agent.place(DOWN)
    agent.move(RIGHT, 1)
    agent.place(DOWN)
    agent.move(RIGHT, 1)
    agent.place(DOWN)
    agent.setItem(DIAMOND_BLOCK, 4, 1)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
    agent.move(FORWARD, 1)
    agent.place(DOWN)
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
<img style="width:100%" src="https://i.ibb.co/PWfHr9k/2024-07-23-163506.png"><br>