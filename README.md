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
##เครื่องเก็บค่าทางด่วนอัตโนมัติ
``` @startuml
user -> MachineCheckIDCar : StartUseTollway
user -> MachineCheckIDCar : EndUsetollway
MachineCheckIDCar -> database : Distance Calculator
database -> MachineCheckIDCar : senttotalcharges
Display <- MachineCheckIDCar : totalcharges
Display -> user : showtotalcharges
database -> cuttingFundSystem : cuttingfund

@enduml

```
<img src = "https://github.com/Hathaichanok241/OOAD-WEEK10/blob/master/Homework/10.2.png?raw=true">
