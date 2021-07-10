---
title: "Golang 関数"
emoji: "🐙"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["Go"]
published: true
---

# 関数定義

## 構文
```go
func name(parameters) (results) {
    body-content
}
```
## 例
```go
package main

func sum(x int, y int) int {
    return x + y
}

func main(){
    sum := sum(2, 3)
    println("Sum:", sum)
}
```
実行結果
```zsh
$ go run main.go
$ 5
```

## 関数の戻り値に名前をつける

```go
func sum(x int, y int)(result int) {
   result = x + y
   return
}

```

## 複数の値を返す
```go
func calc(x int, y int)(sum int, mul int) {
   result = x + y
   mul = x * y
   return
}
```

## ポインター渡し

```go
package main

func main() {
    foo := 5
    update(&foo)
    println(foo)
}

func update(value *int) {
    *value = "10"
}
```
実行結果
```zsh
$ go run main.go
$ 10
```
