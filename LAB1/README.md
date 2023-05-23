

### Системы аутентификации и защиты от несанкционированного доступа

Лабораторная работа №1

### Цель

Вывести информацию о системе

### Исходные данные

1.  ОС Windows 11
2.  RStudio Desktop
3.  Интерпретатор языка R 4.3.0

### План

1.  Вывести информации о системе
2.  Вывести информацию о процессоре
3.  Вывести последние 30 логов

### Шаги

1\. Выполнение команды system2("systeminfo", stdout = TRUE) для вывода информации о системе

```{r}
system2("systeminfo", stdout = TRUE)
```

    [1] ""                                                                                                                                                                                    
    [2] "\x88\xac\xef 㧫\xa0:                         DESKTOP-LOUQV3Q"                                                                                                                        
    [3] "\x8d\xa0\xa7\xa2\xa0\xad\xa8\xa5 \x8e\x91:                      \x8c\xa0\xa9\xaa\xe0\xae\xe1\xae\xe4\xe2 Windows 11 \x84\xae\xac\xa0\xe8\xad\xef\xef"                                
    [4] "\x82\xa5\xe0\xe1\xa8\xef \x8e\x91:                        10.0.22621 \x8d/\x84 \xaf\xae\xe1\xe2\u0ba5\xad\xa8\xa5 22621"                                                             
    [5] "\x88\xa7\xa3\xae⮢\xa8⥫\xec \x8e\x91:                  Microsoft Corporation"                                                                                                         
    [6] "\x8f\xa0ࠬ\xa5\xe2\xe0\xeb \x8e\x91:                     \x88\xa7\xae\xab\xa8\u0ba2\xa0\xad\xad\xa0\xef ࠡ\xae\xe7\xa0\xef \xe1⠭\xe6\xa8\xef"                                            
    [7] "\x91\xa1\xaeઠ \x8e\x91:                        Multiprocessor Free"                                                                                                                  
    [8] "\x87\xa0ॣ\xa8\xe1\xe2\xe0\xa8\u0ba2\xa0\xad\xad\xeb\xa9 \xa2\xab\xa0\xa4\xa5\xab\xa5\xe6:      grenkova.a.n@yandex.ru"                                                                
    [9] "\x87\xa0ॣ\xa8\xe1\xe2\xe0\xa8\u0ba2\xa0\xad\xad\xa0\xef \xae࣠\xad\xa8\xa7\xa0\xe6\xa8\xef:   "                                                                                         
    [10] "\x8a\xae\xa4 \xafத\xe3\xaa\xe2\xa0:                     00326-10000-00000-AA629"                                                                                                     
    [11] "\x84\xa0\xe2\xa0 \xe3\xe1⠭\xae\xa2\xaa\xa8:                   10.02.2023, 21:16:22"                                                                                                  
    [12] "\x82६\xef \xa7\xa0\xa3\xe0㧪\xa8 \xe1\xa8\xe1⥬\xeb:           19.05.2023, 22:41:17"                                                                                                  
    [13] "\x88\xa7\xa3\xae⮢\xa8⥫\xec \xe1\xa8\xe1⥬\xeb:             LENOVO"                                                                                                                    
    [14] "\x8c\xae\xa4\xa5\xab\xec \xe1\xa8\xe1⥬\xeb:                   81YQ"                                                                                                                  
    [15] "\x92\xa8\xaf \xe1\xa8\xe1⥬\xeb:                      x64-based PC"                                                                                                                   
    [16] "\x8f\xe0\xae\xe6\xa5\xe1\xe1\xae\xe0(\xeb):                     \x97\xa8\u1aee \xaf\xe0\xae\xe6\xa5\xe1\xe1\xae\u0ba2 - 1."                                                          
    [17] "                                  [01]: AMD64 Family 23 Model 96 Stepping 1 AuthenticAMD ~2000 \x8c\x83\xe6"                                                                         
    [18] "\x82\xa5\xe0\xe1\xa8\xef BIOS:                      LENOVO E7CN45WW, 28.04.2022"                                                                                                     
    [19] "\x8f\xa0\xaf\xaa\xa0 Windows:                    C:\\WINDOWS"                                                                                                                        
    [20] "\x91\xa8\xe1⥬\xad\xa0\xef \xaf\xa0\xaf\xaa\xa0:                  C:\\WINDOWS\\system32"                                                                                              
    [21] "\x93\xe1\xe2ன\xe1⢮ \xa7\xa0\xa3\xe0㧪\xa8:              \\Device\\HarddiskVolume1"                                                                                                   
    [22] "\x9f\xa7\xeb\xaa \xe1\xa8\xe1⥬\xeb:                     ru;\x90\xe3\xe1᪨\xa9"                                                                                                        
    [23] "\x9f\xa7\xeb\xaa \xa2\xa2\xae\xa4\xa0:                       ru;\x90\xe3\xe1᪨\xa9"                                                                                                   
    [24] "\x97\xa0ᮢ\xae\xa9 \xaf\xae\xef\xe1:                     (UTC+03:00) \x8c\xae᪢\xa0, \x91\xa0\xad\xaa\xe2-\x8f\xa5\xe2\xa5\xe0\xa1\xe3\xe0\xa3"                                         
    [25] "\x8f\xae\xab\xad\xeb\xa9 \xae\xa1ꥬ 䨧\xa8\xe7\xa5\u1aae\xa9 \xaf\xa0\xac\xef\xe2\xa8:   15\xff735 \x8c\x81"                                                                         
    [26] "\x84\xae\xe1\xe2㯭\xa0\xef 䨧\xa8\xe7\xa5᪠\xef \xaf\xa0\xac\xef\xe2\xec:      7\xff650 \x8c\x81"                                                                                     
    [27] "\x82\xa8\xe0\xe2㠫쭠\xef \xaf\xa0\xac\xef\xe2\xec: \x8c\xa0\xaa\xe1. ࠧ\xac\xa5\xe0: 16\xff759 \x8c\x81"                                                                               
    [28] "\x82\xa8\xe0\xe2㠫쭠\xef \xaf\xa0\xac\xef\xe2\xec: \x84\xae\xe1\xe2㯭\xa0:     6\xff230 \x8c\x81"                                                                                    
    [29] "\x82\xa8\xe0\xe2㠫쭠\xef \xaf\xa0\xac\xef\xe2\xec: \x88ᯮ\xab\xec\xa7\xe3\xa5\xe2\xe1\xef: 10\xff529 \x8c\x81"                                                                        
    [30] "\x90\xa0ᯮ\xab\xae\xa6\xa5\xad\xa8\xa5 䠩\xab\xa0 \xaf\xae\xa4\xaa\xa0窨:      C:\\pagefile.sys"                                                                                      
    [31] "\x84\xae\xac\xa5\xad:                            WORKGROUP"                                                                                                                          
    [32] "\x91\xa5ࢥ\xe0 \xa2室\xa0 \xa2 \xe1\xa5\xe2\xec:              \\\\DESKTOP-LOUQV3Q"                                                                                                    
    [33] "\x88\xe1\xafࠢ\xab\xa5\xad\xa8\xa5(\xef):                   \x97\xa8\u1aee \xe3\xe1⠭\xae\xa2\xab\xa5\xad\xad\xeb\xe5 \xa8\xe1\xafࠢ\xab\xa5\xad\xa8\xa9 - 4."                            
    [34] "                                  [01]: KB5022497"                                                                                                                                   
    [35] "                                  [02]: KB5012170"                                                                                                                                   
    [36] "                                  [03]: KB5026372"                                                                                                                                   
    [37] "                                  [04]: KB5025351"                                                                                                                                   
    [38] "\x91\xa5⥢\xeb\xa5 \xa0\xa4\xa0\xaf\xe2\xa5\xe0\xeb:                 \x97\xa8\u1aee \xe1\xa5⥢\xeb\xe5 \xa0\xa4\xa0\xaf\xe2\xa5\u0ba2 - 5."                                            
    [39] "                                  [01]: Intel(R) Wi-Fi 6 AX200 160MHz"                                                                                                               
    [40] "                                        \x88\xac\xef \xaf\xae\xa4\xaa\xab\xee祭\xa8\xef: \x81\xa5\xe1\xaf\u0ba2\xae\xa4\xad\xa0\xef \xe1\xa5\xe2\xec"                                
    [41] "                                        DHCP \xa2\xaa\xab\xee祭:    \x84\xa0"                                                                                                        
    [42] "                                        DHCP-\xe1\xa5ࢥ\xe0:     192.168.0.1"                                                                                                         
    [43] "                                        IP-\xa0\xa4\xe0\xa5\xe1"                                                                                                                     
    [44] "                                        [01]: 192.168.0.24"                                                                                                                          
    [45] "                                        [02]: fe80::8ec6:86bb:30a6:4c18"                                                                                                             
    [46] "                                  [02]: Bluetooth Device (Personal Area Network)"                                                                                                    
    [47] "                                        \x88\xac\xef \xaf\xae\xa4\xaa\xab\xee祭\xa8\xef: \x91\xa5⥢\xae\xa5 \xaf\xae\xa4\xaa\xab\xee祭\xa8\xa5 Bluetooth"                             
    [48] "                                        \x91\xae\xe1\xe2\xaeﭨ\xa5:       \x8d\xae\xe1\xa8⥫\xec \xae⪫\xee祭"                                                                          
    [49] "                                  [03]: VirtualBox Host-Only Ethernet Adapter"                                                                                                       
    [50] "                                        \x88\xac\xef \xaf\xae\xa4\xaa\xab\xee祭\xa8\xef: Ethernet 2"                                                                                 
    [51] "                                        DHCP \xa2\xaa\xab\xee祭:    \x8d\xa5\xe2"                                                                                                    
    [52] "                                        IP-\xa0\xa4\xe0\xa5\xe1"                                                                                                                     
    [53] "                                        [01]: 192.168.56.1"                                                                                                                          
    [54] "                                        [02]: fe80::3e33:4450:85f4:d92f"                                                                                                             
    [55] "                                  [04]: VMware Virtual Ethernet Adapter for VMnet1"                                                                                                  
    [56] "                                        \x88\xac\xef \xaf\xae\xa4\xaa\xab\xee祭\xa8\xef: VMware Network Adapter VMnet1"                                                              
    [57] "                                        DHCP \xa2\xaa\xab\xee祭:    \x84\xa0"                                                                                                        
    [58] "                                        DHCP-\xe1\xa5ࢥ\xe0:     192.168.189.254"                                                                                                     
    [59] "                                        IP-\xa0\xa4\xe0\xa5\xe1"                                                                                                                     
    [60] "                                        [01]: 192.168.189.1"                                                                                                                         
    [61] "                                        [02]: fe80::c14a:79a0:d051:45bd"                                                                                                             
    [62] "                                  [05]: VMware Virtual Ethernet Adapter for VMnet8"                                                                                                  
    [63] "                                        \x88\xac\xef \xaf\xae\xa4\xaa\xab\xee祭\xa8\xef: VMware Network Adapter VMnet8"                                                              
    [64] "                                        DHCP \xa2\xaa\xab\xee祭:    \x84\xa0"                                                                                                        
    [65] "                                        DHCP-\xe1\xa5ࢥ\xe0:     192.168.183.254"                                                                                                     
    [66] "                                        IP-\xa0\xa4\xe0\xa5\xe1"                                                                                                                     
    [67] "                                        [01]: 192.168.183.1"                                                                                                                         
    [68] "                                        [02]: fe80::acd8:abda:b483:e735"                                                                                                             
    [69] "\x92ॡ\xae\xa2\xa0\xad\xa8\xef Hyper-V:               \x90\xa0\xe1\xe8\xa8७\xa8\xef ०\xa8\xac\xa0 \xac\xae\xad\xa8\xe2\xaeਭ\xa3\xa0 \xa2\xa8\xe0\xe2㠫쭮\xa9 \xac\xa0設\xeb: \x84\xa0"
    [70] "                                  \x82\xa8\xe0\xe2㠫\xa8\xa7\xa0\xe6\xa8\xef \xa2\xaa\xab\xee祭\xa0 \xa2\xae \xa2\xe1\xe2\u0ba5\xad\xad\xae\xac \x8f\x8e: \x84\xa0"                  
    [71] "                                  \x8f८\xa1ࠧ\xae\xa2\xa0\xad\xa8\xa5 \xa0\xa4\xe0\xa5ᮢ \xa2\xe2\xaeண\xae \xe3\u0ba2\xad\xef: \x84\xa0"                                                 
    [72] "                                  \x84\xae\xe1\xe2㯭\xae \xaf।\xae\xe2\xa2\xe0\xa0饭\xa8\xa5 \xa2믮\xab\xad\xa5\xad\xa8\xef \xa4\xa0\xad\xad\xeb\xe5: \x84\xa0" 

