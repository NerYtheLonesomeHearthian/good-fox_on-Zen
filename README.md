# Good Fox on Zen Browser

This is a fork of [quiltedhills](https://github.com/quiltedhills)' [good-girl](https://github.com/quiltedhills/good-girl) aimed at making the script immediately work with the Zen Browser. It also adds more silly emoticons customization.

This script also changes the "They/Them" pronouns message from "Good bean." to "Good fox.".

<img width="612" height="158" alt="Good Fox example" src="https://github.com/user-attachments/assets/6908baef-d86c-4a76-a53a-1a209a14603b" />


Here's the customizable silly emoticons:

<img width="619" height="326" alt="Emoticon dropdown" src="https://github.com/user-attachments/assets/d7f4431d-1504-457f-8cbc-fa110d057e00" />


<img width="612" height="156" alt="Good Fox + Hearthian ::3 example" src="https://github.com/user-attachments/assets/7a6ebe68-3472-4289-a7bb-c34d36af405b" />


They obviously work with all pronouns:

<img width="609" height="154" alt="using ::3 with other pronouns example" src="https://github.com/user-attachments/assets/ce862c9a-0236-480d-8d26-751d10e32359" />



## Instructions

### Below is the revised README, modified for Zen:

This is an autoconfig script for ~Firefox~ Zen that adds a silly settings panel with an equally silly effect.

<img width="656" height="277" alt="Screenshot of the Firefox Browser Settings tab, with a message reading 'Firefox is your default browser. Good girl.'" src="https://github.com/user-attachments/assets/e1edcaf9-7baa-4953-8b13-bdf24ec569d5" />

(Other gender affirmation options are also available in the brand new [Pronouns dropdown](#preview) in Settings)
<hr>

### Installation
This should be your guide: https://support.mozilla.org/en-US/kb/customizing-firefox-using-autoconfig


#### For <ins>Windows</ins>, if you have not installed or used these kinds of scripts before, it would look like this:

##### 1) Get the files.
Hit the green **Code** button at the top, and then **Download ZIP**

##### 2) Get to your Zen directory.
Go to `C:/Program Files/Zen Browser/`, or `C:/Program Files (x86)/Zen Browser/`, or wherever your `zen.exe` file is located. To find it, you can search for the app in the Start menu and then click on "open file location" repeatedly until it brings you to the correct directory. Here's how:
<img width="837" height="474" alt="finding Zen in start menu" src="https://github.com/user-attachments/assets/bed1e753-fc0a-46c7-976c-70e110baa09c" />

<img width="622" height="44" alt="right clicking on Zen shortcut" src="https://github.com/user-attachments/assets/333a4fb8-fe31-4885-b7b6-6a971a608cdf" />

  
You then right click on the shortcut and press "open file location" once again.

##### 3) Place the files.
Extract the contents of the `Zen Browser/` folder of the ZIP file.

The result should be: the `zen.cfg` file in the main `\Zen Browser` directory, right next to `zen.exe`; the `autoconfig.js` file in the `\Zen Browser\defaults\pref` folder.

Here's an example: 

<img width="638" height="295" alt="zen.cfg location" src="https://github.com/user-attachments/assets/4211e47a-73ab-437f-9334-73461fb35994" />


<img width="653" height="190" alt="autoconfig.js location" src="https://github.com/user-attachments/assets/08741336-4253-47a6-a9dc-49e4d04f6d5e" />


##### 4) Restart Zen.
You can do this by completely closing the program or by going to `about:support` in a new tab and clicking on "Clear startup cache...".

And I think that should be it? (Please reach out to me if this doesn't work!)

#### For <ins>non-Windows</ins>, you should follow the link above to get the right paths and locations for everything!

And if you've previously had other scripts like this installed, you probably (hopefully) know better than me, and I hope you can figure out how to make multiple of them work simultaneously.

### Troubleshooting (if it doesn't work)
Zen sometimes ignores new `.js` files in the `defaults\pref\` folder if it already has its own configuration files taking priority.

Go to your `Zen Browser\defaults\pref\` folder.

If you see another `.js` file there (like `config-prefs.js` or `zen-prefs.js`) alongside the autoconfig.js you just added, open that existing Zen file in Notepad (or whatever code editor you prefer).

Add these two lines to the very bottom of that existing file:

```javascript
pref("general.config.filename", "zen.cfg");
pref("general.config.obscure_value", 0);
```

Save the file and restart the browser in the same way as before.

If you want, delete the extra `autoconfig.js` you added earlier, it should not be necessary anymore.

### Configuration (advanced)
> [!CAUTION]
> Make sure that any files you edit keep LF file endings!\
> If a script stops working after you edited it, double check that the file endings are not set to CRLF.
> 
> If you are editing the file in VSCode, there will be a little thingy in the bottom-right.

Most of the things you need are located in `zen.cfg`, which should end up near your `zen.exe` file after unpacking.\
Near the top of the file are some constants that you are free to tweak to your liking! (And you can tweak other parts of the script too, of course)\
Most of them have comments explaining what each thing does.

You can change where the Pronouns are located in settings, you can change what pronouns are available, and you can change what pronoun gives what message for the Default Browser screen.\

### Preview

Here are the showcase GIFs from the original repo:

<img width="632" height="222" alt="Screenshot of all settings options introduced by the script" src="https://github.com/user-attachments/assets/676e0c08-69c2-4bbb-bf91-54e612e83897" />
<hr>
<img width="750" alt="GIF showing off the Pronouns dropdown, and how it affects the Default Browser message" src="https://i.imgur.com/dnqoYt0.gif" />
