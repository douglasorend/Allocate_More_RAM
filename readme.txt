[hr]
[center][color=red][size=16pt][b]ALLOCATE MORE RAM v1.1[/b][/size][/color]
[url=http://www.simplemachines.org/community/index.php?action=profile;u=253913][b]By Dougiefresh[/b][/url] -> [url=http://custom.simplemachines.org/mods/index.php?mod=3848]Link to Mod[/url]
[/center]
[hr]

[color=blue][b][size=12pt][u]Introduction[/u][/size][/b][/color]
[url=http://wiki.simplemachines.org/smf/What_the_white_screen_of_death_means_when_accessing_admin_or_package_installs]This page[/url] begins to explain the problem:
[quote]
The issue appears to be that when a page is loaded, and the script tries to load one (or more) additional files to perform sub-tasks, the system runs out of allocated memory.

The reason this is happening is because those of you encountering this issue are very likely running your site on an overselling host. This means that the host you chose sells sites with "unlimited" stuff, such as bandwidth, or disk space. The truth is that nobody could actually afford to sell "unlimited" everything (or anything). Hosts need to pay for expenses and make money. The host that you chose may advertise "unlimited", but in reality, they have severely limited your account, because they put far too many "unlimited" accounts on the same physical, or virtual, machine. They then apply "hidden" limits, and shut your forum down, when your usage exceeds these limits. Even though you are, therefore, meant to have been offered an "unlimited" service, you have not.

It is important to realize that there is a limit to how much memory a given script can access, and that every host has a limit like this. A real host, however, has a reasonable amount, and will not put far too many accounts on a single server such that they overuse the available resources, and a real host will discuss how much you require if you truly need to exceed that amount.

In your case, the host has set this limit low. So low, in fact, that the package manager cannot load Subs-Post.php to process the BBC tags in the readme file of the mod. If that inclusion is bypassed, the script next chokes on the loading of Subs-Package.php, which cannot be bypassed because that file contains the instructions needed to process the Mod package.[/quote]

[color=blue][b][size=12pt][u]What It Does[/u][/size][/b][/color]
This mod makes a small change to Class-Package.php to increase the memory requested from 32mb to 128mb, as described in [url=http://www.simplemachines.org/community/index.php?topic=502354.msg3531634#msg3531634]this post[/url].  Please note that this modification is not guaranteed to work, however, it works for me....

[color=blue][b][size=12pt][u]Admin Settings[/u][/size][/b][/color]
There are no admin settings.  To disable it, you must remove this mod.

[color=blue][b][size=12pt][u]Compatibility Notes[/u][/size][/b][/color]
This mod was tested on SMF 2.0.7, but should work on SMF 2.0 and up.  SMF 1.1 is not and will not be supported, so please don't ask.

[color=blue][b][size=12pt][u]Changelog[/u][/size][/b][/color]
[quote]
[b]v1.1 - March 20th, 2014[/b]
o Version restriction of mod packaging to not allow it to run on SMF 2.0.8+

[b]v1.0 - March 20th, 2014[/b]
o Initial Release of the mod
[/quote]

[hr]
[url=http://creativecommons.org/licenses/by/3.0][img]http://i.creativecommons.org/l/by/3.0/80x15.png[/img][/url]
This work is licensed under a [url=http://creativecommons.org/licenses/by/3.0]Creative Commons Attribution 3.0 Unported License[/url]