2\. Выполнение команды system("wmic cpu get name") для вывода информации о процессоре

```{r}
system2("cmd", args = c("/c", "wmic cpu get name"), stdout = TRUE)
```
    [1] "Name                                    \r"
    [2] "AMD Ryzen 7 4700U with Radeon Graphics  \r"
    [3] "\r"

3\. Выполнение команды system("powershell.exe Get-EventLog -LogName System -Newest 30") для вывода логов

```{r}
system2("powershell.exe", args = c("Get-EventLog", "-LogName", "System", "-Newest", "30"), stdout = TRUE)
```
    [1] ""                                                                                                                                                                                                                        
    [2] "   Index Time          EntryType   Source                 InstanceID Message                                           "                                                                                                 
    [3] "   ----- ----          ---------   ------                 ---------- -------                                           "                                                                                                 
    [4] "   10603 \xac\xa0\xa9 23 23:09  Warning     Microsoft-Windows...         1014 \x90\xa0\xa7\xe0\xa5襭\xa8\xa5 \xa8\xac\xa5\xad \xa4\xab\xef \xa8\xac\xa5\xad\xa8 portal.mail.ru \xa8\xe1⥪\xab..."                         
    [5] "   10602 \xac\xa0\xa9 23 22:19  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [6] "   10601 \xac\xa0\xa9 23 22:15  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [7] "   10600 \xac\xa0\xa9 23 21:26  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [8] "   10599 \xac\xa0\xa9 23 21:18  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [9] "   10598 \xac\xa0\xa9 23 20:27  Error       DCOM                        10010 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '10010'..."           
    [10] "   10597 \xac\xa0\xa9 23 20:25  Warning     DCOM                        10016 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '10016'..."           
    [11] "   10596 \xac\xa0\xa9 23 20:25  Warning     DCOM                        10016 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '10016'..."           
    [12] "   10595 \xac\xa0\xa9 23 20:25  Warning     DCOM                        10016 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '10016'..."           
    [13] "   10594 \xac\xa0\xa9 23 20:25  Warning     DCOM                        10016 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '10016'..."           
    [14] "   10593 \xac\xa0\xa9 23 20:25  Information BTHUSB                 1074069522 \x91\xa8\xe1⥬\xa0 Windows \xad\xa5 \xac\xae\xa6\xa5\xe2 \xe1\xae\xe5࠭\xa8\xe2\xec \xaa\xae\xa4\xeb \xaf\u0ba2\xa5\xe0\xaa..."               
    [15] "   10592 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...         7001 \x93\xa2\xa5\xa4\xae\xac\xab\xa5\xad\xa8\xa5 \xae \xa2室\xa5 \xaf\xae\xab짮\xa2\xa0⥫\xef \xa4\xab\xef \xafணࠬ\xac\xeb ..."                   
    [16] "   10591 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...            1 \x91\xa8\xe1⥬\xa0 \xa2\xeb諠 \xa8\xa7 \xe1\xae\xe1\xe2\xaeﭨ\xef \xaf\xae\xad\xa8\xa6\xa5\xad\xad\xae\xa3\xae \xed\xad\xa5࣮\xaf\xae..."      
    [17] "   10590 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [18] "   10589 \xac\xa0\xa9 23 20:25  Information Netwtw10               1073748845 7021 - Connection telemetry fields and analysis..."                                                                                        
    [19] "   10588 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [20] "   10587 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...           32 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '32' \xa2 ..."        
    [21] "   10586 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...           18 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '18' \xa2 ..."        
    [22] "   10585 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...           30 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '30' \xa2 ..."        
    [23] "   10584 \xac\xa0\xa9 23 20:25  Information Netwtw10               1073748849 7025 - Dump after return from D3 before cmd       "                                                                                        
    [24] "   10583 \xac\xa0\xa9 23 20:25  Information Microsoft-Windows...            1 \x82\xae\xa7\xac\xae\xa6\xad\xae\xa5 \xae\xa1\xad\xa0\xe0㦥\xad\xa8\xa5 CVE: 2023-05-23T17:25:17...."                                      
    [25] "   10582 \xac\xa0\xa9 23 19:30  Information Microsoft-Windows...          107 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '107' \xa2..."        
    [26] "   10581 \xac\xa0\xa9 23 19:30  Information Microsoft-Windows...           42 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '42' \xa2 ..."        
    [27] "   10580 \xac\xa0\xa9 23 19:30  Information Microsoft-Windows...          566 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '566' \xa2..."        
    [28] "   10579 \xac\xa0\xa9 23 19:30  Information Microsoft-Windows...          187 \x8d\xa5 \xad\xa0\xa9\xa4\xa5\xad\xae \xae\xaf\xa8ᠭ\xa8\xa5 \xa4\xab\xef ᮡ\xeb\xe2\xa8\xef \xe1 \xaa\xae\xa4\xae\xac '187' \xa2..."        
    [29] "   10578 \xac\xa0\xa9 23 19:30  Information Win32k                 1073742091 \x8f\u0ba2\xa5ઠ \xaa\xa0\xe7\xa5\xe1⢠ \xae\xa1\xae\xe0㤮\xa2\xa0\xad\xa8\xef \xe1 \xa2\xae\xa7\xac\xae\xa6\xad\xae\xe1\xe2\xec\xee \xe1..."
    [30] "   10577 \xac\xa0\xa9 23 19:30  Information Microsoft-Windows...         7002 \x93\xa2\xa5\xa4\xae\xac\xab\xa5\xad\xa8\xa5 \xae \xa2\xeb室\xa5 \xaf\xae\xab짮\xa2\xa0⥫\xef \xa4\xab\xef \xafணࠬ\xac\xeb..."                
    [31] "   10576 \xac\xa0\xa9 23 19:28  Information Netwtw10               1073748845 7021 - Connection telemetry fields and analysis..."                                                                                        
    [32] "   10575 \xac\xa0\xa9 23 19:28  Information Netwtw10               1073748835 7011 - radio ON                                   "                                                                                        
    [33] "   10574 \xac\xa0\xa9 23 19:27  Information BTHUSB                 1074069522 \x91\xa8\xe1⥬\xa0 Windows \xad\xa5 \xac\xae\xa6\xa5\xe2 \xe1\xae\xe5࠭\xa8\xe2\xec \xaa\xae\xa4\xeb \xaf\u0ba2\xa5\xe0\xaa..."               
    [34] ""                                                                                                                                                                                                                        

### Оценка результата

В результате лабораторной работы мы получили основную информацию об ОС, процессоре и логи системы.

### Вывод

Таким образом, мы научились работать с базовыми командами командой строки и получать информацию об операционной системе.
