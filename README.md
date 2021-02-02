# SYBGA: Ein "Reversi"-Tutorial für BGA
(Quelle:: https://boardgamearena.com/doc/Tutorial_reversi)

https://github.com/geziefer/sybga
-> checkout tags Tutorial_Step_X

Tutorial_Step_0: Template
- sybga:   Projekttemplate mit TODOs und Examples

Tutorial_Step_1: Board
- img:	   Board und Token Grafik
- tpl:     div mit Block für Squares mit Platzhaltern
- view:    64x Block mit Square füllen
- css:     Board als Hintergrund, relativ; 
           Square darauf, absoute 
-> F5, Squares mit F12

Tutorial_Step_2: Token-Platzierung
- tpl:     div mit Token; HTML-Fragment für Token
- css:     Token als CSS Sprite
- game:    Colors setzen in setup
- js:      Function für Token-Platzierung mit Dojo-Animation in utility section;
           Token-Testplatzierung in setup
-> F5

Tutorial_Step_3: Datenmodell
- db:      Datenmodell Board
- game:    Tabelle füllen mit NULLs und 4 Token in setup;
           Token laden in getAllDatas
- js:      Tokens platzieren gemäß DB in setup
-> Neustart Spiel

Tutorial_Step_4: State Machine und Game Logik
- states:  Zustandsmaschine, 2 neue States mit Translation
- game:    Function für player args in game state arguments section;
           Function für possible moves mit dojo css Änderung in utility section;
           Function für get board in utility section;
           Function für turned over discs in utility section;
           Function für next player Action in game state action section
-> F5

Tutorial_Step_5: Zugmöglichkeiten
- js:      Aufruf update possible moves in onEnteringState;
           Function für update possible moves in utility section
- css:     Highlight possible moves Felder
-> F5

Tutorial_Step_6: Zug ausführen
- js:     onclick Callback für Square mit Dojo;
          Function für play disc in player action section
- action: Function für client action play disc
- game:   Function für play disc in player action section
-> F5 in beiden Browsern

Tutorial_Step_7: Animation
- js:     Notification Callbacks mit Dojo in setupNotifications;
          Function für play disc notification für neues Token auf Board;
          Function für turn over discs notification für tun over Animation mit Dojo;
          Function für new scores notification für Score Update
-> F5

