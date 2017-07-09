# Arduino Latest Version 📥
Ever wonder which is the latest version of Arduino IDE currently released?
<br>Now you can know it, programmatically!

## Get the latest version number
You can know witch is the latest version of arduino available by hitting this URL:

### curl
```bash
$ curl https://cdn.rawgit.com/arduino-cli/arduino-latest/master/VERSION
```

### node

```javascript
const request = require('request');
const latest_endpoint = 'https://cdn.rawgit.com/arduino-cli/arduino-latest/master/VERSION';

request(latest_endpoint, function (error, response, body) {
   if (!error && response.statusCode == 200) {
       console.log(body) // Shows the version on the console.
   }
});
```

## Arduino mirrors

OS | Arch | URI
---|------|----
win32 | x64 | [https://downloads.arduino.cc/arduino-`VERSION`-windows.zip](https://www.arduino.cc/en/Main/Software)
darwin | x64 | [https://downloads.arduino.cc/arduino-`VERSION`-macosx.zip](https://www.arduino.cc/en/Main/Software)
linux | x32 | [https://downloads.arduino.cc/arduino-`VERSION`-linux32.tar.xz](https://www.arduino.cc/en/Main/Software)
linux | x64 | [https://downloads.arduino.cc/arduino-`VERSION`-linux64.tar.xz](https://www.arduino.cc/en/Main/Software)
linux | arm | [https://downloads.arduino.cc/arduino-`VERSION`-linuxarm.tar.xz](https://www.arduino.cc/en/Main/Software)

## Arduino download page
The latest version available can be verified [here](https://www.arduino.cc/en/Main/Software).