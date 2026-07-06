# Juhised magnetofoni tööriistade kasutamiseks

Lühendid:

`MLOS` - mittejuhitav lindiop.süsteem  
`JLOS` - juhitav lindiop.süsteem  
`CP/M` - standardne kettaop.süsteem  
`BLOS` - baaslindiop.süsteem  

Programmid:

|              |                                                                       |
| ------------ | ---------------------------------------------------- |
| `FORM  .COM` | lindi formateerimine ja süsteemi salvestamine                         |
| `COPA  .COM` | kopeerimine `CP/M` -> `JLOS`, `JLOS` -> `CP/M` ja `CP/M` -> `CP/M`    |
| `COPM  .COM` | kopeerimine `CP/M` -> `MLOS`, `MLOS` -> `CP/M` ja `CP/M` -> `CP/M`<br>kui `JLOS`-i alt käivitatud,siis `JLOS` -> `MLOS` ja `MLOS` -> `JLOS` |
| `GENA  .COM` | JLOS-i genereerimine                                                  |
| `GENM  .COM` | MLOS-i genereerimine                                                  |
| `ATOS  .SYS` | juhitava lindi op.süsteem<br>(ei ole laademoodul)                     |
| `MTOS  .SYS` | mittejuhitava lindi op.süsteem<br>(ei ole laademoodul)                |
| `SETS  .COM` | failide staatuste kuvamiseks ja muutmiseks                            |

## `FORM.COM`

Programm JLOS-i lintide formateerimiseks ja süsteemi
kirjutamiseks. Võib käivitada op.süsteemides `CP/M`, `JLOS` , `MLOS`.

`FORMAT` - lindi formateerimine.

 - mitu plokki kirjutada? Kui vastus=0, siis peavad plokid olema
   juba varem kirjutatud.
 - mitu plokki lugeda? Lugema peab vähemalt 8 plokki.
 - kataloog kontrollida? Pärast kataloogi salvestamist lindile,
   teostatakse selle lugemine ning võrdlemine. Kui kontrollimisel
   on vigu,siis on võimalus kataloog uuesti salvestada lindile.
 - süsteem kirjutada? Kui käsuga `LOAD` on laetud op.süsteem,
   siis on kasutajal võimalus pärast formateerimist salvestada
   lindile ka süsteem.
 - süsteem kontrollida? Salvestatud süsteemi kontroll.

`SYSGEN` - lindile süsteemi kirjutamine.

 - kui süsteem on juba mällu laaditud, siis tuleb magnetofoni asetada
   lint,millele soovime süsteemi salvestada.
 - kui süsteem ei ole laaditud,tuleb kõigepealt süsteemselt lindilt
   lugeda süsteem, seejärel vahetada linti ning salvestada.

`LOAD` - laadida lindiopsüsteem ketta/lindifailist mällu.

 - juhitava magnetofoniga op.süsteem failis `ATOS.SYS`
 - mittejuhitava magnetofoniga op.süsteem failis `MTOS.SYS`

`EXIT` - väljumine programmist.

 * `Ctrl-ESC` viib alati programmi põhimenüüsse.
 * Selle programmiga võib teha ka `MLOS`-i süsteemseid linte:
    - formateerida lindist ainult 8 esimest plokki ja salvestada
      süsteem MLOS(fail `MTOS.SYS`).
 * Programmi võib käivitada ka op.süsteemis `MLOS`, ning seal
   formateerida linte ning kanda nendele süsteeme.
 * Kui programm on käivitatud op.süsteemis `JLOS`, siis väljumisel
   programmist tuleb magnetofonile asetada lint, mis oli avatud
   programmi käivitamisel.
   

## `COPA.COM`

Programm failide kopeerimiseks kettalt juhitavale lindile,
lindilt kettale ja kettalt kettale. Programm käivitatav ainult
op.süsteemis `CP/M`.

|               |                                                                       |
| ------------- | ---------------------------------------------------- |
| `O - (OPEN)`  | lindi kataloogi avamine. |
| `L - (CLOSE)` | lindi kataloogi sulgemine, kataloog jääb avatuks. |
| `D - (DIR)`   | ketta/lindikataloogi kuvamine.<br>`A...D` - kettaseade<br>`T`     - lint |
| `E - (EXIT)`  | väljumine programmist. Kui lint on avatud, siis toimub küsimine lindi sulgemise kohta. |
| `R - (RESET)` | lindi kerimine algusesse ja "reset" ketastele. |
| `C - (COPY)`  | failide kopeerimine. Esiteks sisestada lähtefaili nimi. Kui sellist faili ei leita,siis ilmub ekraanile vastav teade. Kui failinime ei sisestata, toimub pöördumine programmi põhimnüüsse. Järgmisena sisestada tulemusfaili nimi (võib sisestada ainult seadme tähise, nimi kantakse automaatselt üle lähtefailist). Kui selline fail juba eksisteerib, siis toimub küsimine faili ülekirjutamise kohta. Eitava vastuse korral tuleb failinimi uuesti sisestada. Jaatava vastuse korral kirjutatakse antud fail üle (ka siis, kui on staatusega `R/O`).<br>Failinimes võib kasutada järgmisi seadmete tähistusi:<br>`A...D` - kettaseade<br>`T`     - lint<br>Kui seadme tähis puudub,siis vaadeldakse vaikimisi olevat seadet. |



