# Regression_Class
Swiftで簡単に単回帰分析ができるクラス
## インストール
```
git clone git@github.com:JimpeiYamamoto/Regression_Class.git
```
## 使用方法
### 宣言
```swift
var reg = Regression()
let x_lst = [1.0, 2.0, 3.0, 4.0]
let y_lst = [23.0, 44.0, 33.0, 47.4]
```
### 傾きの取得
```swift
let gradient = reg.calc_gradient(x_lst, y_lst)
```
### 切片の取得
```swift
let intercept = reg.calc_intercept(x_lst, y_lst)
```
### 予測
x = 23.0を入れた時のyを計算
```swift
let ans = calc_ans(x_lst, y_lst, 23.0)
```