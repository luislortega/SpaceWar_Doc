# SpaceWar | MMO of space action

This is a totally private project, the copyright of this code belongs to GG Studios, some assets and UI concepts belong to the BigPoint company, for now it is a non-profit project.

Special thanks to **s3kglitches** (YouTube) who provided me with many sprites from 2009, **TexterDo1** (GitHub) which provided me with the initial tools with the DeathSpaces 3D emulators, **ooscargerman** (GitHub) which gave me a lot of knowledge in cyber security for cloud servers, BotNet and DDoS attacks and how to protect myself from them.

**Mission:** recreate a version of darkorbit based on 2009.

**Vision:** Create a new game concept based on DO, but with a plot twist in terms of events, community and teamwork, taking all the good of DO to create a solid community

## Technologie stack

**Frontend:** Vue.JS (HTML5, JavaScript, CSS)

**Game client:** GDScript

**Backend:** GoLang

**Database:** MySql

## Documentation tools

To-do...

## Naming conventions

**Frontend:**

[VueJS official](https://vuejs.org/v2/style-guide/)

[JavaScript AirBnB](https://github.com/airbnb/javascript)

[CSS BEM](http://getbem.com/naming/)

**Game client:** 

[GDScript official](https://docs.godotengine.org/es/stable/getting_started/scripting/gdscript/gdscript_styleguide.html)

**Backend:**

[GoLang official](https://www.golangprograms.com/naming-conventions-for-golang-functions.html)

**Database:**

[MySql linux](https://anandarajpandey.com/2015/05/10/mysql-naming-coding-conventions-tips-on-mysql-database/)

## Version log

### => v.0.0.1

Basic multiplayer, simply ships shown and can attack each other, with a semi-functional chat

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v001/Screenshot_1.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v001/Screenshot_2.jpg" width="500">

### => v.0.0.2

Improvements in attacks, types of attacks, movements and better abstraction, it does not contain a connected database or functional socket.

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v002/Screenshot_1.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v002/Screenshot_2.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v002/Screenshot_3.jpg" width="500">


### => v.0.0.3 (In development)

It will contain all the functionality of darkorbit 2009, except skylab, clans, auctions, general account settings, refinement of lasers or generators, bonus page, page to buy uridium, missions, without cubikones / npc with unique characteristics, only low maps will be available.

**Conceptual UI**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_1.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_2.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_3.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_4.jpg" width="500">

**Available maps**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_15.jpg" width="500">

**Class modeling**

To-do...

**Database modeling**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_5.jpg" width="500">

**Database example data**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_6.jpg" width="500">

player_id: int | auto increment

session_id: default null | value auto generated by JWT

info: The last IP that at the beginning is the same IP of registration and the date of registration

server_id: default 1

username: default null

password: default null | encrypted by MD5

email: default null

data: default {"uridium":0,"credits":0,"honor":0,"experience":0,"jackpot":0}

current_config default 1

health default 0

shield default {"firstConf":0, "secondConfg":0}

position: default {"x": 0, "y": 0} | change depending the faction

map_id default 0 | change depending the faction

ship_id default 1

booty_key default 0 

premium default {"active":false,"date":null}

titles default []

faction_id | change depending the faction

clan_id default 0

rank_id default 1

rank_points default 0

rank default 0

extra_energy default 0

gate_rings default 0

old_pilot_name default []


<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_7.jpg" width="500">

player_id int

config_lasers default [[],[]] => el numero es basado en la posicion de items en esta misma tabla

config_generators default [[],[]] => el numero es basado en la posicion de items en esta misma tabla

config_drones default [[],[]] => el numero es basado en la posicion de items en esta misma tabla

config_extras default [[],[]] => el numero es basado en la posicion de items en esta misma tabla

items default {"lf1Count":0, "lf2Count":0, "lf3Count": 0, "mp1Count":0,"a01Count":0, "a02Count":0, "bO1Count":0, "bO2Count":0, "1010Count":0, "2010Count":0, "3210Count":0, "3310Count":0, "6900Count":0, "7900Count":0, "geminex":0, "sl01Cpu":0, "sl02Cpu":0, "sl03Cpu":0, "clo4kCpu10":0, "clo4kCpu50":0, "rep1":0, "rep2":0, "rep3": 0, "rep4": 0, "rokt01":0, "ncrrbCpu":0, "sm01Cpu":0, "ish01Cpu":0, "rllb1Cpu":0, "hm7":0, ships":[], "designs":[], "skillTree":{"logdisks":0,"researchPoints":0,"resetCount":0}}

cargo default {"Prometium":0, "Endorium":0, "Terbium":0, "Prometid":0, "Duranium":0, "Xenomita":0, "Promerium":0, "Seprom":0}

ammo default {"lcb10":0,"mcb25":0,"mcb50":0,"mcb100":0,"rsb75":0,"sab50":0,  "r310":0,"plt2026":0,"plt2021":0,"acm1":0,"eco10":0,"pem01":0}

skill_points defualt {"engineering":0,"shieldEngineering":0,"detonation1":0,"detonation2":0,"heatseekingMissiles":0, "rocketFusion":0,"cruelty1":0,"cruelty2":0,"explosives":0,"luck1":0,"luck2":0}

base_modules default []

boosters default {}

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_8.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_9.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_10.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_11.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_12.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_13.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_14.jpg" width="500">


**Socket architecture**

To-do...

**API architecture**

To-do...