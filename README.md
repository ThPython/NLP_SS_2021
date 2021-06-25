# NLP_SS_2021
Vorlesung NLP im Sommersemester 2021

Kanban Board https://github.com/users/Danielsoeller/projects/7?add_cards_query=is%3Aopen
Presi https://docs.google.com/presentation/d/113Yi6Itv_kxDrfnNHw37NRIL2TiLGcpKjNdyfj8ynW0/edit?usp=sharing

# Projekt Plan

Ziel: WIr wollen untersuchen, wie sich die öffentliche Meinung über Politiker im Laufe der Zeit verändert. 
Dafür wollen wir für jeden Politkier und für jeden Tag einen durchschnitlichen Sentiment Score errechnen, welchen wir dann auf einer Zeitachse plotten.
Wir können uns vorstellen, dass wir Sesionale?? Unterschiede finden. Dass Politiker im Sommer beliebter sind als im WInter.
Oder, dass wir anhand von besonderen Ausschlägen bzw. Veränderungen, auf Real Life Ereignisse schließen können.

## Vorgehen: 

**Daten extrahieren:** Aus den von unseren Dozenten gegebenem Datensatz extrahieren wir die query extentions oder Expansions ?. Dies machen wie mit einer einfachen Regex Expression: **"(.+?)"**

 '["Jan van Aken",["jan van aken privat","jan van aken bundestag","jan van aken biografie",
 "jan van aken twitter","jan van aken das geständnis des mönchs","jan van aken facebook",
 "jan van aken türkei","jan van aken israel","jan van aken kontakt","jan van aken mdb",
 "jan van aken maler","jan van aken linke","jan van aken sahra wagenknecht","jan van aken mitarbeiter",
 "jan van aken g20","jan van aken kurden","jan van aken praktikum","jan van aken pkk fahne",
 "jan van aken frau","jan van aken autor"]'
 
Nun ziehen wir den ersten String (Name des Politikers), von den nächsten X Strings ab. Sodass wir nur noch eine Liste von den Extaions??? Strings haben
[privat, bundestag, biografie, twitter, das geständnis des mönchs, facebook, .....]

Nun erechnen wir einen durchschnittlichen Sentiment score für diesen Tag. https://github.com/sloria/TextBlob
und speichern diesen mit dem zugehörigen Tag in einen Data Frame für diesen Politker. 

 
