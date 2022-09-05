# CMI překlad
Český překlad pluginů CMILib a CMI.

## Formát
Následující formát bude používán po celou dobu překládání.<br/>
Díky použití širokého rozčlenění barev, je tento překlad univerzální a přizpůsobitelný.<br/>
Značky si lze po stažení dle libosti nahradit za barevné kódy, dle vlastního výběru.

### Tabulka
| Druh textu | Tag |
| --- | :---: |
| Neutrální Text | `<t>` |
| Úspěšný Text | `<ts>` |
| Neúspěšný Text | `<tf>` |
| Speciální Text | `<tspecial>` |
| Neutrální Proměnná | `<var>` |
| Kladná Proměnná | `<vars>` |
| Záporná Proměnná | `<varf>` |
| Ostatní (závorky) | `<misc>` |   

### Prefix
Prefix je již definován v souboru [CMILib/Translations/Locale_CZ.yml](CMILib/Translations/Locale_CZ.yml)<br/>
Zprávám, které jej mají používat stačí na začátek vložit tuto proměnnou:
> !prefix!

### Prostý text

#### Neutrální
> \<t>

#### Úspěch
> \<ts>

#### Neúspěch
> \<tf>

#### Speciální
Zprávy v GUI, progressbary, hover zprávy, actionbar zprávy, apod.
> \<tspecial>

### Proměnné

#### Neutrální
Použití příkazů, počet a název itemů, jména hráčů,...
> \<var>

#### Kladné
Přičtení peněz po prodeji, online status hráče,...
> \<vars>

#### Záporné
Odečtení peněz po nákupu, offline status hráče,...
> \<varf>

### Závorky
Použití závorek se týká hlavně proměnných, nacházejících se uprostřed vět.
> \<misc>

## Příklady formátu
> !prefix! \<t>Použití: \<var>%usage%<br/>
> !prefix! \<tf>Nemůžeš se teleportovat na hráče, který není online!<br/>
> !prefix! \<ts>Úspěšně jsi zakoupil/a \<var>%quantity%x %item%\<ts>! \<misc>(\<varf>- %price% $\<misc>)<br/>
> !prefix! \<ts>Úspěšně jsi prodal/a \<var>%quantity%x item\<ts>! \<misc>(\<vars>+ %price% $\<misc>)<br/>
> !prefix! \<ts>Gamemode cílového hráče byl změněn na \<var>%gamemode%\<ts>! \<misc>(\<var>%player% │ %status%\<misc>)<br/>

*** POZOR! U posledního příkladu není barevné označení u proměnné %status%! Barevnost stavu Offline a Online je potřeba definovat v souboru překladu CMILib. Podobných vyjímek se v překladu může nacházet několik. ***
