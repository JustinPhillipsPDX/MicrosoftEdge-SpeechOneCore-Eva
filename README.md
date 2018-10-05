# MicrosoftEdge-SpeechOneCore-Eva
A .reg file that adds the selection of Microsoft Eva to Microsoft Edge's Read aloud voices dropdown list.

![annotation](https://user-images.githubusercontent.com/29287158/46510559-9a59d800-c7fe-11e8-87e4-dd91a8ecee84.png)

## .reg File Contents

```
Windows Registry Editor Version 5.00
```
```
[HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\CurrentVersion\AppContainer\Storage\microsoft.microsoftedge_8wekyb3d8bbwe\Children\001\Software\Microsoft\Speech_OneCore\Isolated\k6BwW5fty3XWMlmQDjzUq77TXIsLVjJGt268p8btklc\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Speech_OneCore\Voices\Tokens\MSTTS_V110_enUS_EvaM]
```
```
@="Microsoft Eva - English (United States)"
"LangDataPath"="%windir%\\Speech_OneCore\\Engines\\TTS\\en-US\\MSTTSLocenUS.dat"
"VoicePath"="%windir%\\Speech_OneCore\\Engines\\TTS\\en-US\\M1033Eva"
"409"="Microsoft Eva - English (United States)"
"CLSID"="{179F3D56-1B0B-42B2-A962-59B7EF59FE1B}"
```
```
[HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\CurrentVersion\AppContainer\Storage\microsoft.microsoftedge_8wekyb3d8bbwe\Children\001\Software\Microsoft\Speech_OneCore\Isolated\k6BwW5fty3XWMlmQDjzUq77TXIsLVjJGt268p8btklc\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Speech_OneCore\Voices\Tokens\MSTTS_V110_enUS_EvaM\Attributes]
```
```
"Version"="11.0"
"Language"="409"
"Gender"="Female"
"Age"="Adult"
"DataVersion"="11.0.2013.1022"
"SharedPronunciation"=""
"Name"="Microsoft Eva"
"Vendor"="Microsoft"
"SayAsSupport"="spell=NativeSupported; cardinal=GlobalSupported; ordinal=NativeSupported; date=GlobalSupported; time=GlobalSupported; telephone=NativeSupported; currency=NativeSupported; net=NativeSupported; url=NativeSupported; address=NativeSupported; alphanumeric=NativeSupported; Name=NativeSupported; media=NativeSupported; message=NativeSupported; companyName=NativeSupported; computer=NativeSupported; math=NativeSupported; duration=NativeSupported"
"SampleText"="You have selected %1 as the default voice."
```
