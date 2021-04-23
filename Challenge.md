```uml
@startuml
start
:wether = 天気情報;
if(wether == 0)
:快晴です; 
stop
elseif(wether == 1)
:曇りです;
stop
elseif(wether == 2)
:雨です;
stop
else
:不明です;
stop
@enduml
```
