# KopoBlockChain

## Index
#### 1. [Project Introduction](#project-introduction)
#### 2. [Execution method](#execution-method)
#### 3. [Function](#function)
#### 4. Diagram
___
[Project Introduction]
- Block and transaction data generation
- Learning Blockchain Principles through Block Mining
___
[Execution method]
1. Server running(ip, port)
2. After changing the bottom url ip and port,
   make a request to the server
3. Response from server
___
[Function]
- getBlockData
Get block data (blockchain.csv) information

```
GET 'http://ip:port/block/getBlockData'
```

- generateBlock
Create block and add blockchain.csv (create blockchain.csv on first run)

```
GET 'http://ip:port/block/generateBlock'
```

- newtx
Create new transaction data (create txData.csv on first run)

```
POST 'http://ip:port/block/newtx'
```

- validateBlock
Comparison of my socket server block and the requested counterpart server block (validation check)

```
POST 'http://ip:port/block/validateBlock'
```

- addNode
Add server ip, port to be linked during broadcasting (create nodelst.csv on first run)

```
GET 'http://ip:port/node/addNode?ip:port'
```
___
[Diagram]
