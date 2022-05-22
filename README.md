#Library


## Contact

<theora.vilderson.contact@gmail.com>

### Features

- **use amPM**
- **Change all part color**
- **responsive!**
- **Date Auto sync**
- **can be used with optional Date**
- **Events for Tick and Tock!**

### Default Options :

- **scaleWidth**: ***200***,
- **scaleHeight**: ***200***,
- **fontSize**: ***15***,
- **space**: ***10***,
- **secondPointerSize**: ***2***,
- **minutePointerSize**: ***5***,
- **hourPointerSize**: ***7***,
- **secondPointerStayBack**: ***10***,
- **secondPointerHandsOff**: ***10***,
- **minutePointerHandsOff**: ***20***,
- **hourPointerHandsOff**: ***26***,
- **clockBorderSize**: ***5***,
- **markerDashedWidth**: ***1***,
- **markerMinuteDashedSize**: ***1***,
- **markerHourDashedSize**: ***5***,
- **centralDotSize**: ***5***,
- **textHourSpace**: ***5***,
- **mainBorderColor**: "***grey***",
- **mainBorderCoverColor**: "***white***",
- **centralDotColor**: "***grey***",
- **secondPointerColor**: "***red***",
- **minutePointerColor**: "***black***",
- **hourPointerColor**: "***black***",
- **minDashColor**: "***rgb***(0,0,0)",
- **hourDashColor**: "***rgb***(0,0,0)",
- **hourTextColor**: "***rgb***(0,0,0)",
- **titleColor**: "***rgb***(0,0,0)",
- **title**: "***Theora*** Vilderson",
- **titleFont**: "***sans***-serif",
- **hourFont**: "***monospace***",



### Create Clock Object :
```   
let clock = new Clock({
      element: canvasElm, // the element should be canvas
      onTick:(date)=>{ /* do something*/ },
      onTock:(date)=>{ /* do something*/ },
      time: userDate, //you can use optional Date
      options:{}
    });
    // run it once and the element should be valid !
    // otherwise will be Error shown up

```
### Start/Stop Clock :
```
let clock = new Clock({
      element: canvasRef.current, // the element should be canvas
      onTick:(date)=>{ /* do something*/ },
      onTock:(date)=>{ /* do something*/ },
      time: userDate, //you can use optional Date
      options:{}
    });
    clock.startClock(); // start
    clock.stopClock(); // stop

    //
    // remember in react use  useEffect to create clock 
    // return function and stop the Clock!

```

- **the options for sizing uses Scale Algorithm**
- **YourPixlSize * CurrentSurface / defaultSurface**
- **use your imagine size Handler to just work it out! :)**
