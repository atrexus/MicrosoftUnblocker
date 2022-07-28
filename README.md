# MicrosoftUnblocker
A program that can unblock any executable that is being blocked by Microsoft Family Systems. This unblocker does not do anything fancy, but simply exploits a vulnerability that I discovered over a year ago. Any of the current releases only work on Windows 10 and above due to the project using more recent .NET Frameworks. 

> This program does not remove any time limits from your computer as that would require fumbling with system binaries which are not done here at all. Doing something like that would require elevated permission (you need to be an administrator), which seems to be impossible.

### The Vulnerability
As I mentioned previously, MicrosoftUnblocker exploits a small (and may I add, quite dumb) vulnerability that I discovered a while ago. I noticed that when a program is called using the ``--app`` parameter from the command line it is undetected by the blocking software. As of now, I don't know why this is, most likely it has something to do with Microsoft not scanning for apps supposedly not launched by the current user.

## How do I use this?
I have tried to make this program as lightweight as possible and I was able to narrow it down to these few steps:
1. **Select the Executable**: Once opened the program will prompt you to select your app to unblock. The executable can not be a shortcut (they end in ``.lnk``), it must be the actual executable since the shortcut could be pointing to a different program than what you want to unblock.
2. **Wait for Message**: Now all you need to do is wait. This process could take a while depending on the application, but usually it gets done quite quickly. If the program succeeded, it should display a message like so: ![Screenshot1](https://github.com/Buff3rOverfl0w/MicrosoftUnblocker/blob/main/Images/Screenshot1.png) 
3. **Run the Unblocked App**: Finally, you can venture to that directory presented in the previous step and you have complete access to all of your unblocked apps! The icons may be quite pixilated and I apologise for that, I still need to find a workaround for them. 

