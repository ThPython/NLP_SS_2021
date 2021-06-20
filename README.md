# NLP_SS_2021
Vorlesung NLP im Sommersemester 2021

# Porjekt Plan

Ziel: WIr wollen unterschuchen, wie sich der die Öffentliche Meinung über Politiker im Laufe der Zeit verändert. 
Dafür wollen wir für jeden Politkier,für jeden Tag einen Druchschnitlichen Sentiment Socere erechen. Denn wir dan wieder rum auf die Zeitachse ploten.
Wir können uns vorstelen das wir Sesionale Unterschiede finde, das also Politiker im Sommer beliebter sind, als im WInter.
Oder das wir anhand von besonderen ausschlägen, auf real Life ereignisse schlißen können.

## Vorgehen: 

**Daten extrahieren:** Aus den von unseren Dozenten geben daten Satz extrahieren wir die quary extentions. Dies machen wie mit einer Einfachen Regex Expration: **"(.+?)"**

 '["Jan van Aken",["jan van aken privat","jan van aken bundestag","jan van aken biografie",
 "jan van aken twitter","jan van aken das geständnis des mönchs","jan van aken facebook",
 "jan van aken türkei","jan van aken israel","jan van aken kontakt","jan van aken mdb",
 "jan van aken maler","jan van aken linke","jan van aken sahra wagenknecht","jan van aken mitarbeiter",
 "jan van aken g20","jan van aken kurden","jan van aken praktikum","jan van aken pkk fahne",
 "jan van aken frau","jan van aken autor"]'
 
nun ziehen wir den ersten String(Name des Politiker), von den nächsten X Stings ab. Sodas wir nur noch eine liste von den Extaions String haben
[privat, bundestag, biografie, twitter, das geständnis des mönchs, facebook, .....]

nun erechnen wir einen Duchschnitlichen Sentiment socere für diesen Tag. UNd speicher diesen mit den dem zugehörigen Tag in eien Data Frame für diesen Politker. 



**Daten Untersuchen**, nun konnen wir die Daten untersuchen, so könnenneben visualtionen und Duchschnite für mehre Politiker einer Partei oder Geschlecht, 
auch ausreißer analysen durch gefühert werden.
 
