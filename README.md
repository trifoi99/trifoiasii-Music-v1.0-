<img width="150" height="150" align="right" style="float: right; margin: 0 10px 0 0;" alt="music_disc" src="https://i.imgur.com/JWSIlSt.png">

# Music Disc 

<a href="https://github.com/hmes98318/Music-Disc/releases"><img alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/hmes98318/Music-Disc?style=for-the-badge"></a> 
<a href="https://discord.js.org/"><img src="https://img.shields.io/badge/Discord.JS-v14-blue?style=for-the-badge&logo=DISCORD" /></a> 
<a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node%20Version->=16.13.0-brightgreen?style=for-the-badge&logo=Node.js"></a> 
<a href="https://github.com/hmes98318/Music-Disc/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/hmes98318/Music-Disc?style=for-the-badge&color=brightgreen"></a>  

### Discord.js v14 Music Bot  
Supports **YouTube**, **Spotify**, **SoundCloud** streams.


### Reference version  
[**node.js  `v18.12.1`**](https://nodejs.org/en/)  
[**discord.js  `v14.6.0`**](https://www.npmjs.com/package/discord.js)  


## Deploying with node.js

### Clone the repository
```
git clone -b v1.2.4 https://github.com/hmes98318/Music-Disc.git
```
or [**click here**](https://github.com/hmes98318/Music-Disc/releases) to download  


### Install the dependencies
auto install all dependencies on [`package.json`](./package.json)  
```
npm install
```

### Configure Files
[`.env`](./.env) 
```env
TOKEN = "your_token"
```

[`config.json`](./config.json)  
```json
{
    "name": "trifoiasii-Music",
    "prefix": "+",
    "playing": "+help | MusicBOT",
    "color": "#FFFFFF",
    "defaultVolume": 50,
    "maxVolume": 100,
    "autoLeave": true,
    "autoLeaveCooldown": 1000,
    "displayVoiceState": true,
    "port": 33333
}
```
**`autoLeave`** : After the music finished, can choose whether let the bot leave voice channel automatically or not.  
**`displayVoiceState`** : Show voice channel status updates.   

## Running the script 
```
node index.js
```


## Deploying with Docker Compose  
**image link** : https://hub.docker.com/r/hmes98318/music-disc  
### put your Token into [`docker-compose.yml`](./docker-compose.yml)
```yml
version: '3.8'
services:
  music-disc:
    image: hmes98318/music-disc:1.2.4
    container_name: music-disc
    restart: always
    environment:
      TOKEN: "MTA0NzE3MjQ2ODU1NDYwNDU4NA.GRDUIP.9N8UmRlr7hsUc1UeRiF_t-SNmwloY53IBiYvFk"
      PREFIX: "+"
      PLAYING: "+help | music"
      COLOR: "#FFFFFF"
      DEFAULTVOLUME: 50
      MAXVOLUME: 100
      AUTO_LEAVE: "true"
      DISPLAY_VOICE_STATE: "true"
    ports:
      - 33333:33333
```

### Start the container  
```
docker-compose up -d
```


## Deploying with Replit  
Watch it by clicking on the image down below  
[![Music-Disc-with-Replit](https://img.youtube.com/vi/WH5aSHIebcc/0.jpg)](https://youtu.be/WH5aSHIebcc)  


