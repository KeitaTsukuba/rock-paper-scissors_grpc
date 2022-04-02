# rock-paper-scissors_grpc.pb
grpcのサンプルとしてジャンケンゲームを作成した

# server側の立ち上げ
```
% go run ./cmd/api
```

# client側の立ち上げ
```
% go run ./cmd/cli 
start Rock-paper-scissors game.
1: play game
2: show match results
3: exit
please enter >
```

# 遊び方
serverとclientを立ち上げる
数字の1,2,3のうち1つ入力する
1はゲームを開始する、2は今までのゲームの履歴を見る、3はゲームを終える

```
1: play game
2: show match results
3: exit
please enter >
```

1を選択すると以下のようにグー、パー、チョキの選択を行う
1,2,3を入力する

```
please enter >1
Please enter Rock, Paper, or Scissors.
1: Rock
2: Paper
3: Scissors
please enter >
```

ゲームの結果が表示される
```
please enter >1
***********************************
Your hand shapes: ROCK 
Opponent hand shapes: SCISSORS 
Result: WIN 
***********************************
```
