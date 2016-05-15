# DateTimeConversion v 1.0

* #### First of all let's discuss the functionality of DateTimeConversion

  - Get Local DateTime 
  - Get UTC DateTime
  - Convert Local DateTime to UTC DateTime and Vice versa   

* #### How to use ?
      
  - Get Local DateTime :
    - `Generic.getCurrentLocalTime()` to get Current LocalTime . It will return string .
  - Get UTC DateTime  :
    - `Generic.getCurrentUTCTime()` to get Current UTCTime . It will return string .
  - Convert Local to UTC :
    - `LocalToUTC.convertLocalToUTC(new SimpleDateFormat("MM/dd/yyyy KK:mm:ss a Z"),Generic.getCurrentLocalTime())` 
    - There are two arguments where in first argument you should specify SimpleDateFormat and in second argument a string which represent Local DateTime in same SimpleDateFormat as of first argument . Please note both the argument should have same date format.
  - Convert UTC to Local :
    - `UTCToLocal.convertUTCToLocal(new SimpleDateFormat("MM/dd/yyyy KK:mm:ss a Z"),Generic.getCurrentUTCTime())`
    - There are two arguments where in first argument you should specify SimpleDateFormat and in second argument a string which represent UTC DateTime in same SimpleDateFormat as of first argument . Please note both the argument should have same date format.
    
* ### Installation

  - Download the jar file and add it your your project . Right click on your project -> Build Path -> Add External Archives -> select the jar file .
    
* ### Instructions

  - This jar will perfectly work if the code is locally hosted . If hosted on server `getCurrentLocalTime` and `getCurrentUTCTime` will give the results accoring to the server geolocation . Suppose you are in INDIA and you have hosted code on a server which reside in America so these two functions will return you the DateTime accordingly .
  - The other two functions will perfectly work fine even on server depending on what argument you pass . If you want to pass client current DateTime and not server and suppose you are using JavaScript then you can use JavaScript Date function to  get clients current DateTime .
  
