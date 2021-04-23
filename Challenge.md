```uml
@startuml
start
:wether = 天気情報;
if(wether == 0)then(true)
  :快晴です; 
  stop
elseif(wether == 1) then(true)
  :曇りです;
  stop
elseif(wether == 2) then(true)
  :雨です;
  stop
else (false)
  :不明です;
  stop
@enduml
```
