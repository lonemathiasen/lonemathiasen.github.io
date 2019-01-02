---
layout: default
title: Markdown
description: Markdown guide
---

Dette er en guide til Markdown. Det er tiltænkt som et opslagsværk, så man hurtigt kan se hvilke kommandoer man kan bruge til at få forskellige styles. Guiden er inspireret af dette [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Alle eksempler vil indeholde et eksempel på det man skal skrive og efterfølgende vise hvordan resultatet kommer til at se ud. For eksempel således:
```md
Dette vil være eksempel kode
```
Her vil der vises hvordan det rent faktisk vil se ud på hjemmesiden.

---

## Normal tekst og linjeskift
Hvis man bare skriver tekst, bliver det blot sat ind på hjemmesiden som det står. Ganske lige til. Hvis man laver et enkelt linjeskift har det ingen indflydelse.
Hvis man gerne vil lave et enkelt linjeskift, gør man det ved at slutte en linje med en backslash (`\`), eller med to mellemrum.
Hvis man derimod laver et dobbelt linjeskift, (så der kommer en tom linje) får man en ny paragraf. Dette ser således ud:
```md
Her er noget tekst.
Her er der lavet et enkelt linjeskift hvilket ikke gør noget

Her er et dobbelt linjeskift, derfor bliver dette til en ny paragraf\
Forrige linje slutter med backslash, derfor kommer der et linjeskift.  
Forrige linje slutter med to mellemrum, derfor kommer der også her et linjeskift.
```
Her er noget tekst.
Her er der lavet et enkelt linjeskift hvilket ikke gør noget

Her er et dobbelt linjeskift, derfor bliver dette til en ny paragraf\
Forrige linje slutter med backslash, derfor kommer der et linjeskift.  
Forrige linje slutter med to mellemrum, derfor kommer der også her et linjeskift.

## Overskrifter
Man laver overskrifter ved at starte en linje med et hashtag. Jo flere hashtag der sættes jo mindre bliver overskriften, så det er altså nemt at lave underoverskrifter. Dette ser således ud:
```md
# Stor overskrift
## Mellemstor overskrift
### Lille overskrift
#### Meget lille overskirft
```
# Stor overskrift
## Mellemstor overskrift
### Lille overskrift
#### Meget lille overskirft

Bemærk, at de ovenstående oversættes til h1, h2, h3, h4, osv. HTML tags. Det er altså muligt at style dem i CSS, hvis de skal fremgå anderledes.

---

## Fremhævning
Man kan fremhæve tekst på forskellige måder. Både *kursiv*, **fed** og ~~gennemstreget~~ tekst er muligt. Dette gøres således:
```md
Man fremhæver med *kursiv skrift* ved at sætte stjerner omkring (`*`)  
For **fed skrift** sættes der dobbelte stjerner omkring (`**`)  
~~Overstreget skrift~~ laved ved at sætte dobbelte tilder omkring (`~~`)
```
Man fremhæver med *kursiv skrift* ved at sætte stjerner omkring (`*`)  
For **fed skrift** sættes der dobbelte stjerner omkring (`**`)  
~~Overstreget skrift~~ laved ved at sætte dobbelte tilder omkring (`~~`)

---

## Lister
Hvis man vil lave en liste af ting, kan det enten være en ordnet liste (med tal) eller en uordnet liste (med prikker). De laves således:
```md
En uordnet liste laves med stjerner:
* Dette er første ting
* Her er anden ting
  * Man kan også lave underpunkter ved blot at rykke dem længere ind med mellemrum
  * Endnu et underpunkt
* Og her er det sidste punkt.

For at lave en ordnet liste bruger man tal således:
1. Dette er første ting på listen
2. Anden ting på listen
   1. Her er en underliste, igen lavet ved at rykke tallene ind med mellemrum
   2. Anden ting på underlisten
   3. Tredje ting på underlisten
   4. Der er mange ting her...
3. Og så er vi væk fra underlisten igen
1. I virkeligheden betyder tallene foran ikke noget
1. Jekyll skal nok sørge for at de bliver fortløbende på hjemmesiden
1. Selvom jeg bliver ved med at skrive `1.` forrest.
```
En uordnet liste laves med stjerner:
* Dette er første ting
* Her er anden ting
  * Man kan også lave underpunkter ved blot at rykke dem længere ind med mellemrum
  * Endnu et underpunkt
* Og her er det sidste punkt.

For at lave en ordnet liste bruger man tal således:
1. Dette er første ting på listen
2. Anden ting på listen
   1. Her er en underliste, igen lavet ved at rykke tallene ind med mellemrum
   2. Anden ting på underlisten
   3. Tredje ting på underlisten
   4. Der er mange ting her...
3. Og så er vi væk fra underlisten igen
1. I virkeligheden betyder tallene foran ikke noget
1. Jekyll skal nok sørge for at de bliver fortløbende på hjemmesiden
1. Selvom jeg bliver ved med at skrive `1.` forrest.

---

## Links
Der er to måder at lave links på. Man kan enten skrive adressen man vil linke til samme sted, eller man kan lave en reference til den og skrive den et andet sted i dokumentet for at gøre det mere letlæseligt. Det ser således ud:

```md
Hvis man gerne vil linke til en anden hjemmeside, kan man gøre det [således](http://google.com)  
Man kan også linke til en relativ side på ens egen hjemmeside [sådan her](index.html)  
Hvis man vil lave en link reference, skriver man blot [teksten][referencen]  
Og så skal man huske, at man et eller andet andet sted på siden skal fortælle hvad referencen betyder  
Men det kan godt være flere linjer senere. 

Man kan også blot skrive en url, fx. http://google.com. Det vil også blive kompilet til et link på siden.  
Og her kommer referencen fra højere oppe:

[referencen]: http://google.com
```
Hvis man gerne vil linke til en anden hjemmeside, kan man gøre det [således](http://google.com)  
Man kan også linke til en relativ side på ens egen hjemmeside [sådan her](index.html)  
Hvis man vil lave en link reference, skriver man blot [teksten][referencen]  
Og så skal man huske, at man et eller andet andet sted på siden skal fortælle hvad referencen betyder  
Men det kan godt være flere linjer senere. 

Man kan også blot skrive en url, fx. http://google.com. Det vil også blive kompilet til et link på siden.  
Og her kommer referencen fra højere oppe:

[referencen]: http://google.com

---

## Billeder
Indsættelse af billeder virker på samme måde som indsættelse af links. Man kan enten specificere hvor billedet er med det samme, eller referere det fra et andet sted.

```md
Indsættelse af billede inline: ![beskrivelse](/assets/markdown.svg)  
Indsættelse med reference: ![beskrivelse][markdown-logo]

[markdown-logo]: /assets/markdown.svg
```
Indsættelse af billede inline: ![beskrivelse](/assets/markdown.svg)  
Indsættelse med reference: ![beskrivelse][markdown-logo]

[markdown-logo]: /assets/markdown.svg

---

## Kode
Hvis man har brug for at indsætte kode, kan man gøre det ved at indsætte back-ticks (`\``) rundt om koden således:
<pre lang="no-highlight"><code>
Man kan `indlejre kode` midt i en linje ved at sætte `enkelte` back-ticks rundt om det.

```
Hvis man vil have en kodeblok some denne
skal man blot sætte tre backticks på en ny linje
for at starte blokken.
Man slutter blokken på samme måde igen
```
</code></pre>

Man kan `indlejre kode` midt i en linje ved at sætte `enkelte` back-ticks rundt om det.

```
Hvis man vil have en kodeblok some denne
skal man blot sætte tre backticks på en ny linje
for at starte blokken.
Man slutter blokken på samme måde igen
```

---

## Tabeller

Tabeller er lidt tricky. Grundlæggende laver man noget der ligner en tabel i Markdown, og så bliver det oversat til en tabel på siden. Det kunne se således ud:
```md
| Navn      | Køn     | Fødselsdag   |
| --------- | ------- | ------------ |
| Jeppe     | Mand    | 01/04-2018   |
| Henriette | Kvinde  | 11/12/2019   |
| *Kursiv*  | **Fed** | understøttes |

Ovenstående er meget letlæseligt i Markdown. Det behøves dog ikke være så pænt formateret:
Selvom | jeg | formatere | grimt
--- | --- | --- | ---
bliver | det | rigtigt | oversat
og | bliver | ret | pænt
på | den | færdige | side
```

| Navn      | Køn     | Fødselsdag   |
| --------- | ------- | ------------ |
| Jeppe     | Mand    | 01/04-2018   |
| Henriette | Kvinde  | 11/12/2019   |
| *Kursiv*  | **Fed** | understøttes |

Ovenstående er meget letlæseligt i Markdown. Det behøves dog ikke være så pænt formateret:

Selvom | jeg | formatere | grimt
--- | --- | --- | ---
bliver | det | rigtigt | oversat
og | bliver | ret | pænt
på | den | færdige | side

---

## Citeringer
Det er muligt at lave en citering ved blot at starte en linje med en `>`.
```md
> Et lands opfindelser fortæller meget om dets beboere. Det er næppe tilfældigt, at det var danskerne, som opfandt antabus og korkbæltet
-- Paul Hammerich
```
> Et lands opfindelser fortæller meget om dets beboere. Det er næppe tilfældigt, at det var danskerne, som opfandt antabus og korkbæltet. - Paul Hammerich

---

## Skillestreger
Det er muligt at sætte en vandret skillestreg for mere struktur. Disse kan indsættes ved at sætte tre bindestreger på en linje for sig selv.
```md
Noget tekst

---

Noget helt andet
```
Noget tekst

---

Noget helt andet
