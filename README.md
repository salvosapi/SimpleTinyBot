# SimpleTinyBot
A simple tiny bot for telegram that reads basic commands and responds. Easily configurable, and apt for users who wish to deploy a simple bot without investing a lot of time into making it.

Introduction - A few things to know about SimpleTinyBot
--------------------------------------------------------------------------------------------------------
SimpleTinyBot is a basic bot written in php, to process simple commands and respond.
Nothing advanced, and nothing fancy.
A real world use of this bot would be for basic information delivering in group chats. 
---------------------------------------------------------------------------------------------------------
1)Configuration
-------------------------------------------------------------------------------------------------------
You must configure SimpleTinyBot with the botToken provided by BotFather
If the bot username and name is not set, it will automatically be fetched
The configuration parameters are defined in json format.

2)Welcome message
--------------------------------------------------------------------------------------------------------
The welcome message is a simple function that welcomes new users added to group chats.
It can be turned off by setting 'wl_enable' to 0 in the config file.

The message that is sent as a greeting is defined in the 'wl_message' setting.
Feel free to alter this to your heart's will.
--------------------------------------------------------------------------------------------------------

3)Commands
---------------------------------------------------------------------------------------------------------
The commands that the bot will look for are set in the commands file.
The commands are set in json format.

The commands are followed by a colon and their responses. Like so
"/sayHello":"Hello guys!"

The above command works as follows
Bot receives input from user in chat -> Bot searches for command /sayHello -> If Bot finds it -> Reply "Hello Guys"


SimpleTinyBot looks for strings mentioned as commands, so feel free to put a forward slash in there or not.
It is adviced to preceed all commands with forward slashes.

The commands you add must follow the json pattern. 

That is, each command must be followed by a colon and its value.
Commands should be enclosed in double quotes, and responses should be enclosed in double quotes too.

NOTE: SINGLE QUOTES ARE NOT SUPPORTED AND WILL CAUSE PROBLEMS

"/command" : "the response";


------------------------------------------------------------------------------------------------------------

4)Security Concerns
------------------------------------------------------------------------------------------------------------
Since the config file contains sensitive information(bot token), it is advised that you store all files of 
SimpleTinyBot in a directory which is named the same as your token.

Here <token> refers to the actual token from BotFather.
<SimpleTinyBot> refers to the SimpleTinyBot files.
example - public_html/<token>/<SimpleTinyBot>

Well, that's about it! :)
For help, join the chat in the link!

https://telegram.me/joinchat/AOmo4gErOrtxl-oF4T24Ig

You can ask for Master Twamp, or King Haider in the chat :)
