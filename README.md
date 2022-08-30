# CMI překlad
Český překlad pluginů CMILib a CMI.

## Formát
Následující formát bude používán po celou dobu překládání.<br/>
Nejen barevné kódy, ale i některé celé části, si lze po stažení dle libosti upravit, pomocí funkce nahrazování.<br/>
Díky použití širokého rozčlenění barev, je tento překlad univerzální a přizpůsobitelný.

### Prefix
Prefix je již definován v souboru [CMILib/Translations/Locale_CZ.yml](CMILib/Translations/Locale_CZ.yml)<br/>
Zprávám, které jej mají používat stačí na začátek vložit tuto proměnnou:
> !prefix!

### Prostý text

#### Neutrální
> &b

#### Úspěch
> &a

#### Neúspěch
> &c

### Proměnné

#### Neutrální
Použití příkazů, počet a název itemů, jména hráčů,...
> &3

#### Kladné
Přičtení peněz po prodeji, online status hráče,...
> &2

#### Záporné
Odečtení peněz po nákupu, offline status hráče,...
> &4

### Závorky
Použití závorek se týká hlavně proměnných, nacházejících se uprostřed vět.
> &8

## Příklady formátu
> !prefix! &bPoužití: &3%usage%<br/>
> !prefix! &cNemůžeš se teleportovat na hráče, který není online!<br/>
> !prefix! &aÚspěšně jsi zakoupil/a &3%quantity%x %item%&a! &8(&4- %price% $&8)<br/>
> !prefix! &aÚspěšně jsi prodal/a &3%quantity%x item&a! &8(&2+ %price% $&8)<br/>
> !prefix! &aGamemode cílového hráče byl změněn na &3%gamemode%&a! &8(&3%player% │ %status%&8)<br/>

*** POZOR! U posledního příkladu není barevné označení u proměnné %status%! Barevnost stavu Offline a Online je již definována v pluginu CMILib. Podobných vyjímek se v překladu může nacházet několik. ***
