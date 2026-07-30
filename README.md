# Good Girl
This is an autoconfig script for Firefox that adds a silly settings panel with an equally silly effect.

<img width="656" height="277" alt="Screenshot of the Firefox Settings tab, with a message reading 'Firefox is your default browser. Good girl.'" src="https://github.com/user-attachments/assets/e1edcaf9-7baa-4953-8b13-bdf24ec569d5" />

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

For <ins>non-Windows</ins>, you should follow the link above to get the right path!

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
<img width="750" alt="GIF showing off the Pronouns dropdown, and how it affects the Default Browser message when interacted with" src="https://i.imgur.com/dnqoYt0.gif" />
