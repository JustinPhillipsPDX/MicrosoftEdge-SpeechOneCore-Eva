# MicrosoftEdge-SpeechOneCore-Eva
A .reg file that adds the selection of Microsoft Eva (**Cortana**'s voice) to Microsoft Edge's Read aloud voices dropdown list.

![annotation](https://user-images.githubusercontent.com/29287158/46510559-9a59d800-c7fe-11e8-87e4-dd91a8ecee84.png)

## Installation
After downloaded the .reg file you will need to edit the file using a text editor of your choice. Change the KEYs within the **HKEY_CURRENT_USER** paths for both *Tokens* key and the *Tokens* *Attributes* key to match Edge's current installation. You can find the KEY Names by opening Registry Editor selecting **HKEY_CURRENT_USER** and then pressing **Ctrl+F**. Search for "**MSTTS_V110_enUS_DavidM**" while selecting Look at: "**Keys**" along with "**Match whole string only**". Next, press **F3** (if applicatble) to cycle through "**Find Next**" until you locate **microsoft.microsoftedge_[version number]** (my version was **microsoft.microsoftedge_8wekyb3d8bbwe**, if your version is different you will need to update it in the .reg file).

![01](https://user-images.githubusercontent.com/29287158/46512547-60420380-c809-11e8-80f1-c747462d53f2.PNG)

![02](https://user-images.githubusercontent.com/29287158/46512851-df840700-c80a-11e8-9bcd-5161ba4c09fe.PNG)

In this example I want to copy the last *Isolated* **Key Name** of "**k6BwW5fty3XWMlmQDjzUq77TXIsLVjJGt268p8btklc**" into the .reg file

![03](https://user-images.githubusercontent.com/29287158/46513242-90d76c80-c80c-11e8-8cbf-5f9a45c16653.PNG)

Once the versions have been updated in the **HKEY_CURRENT_USER** paths, save and double click the .reg file to install.

![04](https://user-images.githubusercontent.com/29287158/46513547-e95b3980-c80d-11e8-9975-f86503f54934.PNG)

You will be presented with a warning, click **YES** to continue.

![05](https://user-images.githubusercontent.com/29287158/46513593-2d4e3e80-c80e-11e8-89c4-8a9e3337944e.PNG)

Click **OK**.

![06](https://user-images.githubusercontent.com/29287158/46513618-4ce56700-c80e-11e8-8133-99a55787e675.PNG)

Finally, you can verify the new Key entries in Registry Editor. Open Edge and right-click on a page select **Read aloud**, go into the upper right corner settings and select **Microsoft Eva - English (United States)** from voices.

![annotation](https://user-images.githubusercontent.com/29287158/46510559-9a59d800-c7fe-11e8-87e4-dd91a8ecee84.png)

## .reg File Contents

```
Windows Registry Editor Version 5.00
```

[HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\CurrentVersion\AppContainer\Storage\microsoft.microsoftedge_8wekyb3d8bbwe\Children\001\Software\Microsoft\Speech_OneCore\Isolated\ **[[UPDATE WITH LAST KEY ENTRY FROM REGISTRY EDITOR]]** \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Speech_OneCore\Voices\Tokens\MSTTS_V110_enUS_EvaM]

```
@="Microsoft Eva - English (United States)"
"LangDataPath"="%windir%\\Speech_OneCore\\Engines\\TTS\\en-US\\MSTTSLocenUS.dat"
"VoicePath"="%windir%\\Speech_OneCore\\Engines\\TTS\\en-US\\M1033Eva"
"409"="Microsoft Eva - English (United States)"
"CLSID"="{179F3D56-1B0B-42B2-A962-59B7EF59FE1B}"
```
[HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\CurrentVersion\AppContainer\Storage\microsoft.microsoftedge_8wekyb3d8bbwe\Children\001\Software\Microsoft\Speech_OneCore\Isolated\ **[[UPDATE WITH LAST KEY ENTRY FROM REGISTRY EDITOR]]** \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Speech_OneCore\Voices\Tokens\MSTTS_V110_enUS_EvaM\Attributes]

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
