Wiskundige Formalisering van Fibonacci-rijtjes als Vectorruimte
Deel 1: Bewijs dat Fibonacci-rijtjes een vectorruimte vormen (Opgave 1.1.19)
Volgens de bronnen is F de verzameling van alle rijtjes (a1, a2, …) van reële getallen die voldoen aan de Fibonacci-eigenschap an+2 = an+1 + an voor alle n ≥ 0.

We hoeven niet alle 8 complexe axioma's voor een vectorruimte te controleren. Omdat de rijtjes uit F een deelverzameling vormen van de ruimte van alle reeksen of 'discrete tijd signalen' (die al als vectorruimte is gedefinieerd), volstaat het volgens Stelling 1.1.13 om aan te tonen dat F een lineaire deelruimte is. Hiervoor toetsen we drie voorwaarden:

De nulvector is aanwezig (0 ∈ F): Het rijtje dat uitsluitend uit nullen bestaat, (0, 0, 0, …), voldoet overduidelijk aan de eigenschap 0 = 0 + 0 en bevindt zich dus in F.
Geslotenheid onder optelling: Stel dat we twee rijtjes a en b in F hebben. Voor de som van deze rijtjes geldt (a+b)n+2 = an+2 + bn+2. Omdat a en b beide Fibonacci-rijtjes zijn, kunnen we dit uitschrijven als (an+1 + an) + (bn+1 + bn). Herschikken levert op: (an+1 + bn+1) + (an + bn), wat exact (a+b)n+1 + (a+b)n is. De som van twee Fibonacci-rijtjes is dus opnieuw een Fibonacci-rijtje.
Geslotenheid onder scalaire vermenigvuldiging: Neem een constante c ∈ ℝ en een rijtje a ∈ F. Dan is de schaling (ca)n+2 = c(an+2) = c(an+1 + an). Dit kunnen we uitschrijven als c an+1 + c an = (ca)n+1 + (ca)n. Het geschaalde rijtje behoort dus ook tot F.
Aangezien F aan alle drie de voorwaarden voldoet, is het een lineaire deelruimte en daarmee een geldige vectorruimte.

Deel 2: Bewijs dat de dimensie van F precies 2 is (Opgave 1.2.25)
Om aan te tonen dat de dimensie van F gelijk is aan 2, moeten we bewijzen dat er een basis voor F bestaat die uit exact twee elementen (vectoren) is opgebouwd. Een basis is per definitie een stelsel dat zowel een volledig stelsel is als lineair onafhankelijk is.

Omdat bij een Fibonacci-rijtje elk volgend getal simpelweg de som van de twee voorgaande is, ligt de gehele reeks deterministisch vast zodra de eerste twee elementen (a1 en a2) bekend zijn. Laten we twee specifieke basis-rijtjes in F creëren die als fundamentele bouwstenen fungeren:

v1 = (1, 0, 1, 1, 2, 3, 5, …)

v2 = (0, 1, 1, 2, 3, 5, 8, …)

We toetsen of deze twee rijtjes de basis vormen:

Is het een volledig stelsel (opspansel)? Elke vector (rijtje) uit F moet geschreven kunnen worden als een lineaire combinatie van v1 en v2. Neem een willekeurig Fibonacci-rijtje a = (a1, a2, a3, …) in F. We kunnen proberen dit te bouwen met a1v1 + a2v2. Laten we naar de eerste twee posities in de reeks kijken:
Positie 1: a1(1) + a2(0) = a1.
Positie 2: a1(0) + a2(1) = a2.
Omdat de eerste twee elementen van ons geconstrueerde rijtje feilloos overeenkomen met die van rijtje a, en omdat lineaire combinaties van Fibonacci-rijtjes weer Fibonacci-rijtjes opleveren (zoals we in deel 1 bewezen), moet de rest van de reeks ook perfect identiek zijn. Ieder willekeurig rijtje a is dus op te bouwen, wat (v1, v2) een volledig stelsel maakt.

Is het lineair onafhankelijk? Er mag geen afhankelijkheid tussen v1 en v2 bestaan; de ene mag geen veelvoud van de andere zijn. Wiskundig betekent dit dat als c1v1 + c2v2 = 0 (waarbij 0 de nulfunctie is), dan mag dit alleen kunnen wanneer c1 en c2 beide 0 zijn.
We kijken weer naar de eerste twee posities van de reeks:
Uit positie 1 volgt: c1(1) + c2(0) = 0 ⇒ c1 = 0.
Uit positie 2 volgt: c1(0) + c2(1) = 0 ⇒ c2 = 0.
Omdat c1 en c2 verplicht 0 zijn, zijn de twee vectoren aantoonbaar lineair onafhankelijk.
Conclusie: Omdat (v1, v2) zowel een lineair onafhankelijk stelsel als een volledig stelsel voor F is, vormt het een basis. Deze basis bestaat uit exact 2 elementen (de twee "atomen" v1 en v2). Volgens de Hoofdstelling van de Lineaire Algebra betekent dit wiskundig definitief dat dim F = 2.
