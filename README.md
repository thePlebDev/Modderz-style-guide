<h1 align="center">
  Modderz Android app
  </h1>
<a href="https://aimeos.org/">
    <img src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/264372d7-3802-4a75-b7f5-0d1b29bf40f9" alt="Aimeos logo" title="Aimeos" align="right" height="60" />
</a>
<a href="https://aimeos.org/">
    <img src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/264372d7-3802-4a75-b7f5-0d1b29bf40f9" alt="Aimeos logo" title="Aimeos" align="left" height="60" />
</a>

<h3 align="center">
  <i align="center">Twitch's unoffical mobile modview style guide 🚀</i>
</h3>

<h4 align="center">
  <a href="https://play.google.com/store/apps/details?id=elliott.software.clicker">
    <img src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/e18a269d-931b-4d30-a307-2ac04f59ca72" alt="link to google play store for app" >
  </a>
  

</h4>

## GitHub Code:
- [HERE](https://github.com/thePlebDev/Clicker)

## Table Of Content

- [Dialog Builders](#builders)
    - [RadioButtonDialog](#RadioButtonDialog)
    - [Dialog Parts](#parts)

 - [Chats Builders](#Chats)
    - [TwitchIRCSystemNotificationsBuilders](#TwitchIRCSystemNotificationsBuilder)
         - [SystemChat](#SystemChat)
         - [SystemChatAlert](#SystemChatAlert)
    - [ChatBuilder](#ChatBulders)
         - [ScrollableChat](#ScrollableChat)
     
   - [TextChatBuilders](#TextChatBuilders)
        - [EnterChat](#EnterChat)
          
   - [BottomModalBuilders](#BottomModalBuilders)
        - [BottomModalContent](#BottomModalContent)
    
   - [ChatSettingsBuilder](#ChatSettingsBuilder)
        - [ChatSettingsSwitchBox](#ChatSettingsSwitchBox)



### RadioButtonDialog <a name="RadioButtonDialog"></a>
 - A typical RadioButtonDialog will look similiar to this:

<img width="204" alt="BanDialog" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/844b0a77-8f85-4ac9-91f9-6049288d9225">



## Chats Builders <a name="Chats"></a>
- Below is representation of all the [Builders](https://dev.to/theplebdev/the-architectural-patterns-i-am-using-to-better-organize-my-jetpack-compose-code-1hj) that I use to create chat messages from data sent from [Twitch IRC server](https://dev.twitch.tv/docs/irc/commands/) and the individual chats sent by user

### TwitchIRCSystemNotificationsBuilders <a name="TwitchIRCSystemNotificationsBuilder"></a>
- This is the builder class that is used to outline the two types of builders in chat, `SystemChat` and `SystemChatAlert`


#### SystemChat <a name="SystemChat"></a>
  - This chat design is meant to represent the typical system message sent from [Twitch IRC server](https://dev.twitch.tv/docs/irc/commands/). Typically a `SystemChat` will follow this design:
 
<img width="249" alt="systemChat" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/eb5cf180-6c5a-40d7-a031-8ab425e4da99">

#### SystemChatAlert <a name="SystemChatAlert"></a>
   - This chat design is meant to represent a alert shown to urgent data to the user. Typically a `SystemChatAlert` will follow this design:

<img width="251" alt="systemChatAlert" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/a9848339-846a-4073-b095-1298c7f04738">


### ChatBuilder <a name="ChatBulders"></a>
- This is the builder class that is used to outline the types of builders used to create the user's chat experience

  #### ScrollableChat <a name="ScrollableChat"></a>
     - Contains all the composables that are to be used to create the basic user experience. Typically all ScrollableChat will look something like this:
       

<img width="261" alt="BasicChatExperience" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/5c8d7b33-8315-4e7b-8601-290383103085">

### TextChatBuilders <a name="TextChatBuilders"></a>
- These builder class' are used to outline the type of composabes in the typing chat functionality. Essentially, where the user types their chat messages

  #### EnterChat <a name="EnterChat"></a>
     - Contains all the composables that are to be used to create the basic user typing experice. Typically, all composables that use the TextChatBuilders.EnterChat will look something like this:
 

<img width="258" alt="ChatBuilder" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/10525d5a-337a-4f9b-97ed-9bf56b0825be">

### BottomModalBuilders <a name="BottomModalBuilders"></a>
- These builders are used to outline the basic layout for the bottom modal. Which is triggered when a user clicks on a chat message

  #### BottomModalContent <a name="BottomModalContent"></a>
     - BottomModalContent is the basic layout for the bottom modal and is usually used in combination with a [RadioButtonDialog](#RadioButtonDialog).
     - A typical UI demonstration ***without***  and ***with*** the dialog will look like this:
       
<img width="254" alt="BottomContentNoDialog" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/59fe7f4a-7593-4cc7-9a30-ccd944722777" style="display:inline-block;">  
<img width="257" alt="BottomContentWithDialog" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/6f8350ad-061c-4410-bca5-e01c59b2dcf6" style="display:inline-block;">


### ChatSettingsBuilder <a name="ChatSettingsBuilder"></a>
- These builders are used to outline the basic layout for the chat settings while the user views the stream.

  #### ChatSettingsSwitchBox <a name="ChatSettingsSwitchBox"></a>
     - ChatSettingsSwitchBox is the basic layout for the chat settings section in the chat. A typical UI demonstration will look like this:
       
<img width="225" alt="ChatSettingsWithAlert" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/5571445e-bc4b-4737-9781-19c7a8264866">

  
