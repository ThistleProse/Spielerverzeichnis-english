NOTE: This is a simple Google translate, so that my dumb English-only butt can use this Plugin. I cannot provide any support or updates. Please see the primary source for such things <3

# Spielerverzeichnis & Statistiken
This plugin creates an overview of players and their associated accounts—a so-called "Who's Who" list. In addition to this list, there are personal player statistics and character statistics. These statistics pages display a wide variety of information and statistical values ​​for the player or character.<br>
In addition to the pre-made statistics and charts, you can also create your own statistics for the player statistics page in the ACP. For example, you can create statistics on how many male, female, or non-binary characters a user has. More detailed information about the settings, options, and custom statistics can be found in the [Wiki](https://github.com/little-evil-genius/Spielerverzeichnis/wiki).<br>
<br>
If this plugin is too complex and extensive for you, you can use the  [Who's Who? 1.1 - Plugin](https://storming-gates.de/showthread.php?tid=19354&pid=135895#pid135895) by [melancholia](https://storming-gates.de/member.php?action=profile&uid=112). Alternatively, you can integrate the tutorial [ Player Overview with Statistics - Storming Gates](https://storming-gates.de/showthread.php?tid=1015591&pid=480982#pid480982) | [ Player Overview with Statistics - Epic](https://epic.quodvide.de/showthread.php?tid=1109&pid=5112#pid5112) by [sparks fly](https://epic.quodvide.de/member.php?action=profile&uid=10). If you're interested in charts, you can, like me, create them using the open-source solution [Chart.js](https://www.chartjs.org/) or watch the tutorial [Charts mit Hilfe von Googles Developer erstellen](https://storming-gates.de/showthread.php?tid=1017740&pid=495004#pid495004) by [Ales](https://storming-gates.de/member.php?action=profile&uid=279).<br>
<br>
<b>Notice:</b><br>
The plugin is compatible with the classic profile fields of MyBB and/or the <a href="https://github.com/katjalennartz/application_ucp">profile plugin from Risuena</a>.<br>
he plugin is also compatible with various in-play trackers/scene trackers: with the <a href="https://github.com/its-sparks-fly/Inplaytracker-2.0">Inplaytracker 2.0 von sparks fly</a>, the successor <a href="https://github.com/ItsSparksFly/mybb-inplaytracker">Inplaytracker 3.0 by sparks fly</a>, the <a href="https://github.com/little-evil-genius/Inplayszenen-Manager">my Inplay Scene Manager (little.evil.genius)</a>, the <a href="https://storming-gates.de/showthread.php?tid=1023729&pid=537783#pid537783">Scene Tracker by Risuena</a>, the <a href="https://github.com/Ales12/inplaytracker">Inplaytracker 1.0 by Ales</a> and the successor <a href="https://github.com/Ales12/inplaytracker-2.0">Inplaytracker 2.0 by Ales</a>.<br>
Similarly, the list menu can also be displayed when using the <a href="https://github.com/ItsSparksFly/mybb-lists"> Sparks Fly automatic list plugin</a>. Both simply need to be configured beforehand. 

# Prerequisite
- The ACP module <a href="https://github.com/little-evil-genius/rpgstuff_modul" target="_blank">RPG Stuff</a> <b>must</b>  be present.
- The <a href="https://doylecc.altervista.org/bb/downloads.php?dlid=26&cat=2" target="_blank">Accountswitcher</a> von doylecc <b>muss</b> installiert sein. <br>
- Für eine Ausgabe von einem zufälligen Inplayzitat wird das <a href="https://github.com/its-sparks-fly/Inplayzitate-2.0"> Inplayzitate 2.0</a> oder <a href="https://github.com/ItsSparksFly/mybb-inplayquotes">Inplayzitate 3.0</a> Plugin von sparks fly oder <a href="https://github.com/Ales12/inplayquotes">Inplayzitate</a> Plugin von Ales oder die <a href="https://github.com/little-evil-genius/inplayzitate">Inplayzitate</a> von mir (little.evil.genius) verwendet. Wenn man diese Option nicht möchte, muss keines der Plugins installiert sein.

# Datenbank-Änderungen
### hinzugefügte Tabelle:
* PRÄFIX_playerdirectory_statistics

### hinzugefügte Spalten in der DB-Tabelle PRÄFIX_users:
* playerdirectory_playerstat
* playerdirectory_playerstat_guest
* playerdirectory_characterstat
* playerdirectory_characterstat_guest

# Neue Sprachdateien
- deutsch_du/admin/playerdirectory.lang.php
- deutsch_du/playerdirectory.lang.php

# Einstellungen - Spielerverzeichnis und Statistiken
- Spielerverzeichnis aktivieren
- Gästeberechtigung
- Spieleranzahl pro Seite
- Ausgeschlossene Accounts
- Spieler-Statistik aktivieren
- Gästeberechtigung
- Charakter-Statistik aktivieren
- Gästeberechtigung
- Profilfeldsystem
- Spielername
- Standard-Avatar
- Avatar verstecken
- Geburtstage der Charaktere
- Geburtstagsfeld
- Letzter Inplaytag
- Feld fürs Alter
- Inplaytracker
- letzte 12 Monate-Statistik
- Szenenanzahl pro Charakter - Statistik
- Szenenanzahl-Statistik - Legende
- Inplaypostanzahl pro Charakter - Statistik
- Inplaypostanzahl-Statistik - Legende
- Farben für die Säulen/Kreisflächen
- Inplayzitate
- Listen PHP
- Listen Menü Template
<br><br>
<b>HINWEIS:</b><br>
Einige Einstellungen sind abhängig voneinander und werden nur angezeigt, wenn bei einer anderen Einstellung Option 1 oder 2 ausgewählt wurde.

# Neue Template-Gruppe innerhalb der Design-Templates
- Spielerverzeichnis und Statistiken

# Neue Templates (nicht global!)
- playerdirectory_characterstat
- playerdirectory_characterstat_inplayquote
- playerdirectory_directory
- playerdirectory_directory_characters
- playerdirectory_directory_user
- playerdirectory_menu_link
- playerdirectory_notice_banner
- playerdirectory_playerstat
- playerdirectory_playerstat_characters
- playerdirectory_playerstat_inplayquote
- playerdirectory_playerstat_ownstat
- playerdirectory_playerstat_ownstat_bar
- playerdirectory_playerstat_ownstat_bit
- playerdirectory_playerstat_ownstat_pie
- playerdirectory_postactivity_months
- playerdirectory_postactivity_months_bit
- playerdirectory_postactivity_months_chart
- playerdirectory_postactivity_perChara
- playerdirectory_postactivity_perChara_poststat
- playerdirectory_postactivity_perChara_poststat_bit
- playerdirectory_postactivity_perChara_poststat_chart_bar
- playerdirectory_postactivity_perChara_poststat_chart_pie
- playerdirectory_postactivity_perChara_scenestat
- playerdirectory_postactivity_perChara_scenestat_bit
- playerdirectory_postactivity_perChara_scenestat_chart_bar
- playerdirectory_postactivity_perChara_scenestat_chart_pie
- playerdirectory_usercp_options
- playerdirectory_usercp_options_bit<br><br>
<b>HINWEIS:</b><br>
Alle Templates wurden größtenteils ohne Tabellen-Struktur gecodet. Das Layout wurde auf ein MyBB Default Design angepasst.

# Template Änderungen - neue Variablen
- header - {$menu_playerdirectory}
- usercp_options - {$playerdirectory_options}

# Neues CSS - playerdirectory.css
Es wird automatisch in jedes bestehende und neue Design hinzugefügt. Man sollte es einfach einmal abspeichern - auch im Default. Nach einem MyBB Upgrade fehlt der Stylesheets im Masterstyle? Im ACP Modul "RPG Erweiterungen" befindet sich der Menüpunkt "Stylesheets überprüfen" und kann von hinterlegten Plugins den Stylesheet wieder hinzufügen.

# Links
- euerforum.de/admin/index.php?module=rpgstuff-playerdirectory
- euerforum.de/misc.php?action=playerdirectory
- euerforum.de/misc.php?action=playerstatistic&uid=X
- euerforum.de/misc.php?action=characterstatistic&uid=X

# Demo Screenshots
### Spielerverzeichnis
<img src="https://stormborn.at/plugins/spielerverzeichnis_main.png">

### Spielerverzeichnis/Statistik
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_inplay.png">
<br><br>
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_character.png">

### die letzten 12 Monate
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_12monts_bar.png">
<br><br>
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_12monts.png">

### Szenen/Inplaypost pro Charakter
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_perChara_pie.png">

<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_perChara_bar.png">

<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_perChara.png">

<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_perChara_beides.png">

### Charakterverzeichnis/Charakterstatistik
<img src="https://stormborn.at/plugins/spielerverzeichnis_character.png">

### Einstellungen & Hinweis
<img src="https://stormborn.at/plugins/spielerverzeichnis_ucp.png">

<img src="https://stormborn.at/plugins/spielerverzeichnis_notice.png">

## Eigene Statistiken
### Übersicht
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_own_acp.png">

### Hinzufügen
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_own_acp_add.png">

### Spielerstatistik
<img src="https://stormborn.at/plugins/spielerverzeichnis_spieler_own.png">
