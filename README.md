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
##ระบบตัดเงินอัตโนมัติ
```
@startuml
database -> bank : senttotalcharges
bank -> banksystem : checkmoneyfromaccount
banksystem -> User : SentSMSDon'tHasMoney
bank <- banksystem : cutmoneyfromaccount
banksystem -> User : SentSMS
@enduml
```
<img src = "https://github.com/Hathaichanok241/OOAD-WEEK10/blob/master/Homework/10.3.png?raw=true">

##LoginWebsite
```@startuml
user -> LoginPage : InsertNameAndPass
LoginPage -> WebDatabase : CheckNameandPass
WebDatabase -> user : SHowIncorrect

 
@enduml

```
<img src ="https://github.com/Hathaichanok241/OOAD-WEEK10/blob/master/Homework/10.4.png?raw=true">

##เครื่องขายตั๋วรถไฟ
```@startuml
User -> TicketMachine : ChooseStation
TicketMachine -> Display : Showcost
User -> TicketMachine : InsertMoney 
TicketMachine -> TicketMachine : checkMoney 
TicketMachine -> User : printTicket
@enduml

```
<img src ="https://github.com/Hathaichanok241/OOAD-WEEK10/blob/master/Homework/10.5.png?raw=true">
