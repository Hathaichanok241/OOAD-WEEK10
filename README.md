# OOAD-WEEK10
Sequence Diagram

##เครื่องซักผ้าหยอดเหรียญ
```
@startuml
user -> CoinCounting : InsertCoin()
CoinCounting ->user : returncoin()
CoinCounting -> WashingMachine : Start()
WashingMachine -> user : ShowTime
@enduml 

```
<img src = "https://github.com/Hathaichanok241/OOAD-WEEK10/blob/master/Homework/10.1.png?raw=true">
