**RFCode:** long   
**fromDelay:** integer | *   
**toDelay:** integer | *   
**dimStatus:** = float | -= float | += float | ^ float | ¨ float | ~ float   
 - dimStatus is between 0 and 1
 

#### onRFReceive(RFCode, [fromDelay,toDelay]) -> dimStatus++
When RFCode is receive between fromDelay and toDelay, then the dimmer will increase by 1 percentage point.
####
