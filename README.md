# HTTP protocol redirector
[![pages-build-deployment](https://github.com/intradeus/http-protocol-redirector/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/intradeus/http-protocol-redirector/actions/workflows/pages/pages-build-deployment)

```
                                  https://intradeus.github.io/http-protocol-redirector?r=
```
## Why 
Ever wanted to  
- redirect some users to your own software, but Slack / Discord / Google Chat / Teams said "No!"
- redirect your dev team from their PR to vscode instantly, but Github said "No !"

Then http-protocol-redirector is for you :)

No analytics, no nonsense, just 2 lines of code.

(There are no plans to add a shorter domain for now, as github.io has more chance to be alive in 10 years than my own domain.)

## How 
Simply add `https://intradeus.github.io/http-protocol-redirector?r=` in front of your own URL with your own protocol, and it'll forward it.


Let's say you have the [ms-vscode.remote-repositories](https://marketplace.visualstudio.com/items?itemName=github.remotehub) extension for vscode and want your team to open a link.

Then, neither this vscode protocol link is clickable, nor is its hyperlink version :  
- vscode://ms-vscode.remote-repositories/open?url=https://github.com/intradeus/http-protocol-redirector
- [hyperlink version](vscode://ms-vscode.remote-repositories/open?url=https://github.com/intradeus/http-protocol-redirector)

But by adding the redirector, you can make it clickable : 
- https://intradeus.github.io/http-protocol-redirector?r=vscode://ms-vscode.remote-repositories/open?url=https://github.com/intradeus/http-protocol-redirector
- [hyperlink version](https://intradeus.github.io/http-protocol-redirector?r=vscode://ms-vscode.remote-repositories/open?url=https://github.com/intradeus/http-protocol-redirector)

## Watch out
I know that there is a security reason why these companies don't allow custom protocols to be opened, but sometimes you just wanna do more with their tools. 

This is just a reminder that you should always see the content of any hyperlink you're clicking on, and you should never open something that you do not trust.

Fortunately, browsers will always ask you if you want to open something in a software, before actually opening it :)
