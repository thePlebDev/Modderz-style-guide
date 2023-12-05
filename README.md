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

## Table Of Content

- [Dialog Builders](#builders)
    - [RadioButtonDialog](#RadioButtonDialog)
    - [Dialog Parts](#parts)

 - [Chats Builders](#Chats)
    - [TwitchIRCSystemNotificationsBuilders](#TwitchIRCSystemNotificationsBuilder)
         - [SystemChat](#SystemChat)
         - [SystemChatAlert](#SystemChatAlert)



### RadioButtonDialog <a name="RadioButtonDialog"></a>
 - A typical RadioButtonDialog will look similiar to this:

<img width="204" alt="BanDialog" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/844b0a77-8f85-4ac9-91f9-6049288d9225">



## Chats Builders <a name="Chats"></a>
- Below is representation of all the [Builders](https://dev.to/theplebdev/the-architectural-patterns-i-am-using-to-better-organize-my-jetpack-compose-code-1hj) that I use to create chat messages from data sent from [Twitch IRC server](https://dev.twitch.tv/docs/irc/commands/).

### TwitchIRCSystemNotificationsBuilders <a name="TwitchIRCSystemNotificationsBuilder"></a>
- This is the builder class that is used to outline the two types of builders in chat, `SystemChat` and `SystemChatAlert`


#### SystemChat <a name="SystemChat"></a>
  - This chat design is meant to represent the typical system message sent from [Twitch IRC server](https://dev.twitch.tv/docs/irc/commands/). Typically a `SystemChat` will follow this design:
 
<img width="249" alt="systemChat" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/eb5cf180-6c5a-40d7-a031-8ab425e4da99">

  #### SystemChatAlert <a name="SystemChatAlert"></a>
   - This chat design is meant to represent a alert shown to urgent data to the user. Typically a `SystemChatAlert` will follow this design:

<img width="251" alt="systemChatAlert" src="https://github.com/thePlebDev/Modderz-style-guide/assets/47083513/a9848339-846a-4073-b095-1298c7f04738">



   

  