## `COPM.COM`

Programm failide kopeerimiseks kettalt mittejuhitavale
lindile,lindilt kettale ja kettalt kettale. Programm käivitatav
op.süsteemis `CP/M` ja oskuslikul kasutajal ka `JLOS`-s.Dialoog
tarbijaga analoogne programmiga `COPA.COM`.


## `GENA.COM`

Programm juhitava lindiop.süsteemi kirjutamiseks. Prog-
ramm käivitatav op.süsteemis `CP/M` ja `JLOS`.
 - asetada magnetofonile lähtelint (s.o. lint kus on süsteem).
 - kui süsteem on loetud,tuleb magnetofonile asetada lint,
   millele soovitakse süsteemi kirjutada.
 - NB! Programmist väljumisel op.süsteemis JLOS tuleb
   magnetofonile asetada lint, mis oli avatud programmi käivitamisel.
 - `Ctrl-ESC` viib alati juhtimise programmi tagasi.
 - `Ctrl-C` katkestab programmi töö.  
       

## `GENM.COM`

Programm mittejuhitava lindiop.süsteemi kirjutamiseks.
Programm käivitatav op.süsteemis `CP/M`, `JLOS` ja `MLOS`.

Programmidega `COPM.COM` ja `GENM.COM` töötamisel väljastatakse teateid:

|               |                                                                       |
| ------------- | ---------------------------------------------------- |
| `Set to Mtos`	| initsialiseerida mittejuhitav lindiop.süsteem s.t. magnetofoni juhtimiskaabel tuleb pesast `X4` eemaldada. |
| `Set to Atos` | initsialiseerida juhitav lindiop.süsteem s.t. magnetofoni juhtimiskaabel tuleb asetada pesasse `X4`.


## `SETS.COM`

Programm failide staatuste väljastamiseks ja muutmiseks.
Programm käivitatav op.süsteemis `CP/M` ja `JLOS`.
`JLOS`-s failide staatuste väljastamisel kuvatakse andmed
faili paiknemise kohta (algus- ja lõpp-plokk ning pikkus).

```
A>SETS [failinimi] [staatus]   
```

|           |                                                                       |
| --------- | ---------------------------------------------------- |
| staatuse: | `R/W` - fail lugemiseks ja kirjutamiseks<br>`R/O` - fail ainult lugemiseks<br>`DIR` - mittesüsteemne fail<br>`SYS` - süsteemne fail |


## JLOS-i funktsioonid

|                 |                                                      |
| --------------- | ---------------------------------------------------- |
| `DIR [f]`       | failide nimekirja väljastamine |
| `REN f1=f2`     | faili ümbernimetamine<br>`f1` - uus  nimi<br>`f2` - vana nimi |
| `ERA f`         | failide kustutamine |
| `REST f`        | kustutatud faili taastamine |
| `MEM`           | väljastatakse üldinfo lindi mäluhõive kohta |
| `TYPE f`        | tekstifaili kuvamine |
| `DUMP f`        | faili sisu kuvamine 16-süsteemis |
| `LOAD f [a]`    | faili laadimine muutmällu<br>`a` - algusaadress (vaikimisi 100H) |
| `RUN [p1] [p2]` | mällu laaditud programmi käivitamine, parameetrid salvestatakse faili juhtplokkidesse |
| `SAVE n f [a]`  | mälusisu salvestamine faili<br>`n` - 2K baidiste plokkide arv<br>`a` - algusaadress (vaikimisi 100H) |
| `CLOSE`         | kataloogi kirjutamine lindile |
|                 | (kataloog jääb avatuks) |
| `OPEN`          | kataloogi lugemine lindilt mällu |
| `MONID`         | väljumine op.süsteemist monitori |
| `HELP`          | residentsete funktsioonide loetelu |
| `CHECK`         | väljastab süsteemse info ja arvutatakse kataloogile uus kontrollsumma. |
| `DUMP ;a`       | muutmälu kuvamine 16-süsteemis<br>`a` - algusaadress |
| `SAVE ;a`       | muutmälu muutmine<br>`a` - algusaadress |

