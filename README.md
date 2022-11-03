# Command Line Interface Chess Game

This is a project for me to learn programming languages.

## Languages Used

-   JavaScript

---

# **JavsScript**

## Classes :

### Main file

```

```

### Player file

```
-name:str
-white:bool
```

### _Piece_ (abstract)

```
-killed:bool
-white:bool

Piece(isWhite:bool)

+isKilled():bool
+isWhite():bool
+canMove():bool
```

### Spot

```
-piece:Piece
-x:int
-y:int

Spot(x:int, y:int, piece:Piece)

+replacePiece():void
+isEmpty():bool
+getX():int
+getY():int
```

### Board

```
-spot:Spot[][]

Board()

+resetBoard():void
+getSpot(x:int, y:int):Spot
+displayBoard():String
```

### Move

```
-startSpot:Spot
-endSpot:Spot
-player:Player

Move(startSpot:Spot, endSpot:Spot, player:Player)
```

### Game

```
-board:Board
-player:Player
-playerTurn:int

Game()

+makeMove():bool
+nextPlayerTurn():void
+isGameEnd():bool
+isStalemate():bool
```
