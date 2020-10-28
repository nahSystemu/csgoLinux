# Setting up a CSGO Linux Server

## Part 1 - Setting up SteamCMD & Installing CSGO

### 	1.1 Installing Pre-Dependencies 
- 	`apt-get install lib32gcc1`

### 	1.2 Downloading and Installing SteamCMD

- 	`useradd -m steam`
- 	`su - steam`\
	`mkdir ~/Steam && cd ~/Steam`
- 	`wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz`\
	`tar xf steamcmd_linux.tar.gz`\
	`./steamcmd.sh`

### 	1.3 Using SteamCMD to Download Server Files

- 	`login <username> <password>`
- 	`force_install_dir ./csgo/`
- 	`app_update 740 validate`

### 	1.4 Launching server
-	[Link to Dev page](https://steamcommunity.com/dev/managegameservers)

	`./srcds_run -game csgo -console -usercon +game_type 0 +game_mode 1 +mapgroup mg_active +map de_dust2 +sv_setsteamaccount THISGSLTHERE -net_port_try`

## Part 2 - Sourcemod & Metamod

### 	2.1 Downloading Sourcemod & Metamod

- 	[Souremod](https://www.sourcemm.net/downloads.php/?branch=stable)
- 	[Metamod](https://www.sourcemod.net/downloads.php?branch=stable)

### 	2.2 Installing Sourcemod & Metamod

- 	Extract contents to `/csgo/` directory

### 	2.3 Generating Metamod VDF

- 	[Link to VDF](https://www.sourcemm.net/vdf)\
	Extract to `/csgo/addons/`
