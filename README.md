# Překlad CMI & CMILib
Český překlad pluginů CMILib a CMI.  
> Pro verzi pluginu CMI: **9.2.3.7**  
> Pro verzi pluginu CMILib: **1.2.3.5**  
  
> Status překladu CMI: **0%**  
> Status překladu CMILib: **75%**

## Formát
Následující formát bude používán po celou dobu překládání.  
Díky použití širokého rozčlenění barev, je tento překlad univerzální a přizpůsobitelný.  
Značky si lze po stažení dle libosti nahradit za barevné kódy, dle vlastního výběru.

### Tabulka
| Druh textu | Tag | Popis |
| --- | :---: | :--- |
| Neutrální Text | `<t>` | Obyčejný text |
| Úspěšný Text | `<ts>` | Text, který značí úspěch. |
| Neúspěšný Text | `<tf>` | Text, který značí neúspěch. |
| Speciální Text | `<tspecial>` | GUI, ActionBar, Hover zprávy, apod. |
| Neutrální Proměnná | `<var>` | Proměnné, počet a název itemů, jména hráčů, apod. |
| Kladná Proměnná | `<vars>` | Přičtění peněz, online status hráče,... |
| Záporná Proměnná | `<varf>` | Odečtení peněz, offline status hráče,... |
| Oddělovač | `<splitter>` | Pouze pro oddělovače textu, nadpisu, atp.|
| Nadpis oddělovače | `<splitterh>` | Pouze pro nadpisy oddělovače textu | 
| Ostatní | `<misc>` | Závorky v textu. |

### Komentáře
Je normální, že si občas nevzpomenete, jak vlastně máte přeložit některé fráze. Proto v průběhu celého překladu používáme komentáře. Ty jsou:
> **INFO** - Důležitá informace na kterou si nemusíte příště vzpomenout. Radši si všechno zapište. Komentáře jsou především pro nás, překladatele. 
   
> **TODO** - Tímto komentářem značíte, že je na daném řádku ještě potřeba něco dodělat. Např. Barvy (resp. Tagy), překlad, atp.
   
> **Uživatel** - Toto je především pro lidi co použijí náš překlad. Překlad nemůže být 100% univerzální a uživatel si pak bude muset donastavit detaily. Perfektní případ použití je na řádku s prefixem, který se používá v celém překladu.

### Prefix
Prefix je již definován v souboru [CMILib/Translations/Locale_CZ.yml](CMILib/Translations/Locale_CZ.yml)<br/>
Zprávám, které jej mají používat stačí na začátek vložit tuto proměnnou: `!prefix!`

### Příklady formátu
```
!prefix! <t>Použití: <var>%usage%<br/> #INFO - Takto se používá komentář INFO.  
!prefix! <tf>Nemůžeš se teleportovat na hráče, který není online! #TODO - Zde je potřeba něco udělat, proto je zde komentář TODO.  
!prefix! <ts>Úspěšně jsi zakoupil/a <var>%quantity%x %item%<ts>! <misc>(<varf>- %price% $<misc>) #Uživatel - Zde si může uživatel něco nastavit.  
!prefix! <ts>Úspěšně jsi prodal/a <var>%quantity%x item<ts>! <misc>(<vars>+ %price% $<misc>)  
!prefix! <ts>Gamemode cílového hráče byl změněn na <var>%gamemode%<ts>! <misc>(<var>%player% │ %status%<misc>)
```
Komentáře v příkladech formátu jsou pouze informativního charakteru, jak je vlastně použít.  
**POZOR! U posledního příkladu není barevné označení u proměnné %status%! Barevnost stavu Offline a Online je potřeba definovat v souboru překladu CMILib. Podobných vyjímek se v překladu může nacházet několik.**

## Instalace překladu
> Je potřeba vypracovat.

## Závěrečná slova
Děkujeme za používání našeho překladu.
Překlad za žádnou cenu není perfektní, a proto potřebujeme přímo Vás. Najdete-li jakoukoliv chybu v překladu, tak je nejvhodnější otevřít problém (Issue) zde na GitHubu a nebo se nám ozvat na [Discordu (odkaz)](https://discord.gg/2w2mZyDvWz). Zde také najdete naše další překlady a máte možnost přímého spojení s překladateli.  
Jsi spokojený s naší prací? Podpoř nás finančně na [Patreonu (odkaz)](https://example.com/) pro exkluzivní výhody.
