### Operators
**value -= number**   
Decreases value with number. If value has a lower limit and it has been reached, value = the lower limit   
**value += number**   
Increases value with number. If value has a upper limit and it has been reached, value = the upper limit   
**value ^ number**   
as +=, but if the upper limit of value has been reached, the increment will restart from the lower limit.    
Ex. value = 80, lower limit = 0 and upper limit = 100   
value ^ 10 -> value = 90   
value ^ 10 -> value = 100   
value ^ 10 -> value = 10   
value ^ 10 -> value = 20   
**value ¨ number**   
as ^, but as a decrement instad of an increment   
**value ~ number**   
Only works for certain variables. For example dimStatus. When lower limit or upper limit is reached, dimUp will be inversed.   
Ex. dimStatus = 0.8, lower limit = 0, upper limit = 1   
dimStatus ~ 0.1 -> dimStatus = 0.9, dimUp = true   
dimStatus ~ 0.1 -> dimStatus = 1.0, dimUp = true   
dimStatus ~ 0.1 -> dimStatus = 0.9, dimUp = false    
dimStatus ~ 0.1 -> dimStatus = 0.8, dimUp = false   

### Variables
**RFCode:** long   
**fromDelay:** integer | *   
**toDelay:** integer | *   
**dimStatus:** = float | -= float | += float | ^ float | ¨ float | ~ float   
 - dimStatus is between 0 and 1
 
### Functions
#### onRFReceive(RFCode, [fromDelay:toDelay]) -> dimStatus+=0.01
When RFCode is receive between fromDelay and toDelay, then the dimmer will increase by 1 percentage point.

**onRFReceive(123456789, [100:200]) -> dimStatus+=0.01**   
When the RFCode 123456789 is received and the last time an RFCode received is between 100 and 200 milliseconds, then increase the luminosity by 1 percentage point.
