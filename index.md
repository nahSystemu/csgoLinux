
### 1. Installing Pre-Dependencies 
`apt-get install lib32gcc1`

### 2. Downloading and Installing SteamCMD

1. `useradd -m steam`
2. `su - steam`
   `mkdir ~/Steam && cd ~/Steam`
3. `wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz`
   `tar xf steamcmd_linux.tar.gz`   
   `./steamcmd.sh`

### 3. Using SteamCMD to Download Server Files

   `login <username> <password>`
   `force_install_dir ./csgo/`
   `app_update 740 validate`

### 4. Launching server
[Link to Dev page](https://steamcommunity.com/dev/managegameservers)

`./srcds_run -game csgo -console -usercon +game_type 0 +game_mode 1 +mapgroup mg_active +map de_dust2 +sv_setsteamaccount THISGSLTHERE -net_port_try`
