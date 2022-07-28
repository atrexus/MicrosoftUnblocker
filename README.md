# MicrosoftUnblocker
A program that can unblock any executable that is being blocked by Microsoft Family Systems. This unblocker does not do anything fancy, but simply exploit a vulnurability that I discovered over a year ago. Any of the current releases only work on Windows 10 and above due to the project using more recent .NET Frameworks. 

> This program does not remove any time limits from your computer as that would require fumbling with system binaries which is not done here at all. That would be up for another project.

## How does it work?
As I mentioned previously, MicrosoftUnblocker exploits a small (and may I add, quite dumb) vulnurability that I discovered a while ago. I noticed that when a program is called using the ``--app`` parameter from the command line it is undetected by the blocking software. As of now I don't know why this is, most likely it has something to do with Microsoft not scanning for apps supposedly not launched by the current user.