`Ctrl-C` katkestab funktsiooni täitmise


## Töötamine JLOS-ga

Töötamine juhitava lindiop.süsteemiga toimub
analoogselt standardse kettaop.süsteemiga `CP/M`.


## MLOS-i funktsioonid

|                 |                                                      |
| --------------- | ---------------------------------------------------- |
| `DIR`           | plokkide nimekirja väljastamine  |
| `TYPE f`        | tekstifaili kuvamine |
| `DUMP f`        | faili sisu kuvamine 16-süsteemis |
| `LOAD f [a]`    | faili laadimine muutmällu<br>`a` - algusaadress (vaikimisi 100H) |
| `BLOAD [a]`     | plokkide laadimine muutmällu<br>`a` - algusaadress |
| `RUN [p1] [p2]` | mällu laaditud programmi käivitamine, parameetrid salvestatakse faili juhtplokkidesse |
| `SAVE n f [a]`  | mälusisu salvestamine faili<br>`n` - 2K baidiste plokkide arv<br>`a` - algusaadress (vaikimisi 100H)  |
| `MONID`         | väljumine op.süsteemist monitori |
| `HELP`          | residentsete funktsioonide loetelu |
| `DUMP ;a`       | muutmälu kuvamine 16-süsteemis<br>`a` - algusaadress |
| `SAVE ;a`       | muutmälu muutmine<br>`a` - algusaadress |

`Ctrl-C` katkestab funktsiooni täitmise


## Töötamine MLOS-ga

Kui toimub faili otsimine (`LOAD`, `TYPE`, `DUMP` või
laademooduli käivitamisel), siis väljastatakse nende
plokkide päised,mis antud faili ei kuulu.

Kui tarbijaprogrammis kasutatakse `BLOS`-i
funktsioone nr. 17 (otsida faili) või nr. 18 (otsida
järgmist faili), siis ekraani esimesele reale väljas tatakse küsimus:

> `FILE EXIST(Y/N)` (Kas fail olemas?)

Jaatava vastuse korral eeldatakse, et otsitava
nimega fail on juba lindil olemas.

Funktsioonide nr. 20 (lugeda 128-baidine plokk)
või nr. 42 (lugeda 2K-baidine plokk) käivitamisel
väljastatakse ekraani esimesele reale mõneks sekundiks
vilkuv tekst: `SWITCH TO READING`
s.t. magnetofon tuleb lülitada lugemise režiimi.

Kui lindilt lugemise ajal väljastatakse veateade: `CHECKSUM ERROR`,
siis antud ploki lugemise kordamisel,tuleb linti 
veidike tagasi kerida ja korrata lugemist.

Funktsioonide nr. 21 (kirjutada 128-baidine
plokk) või nr.43 (kirjutada 2K-baidine plokk) käivitamisel
väljastatakse ekraani esimesele reale mõneks
sekundiks vilkuv tekst: `SWITCH TO RECORDING`
s.t. magnetofon tuleb lülitada kirjutamise režiimi.

Kui ekraani esimesele reale väljastatakse
vilkuv tekst: `STOP THE TAPE`, siis tuleb lint peatada.


`DIR` - Väljastatakse 2K baidiste plokkide päis:

> `n` `nimi` `m`

|        |                                       |
| ------ | ------------------------------------- |
| `n`    | ploki number |
| `nimi` | failinimi |
| `m`    | faili algusploki number  |
 
Kui loetakse juhitavat linti, siis

|        |                                       |
| ------ | ------------------------------------- |
| `n`    | absoluutne ploki number |
| `nimi` | failinimi, kui see plokk kuulub faili lindinimi, kui tühi plokk |
| `m`    | kui plokk faili ei kuulu, siis 0<br>kui plokk kuulub faili, siis faili esimese ploki number |
   
Kui loetakse mittejuhitavat linti, siis

|        |                                       |
| ------ | ------------------------------------- |
| `n`    | ploki jrk.number failis (0-st alates) |
| `nimi` | failinimi |
| `m`    | alati 0 |
 
Kui linti on loetud 1,5 minutit ja selle aja jooksul
pole leitud ühtegi ploki päist, siis väljastatakse
veateade: `TIME OUT` s.t. et tegemist on tühja lindiga

## Magnetofoni ühendamine

Magnetofoni ühendamiseks arvutiga on komplektis vastav kaabel.
Juhitava magnetofoni olemasolul kasutatakse
arvuti pistukupesasid `X5` ja `X4` vastavalt andmesideks
magnetofoniga ja magnetofoni juhtimiseks. Magnetofon
ei tohi olla ajutise peatamise režiimis.
Mittejuhitava magnetofoni kasutamisel tuleb
kaabel pistikupesast `X4` eemaldada.

