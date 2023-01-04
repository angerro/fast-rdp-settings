# fast-rdp-settings
Настройки Windows для быстрого коннекта к ней по RDP протоколу

## Настройки RemoteFX
Подробнее можно почитать [здесь](https://gist.github.com/Misairu-G/616f7b2756c488148b7309addc940b28#remotefx-configure-and-fine-tuning):
1. Запускаем `gpedit.msc` через `Win+R`
2. Идем в `Computer Configuration -> Administrative Templates -> 
Windows Components -> Remote Desktop Service -> Remote Desktop Session Host -> 
Remote Session Environment`
    - включаем `Use advanced RemoteFX graphics for RemoteApp`
    - включаем `Configure compression for RemoteFX data` (выбираем `Do not use an RDP compression algorithm`)
    - включаем `Configure image quality for RemoteFX adaptive Graphics` (выбираем `High`)
    - включаем `Enable RemoteFX encoding for RemoteFX clients designed for Windows Server 2008 R2 SP1`
    - включаем `Configure RemoteFX Adaptive Graphics` (выбираем `Optimize for minimum bandwidth usage`)
3. Идем в `Computer Configuration -> Administrative Templates -> 
Windows Components -> Remote Desktop Service -> Remote Desktop Session Host -> 
Remote Session Environment -> RemoteFX for Windows Server 2008 R2`
    - включаем `Configure RemoteFX`
    - включаем `Optimize visual experience when using RemoteFX` (выбираем `Highest`)
