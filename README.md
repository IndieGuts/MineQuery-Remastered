Reminders:
[ ] - Complete the ReadMe
[ ] - 

Feature Requests:
[ ] - Currently None

Donators:
[ ] - Currently none



# MineQuery-Remastered
Get the information of a Minecraft server using MineQuery Remastered!

** Reminder: **
You'll need to download the core.minequery-remastered.php file, and upload it into your project.
(I suggest creating a folder called "core" and placing this inside there)

** "How can I load the core?" **
Place this PHP snippet into your content where you wish to place the server information
```PHP
<?php // Load MineQuery - Remastered Core
	require('path/to/core.minequery-remastered.php');
	$minequery = new MineQueryRemastered;
?>
```

** "How can I include it on multiple pages, without spamming the snippet on each page?" **
If you know common PHP practices, you can simply place the snippet into a 
header.php file, then require that header.php onto all of your pages!

** "What server information can I get using MineQuery Remastered?" **
Please read the below information, and examples!

** playerSkin - Use this to get a players skin. **
Specify the players "Username", Size of the picture, then "true" or "false" to also apply their hat.
```PHP
<?=$minequery::playerSkin("IndieGuts", 150, "true"); ?>
```

** rawSkin - Use this to get a rawskin of a player **
Specify the players "Username"
```PHP
<?=$minequery::rawSkin("IndieGuts"); ?>
```

** playerHead **
Specify the players "Username", Size of the picture, then "true" or "false" to also apply their hat.
```PHP
<?=$minequery::playerHead("IndieGuts", 150, "true"); ?>PHP
```

** Minecraft & Mojang Server Status **
```PHP
<?=$minequery::statusMinecraft(); ?> » Returns the status of minecraft.net
<?=$minequery::statusMojang(); ?> » Returns the status of session.minecraft.net
<?=$minequery::statusMinecraftSessions(); ?> » Returns the status of account.mojang.com
<?=$minequery::statusAccountAuth(); ?> » Returns the status of authserver.mojang.com
<?=$minequery::statusAuthServer(); ?> » Returns the status of sessionserver.mojang.net
<?=$minequery::statusMojangSession(); ?> » Returns the status of api.mojang.com
<?=$minequery::statusAPI(); ?> » Returns the status of mojang.com
```
** isItUp **
Using this, you can check if an IP, or domain is currently online, or offline! Simply specify a destination!
```
<?=$minequery::isItUp("play.indieguts.com"); ?>
```

** Minecraft Server Information **
Please read below for features that you can use to get information from Minecraft servers!

** Favicon **
Use this to get the favicon (server icon) of a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::favicon("us.mineplex.com"); ?>
```

** Status **
Use this to get the status of a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::status("play.indieguts.com"); ?>
```

** Ping **
Use this to get the viewers ping to the server! Simply specify a server domain or IP!
```PHP
<?=$minequery::ping("play.indieguts.com"); ?>
``` » Will return the viewers ping to the destination

** Online **
Use this to check how many players are online in a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::online("play.indieguts.com"); ?>
```

** Maxplayers **
Use this to get the max players limit on a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::maxplayers("play.indieguts.com"); ?>
```

** Version **
Returns the server version! Simply specify a server domain or IP!
```PHP
<?=$minequery::version("play.indieguts.com"); ?>PHP
``` » May also specify multiple versions if supported

** Protocol **
Get the protocol version of a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::protocol("play.indieguts.com"); ?>
```

** MOTD **
Use this to get the MOTD of a server!
Specify the server domain or IP, then use true to get the & colors, or false, to turn the colors to HTML colors!
```PHP
<?=$minequery::motd("us.mineplex.com", false); ?>
```

** Port **
Get the port version of a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::port("us.mineplex.com"); ?>
```

** Hostname ** (This does NOT mean the hosting or service provider, but the servers connection domain)
Get the hostname version of a server! Simply specify a server domain or IP!
```PHP
<?=$minequery::hostname("us.mineplex.com"); ?>
```

** Query Features**
The server query must be enabled on the targed server to work
enable-query must be set to true in the requested server's server.properties file for this API to work

** Software **
This feature has yet to be described...
```PHP
<?=$minequery::software("us.mineplex.com"); ?>
```

** Gametype **
This feature has yet to be described...
```PHP
<?=$minequery::gametype("us.mineplex.com"); ?>
```

** Map **
This feature has yet to be described...
```PHP
<?=$minequery::map("us.mineplex.com"); ?>
```

** BuyCraft API **
This feature has yet to be described...

** MinecraftMarket API **
This feature has yet to be described...

** Mojang Blacklisted Servers **
This feature has yet to be described...
