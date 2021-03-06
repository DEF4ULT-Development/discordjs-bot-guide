# Common Errors

## Cannot find module `discord.js`

### Problem:

You didn't install Discord.js or installed it in the wrong folder.

### Solution:

* Make sure you are in the **correct** folder where you have your bot's files
* SHIFT+Right-Click in the folder and select **Open command window here**
* Run `npm init -y`, and hit enter until the wizard is complete
* Run `npm i discord.js` again to install Discord.

## `Error: getaddrinfo ENOTFOUND gateway.discord.gg gateway.discord.gg:443`

### Problem:

Your internet went down.

### Solution:

Get better, more stable internet, or host your bot on a VPS.

## Unexpected End of Input

### Problem:

```text
});
^
SyntaxError: Unexpected end of input
```

### Solution:

Your code has an error somewhere. This is _impossible_ to troubleshoot without the **complete** code, since the error can be anywhere \(in fact the error stack often tells you it's at the end of your code\).

The following trick is a lifesaver, so pay attention: Your code editor is trying to help you. Whatever editor you're using \(except notepad++.exe. Don't use notepad++!\), clicking on any \(and I mean any\) special character such as parentheses, square brackets, curly braces, double and single quotes, will automatically highlight the one that matches it. The screenshot below shows this: I clicked on the curly brace at the bottom, it shows me the one on top by highlighting it. Learn this, and how different functions and event handlers "look" like.

![](.gitbook/assets/editorhelp.png)

You can check out [Installing and Using a Proper Editor](other-guides/installing-and-using-a-proper-editor.md) to help in at least knowing there are errors _before_ running your bot code.

## `Error: fields.flat is not a function.`

### Problem:

Discord.js v12 requires atleast node v12.You didn't install node v12 or higher version.

### Solution:

* Install node of version 12 or higher in your machine.

## `Error: .addBlankField is not a function`

### Problem:

`.addBankField()` is depriciated in `discord.js v12`

## Solution:

Instead of `.addBlankField()` you can do `.addField("\u200B","\u200B")` which does the same thing.


## `AbortError: The user aborted a request.`

### Problem: 

This error usually occurs when a request takes long time to resolve it.

### Solution:

* Increase [restRequestTimeout](https://discord.js.org/#/docs/main/stable/typedef/ClientOptions) value in client constructor(options).



