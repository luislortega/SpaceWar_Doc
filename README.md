# SpaceWar | MMO of space action

This is a totally private project, the copyright of this code belongs to GG Studios, some assets and UI concepts belong to the BigPoint company, for now it is a non-profit project.

**Mission:** recreate a version of darkorbit based on 2009.

**Vision:** Create a new game concept based on DO, but with a plot twist in terms of events, community and teamwork, taking all the good of DO to create a solid community

## Technologie stack

**Frontend:** Vue.JS (HTML5, JavaScript, CSS)

**Game client:** GDScript

**Backend:** GoLang

**Database:** MySql

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

It will contain all the functionality of darkorbit 2009, except skylab, clans, auctions, general account settings, refinement of lasers or generators, bonus page, page to buy uridium, missions, without cubikones / npc with unique characteristics.

**Conceptual UI**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_1.jpg" width="500">

player_id: int auto incrementable

session_id: default null y el valor es generado por JWT

info: la ultima ip que al inicio es la misma ip de registro y la fecha de registo

server_id: default 1

username: default null

password: default null y debe estar encriptado por MD5

email: default null

data: default {"uridium":0,"credits":0,"honor":0,"experience":0,"jackpot":0}

config default 1

health default 0

shield default {"firstConf":0, "secondConfg":0}



<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_2.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_3.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_4.jpg" width="500">

**Class modeling**

To-do

**Database modeling**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_5.jpg" width="500">

**Database example data**

<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_6.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_7.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_8.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_9.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_10.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_11.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_12.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_13.jpg" width="500">
<img src="https://raw.githubusercontent.com/luislortega/SpaceWar_Doc/main/screenshots/v003/Screenshot_14.jpg" width="500">


**Socket architecture**

To-do

**API architecture**

To-do