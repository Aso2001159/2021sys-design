```uml
@startuml
start
:wether = 天気情報;
if(wether == 0)
:快晴です; 
elseif(wether == 1)
:曇りです;
elseif(wether == 2)
:雨です;
else
:不明です;
stop
@enduml
```
