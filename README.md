# WhatsApp-Spammer

### What is this: -
This is a simple bot to automate spam messages if you want to annoy your friends.

### Things to remember: -
I'm not responsible for any damage made with this tool. This is just a tool, and the good or bad use of it is up to you

### Steps to make the bot work: -

1. Open WhatsApp (Web version)
1. Open the chat you want to spam.
1. Then hit <kbd>CTRL</kbd><kbd>SHIFT</kbd><kbd>I</kbd> or <kbd>F12</kbd>
1. copy the code from <a href="https://github.com/AlanCh4n/WhatsApp-Spammer/blob/main/bot.js">bot.js</a>
1. paste the code in browser console.
1. Hit enter then it will ask you to type your message and the number of times you want to send the message.
1. Done. 👍

### Code: -
```JS
var message = prompt("Enter your message", "‎");
var counter = parseInt(prompt("How many Times ?", 10));
window.InputEvent = window.Event || window.InputEvent;
var event = new InputEvent("input", { bubbles: true });
var textbox = document.getElementsByClassName("_1awRl copyable-text selectable-text")[1];
for (let index = 0; index < counter; index++) {
  textbox.innerHTML = message;
  textbox.dispatchEvent(event);
  document.getElementsByClassName("_2Ujuu")[0].click();
}
```
