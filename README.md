# Good Girl
This is an autoconfig script for Firefox that adds a silly settings panel with an equally silly effect.

Below there is a revised README for installing the script on Zen.

<img width="656" height="277" alt="Screenshot of the Firefox Browser Settings tab, with a message reading 'Firefox is your default browser. Good girl.'" src="https://github.com/user-attachments/assets/e1edcaf9-7baa-4953-8b13-bdf24ec569d5" />

(Other gender affirmation options are also available in the brand new [Pronouns dropdown](#preview) in Settings)
<hr>

## Installation
This should be your guide: https://support.mozilla.org/en-US/kb/customizing-firefox-using-autoconfig

For <ins>Windows</ins>, if you have not installed or used these kinds of scripts before, it would look like this:
- Hit the green **Code** button at the top, and then **Download ZIP**
- Go to `C:/Program Files/Mozilla Firefox/`, or `C:/Program Files (x86)/Mozilla Firefox/`, or wherever your `firefox.exe` file is located
- Extract the contents of the `Mozilla Firefox/` folder of the ZIP file
- Restart Firefox

And I think that should be it? (Please reach out to me if this doesn't work!)

For <ins>non-Windows</ins>, you should follow the link above to get the right paths and locations for everything!

And if you've previously had other scripts like this installed, you probably (hopefully) know better than me, and I hope you can figure out how to make multiple of them work simultaneously.

## Configuration
> [!CAUTION]
> Make sure that any files you edit keep LF file endings!\
> If a script stops working after you edited it, double check that the file endings are not set to CRLF.
> 
> If you are editing the file in VSCode, there will be a little thingy in the bottom-right.

Most of the things you need are located in `firefox.cfg`, which should end up near your `firefox.exe` file after unpacking.\
Near the top of the file are some constants that you are free to tweak to your liking! (And you can tweak other parts of the script too, of course)\
Most of them have comments explaining what each thing does.

You can change where the Pronouns are located in settings, you can change what pronouns are available, and you can change what pronoun gives what message for the Default Browser screen.\
And a little extra!

## Preview
<img width="632" height="222" alt="Screenshot of all settings options introduced by the script" src="https://github.com/user-attachments/assets/676e0c08-69c2-4bbb-bf91-54e612e83897" />
<hr>
<img width="750" alt="GIF showing off the Pronouns dropdown, and how it affects the Default Browser message" src="https://i.imgur.com/dnqoYt0.gif" />


# Good Fox on Zen Browser
This is a revised version of the README aimed at making the script immediately work with the Zen Browser. It also adds more silly emoticons customization.

It comes from the [fork](https://github.com/NerYtheLonesomeHearthian/good-fox_on-Zen) made by [NerYtheLonesomeHearthian](https://github.com/NerYtheLonesomeHearthian).

This script also changes the "They/Them" pronouns message from "Good bean." to "Good fox.". Keep in mind that this specific change will apply only to the version of the script in the `Zen Browser` folder.

<img width="612" height="158" alt="Screenshot (001238)" src="https://github.com/user-attachments/assets/75260bd5-5a04-46bf-8343-ba53a919e14c" />


Here's the customizable silly emoticons:

<img width="611" height="323" alt="Screenshot (001245)" src="https://github.com/user-attachments/assets/c605b2fb-1e2a-4254-aa15-0c07f898910e" />


<img width="609" height="154" alt="Screenshot (001239)" src="https://github.com/user-attachments/assets/36311166-7cfc-45ef-ad22-76bd8099becb" />

They obviously work with all pronouns:

<img width="612" height="156" alt="Screenshot (001236)" src="https://github.com/user-attachments/assets/42425a40-0ec6-4e67-9e5b-45a6ecfc9273" />


## Below is the README, modified for the Zen installation:

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
<img width="837" height="474" alt="Screenshot (001241)" src="https://github.com/user-attachments/assets/3e7b4cec-d49d-4783-9454-9527b0702f3f" />

<img width="622" height="44" alt="Screenshot (001242)" src="https://github.com/user-attachments/assets/d866b5d3-7580-4c4d-9556-cc85373c8163" />
  
You then right click on the shortcut and press "open file location" once again.

##### 3) Place the files.
Extract the contents of the `Zen Browser/` folder of the ZIP file.

The result should be: the `zen.cfg` file in the main `\Zen Browser` directory, right next to `zen.exe`; the `autoconfig.js` file in the `\Zen Browser\defaults\pref` folder.

Here's an example: 

<img width="638" height="295" alt="Screenshot (001244)" src="https://github.com/user-attachments/assets/3660fc18-819a-4168-a70a-9f82db863543" />

<img width="653" height="190" alt="Screenshot (001243)" src="https://github.com/user-attachments/assets/3ff6cfa4-9fdb-405f-addc-b51d0cc09c83" />

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
And a little extra!
