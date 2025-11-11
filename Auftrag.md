# Arbeitsauftrag
Beobachte das Objektspiel zum *second hand shop* und beantworte folgende Fragen:
1. Wie entwickelt sich die Länge der Datenstruktur? Spielt die Länge der Datenstruktur eine Rolle zur Verwaltung der Elemente?
- Verlängert sich immer wenn jemand den Laden betritt
- Es passen immer nur drei Kunden in den Laden

- spielt keine Rolle (Vermutung: alle Verwaltungsoperationen funktionieren auf jeder beliebigen Länge. Auf die meisten Elemenete wird nicht zugegriffen)

2. Wie werden neue Elemente hinzugefügt?
- Verwaltung fügt das Element hinter das letzte Element ein.
- interessanter Fall: Das aller erste Element, wenn die Schlange leer ist

3. Auf welche Elemente wird Zugegriffen?
- es wird nur auf das erste Element zugegriffen

4. Welche Beziehungen der Elemente gibt es untereinander?
- Ein Element kennt das Element, welches vor ihm steht
- jedes Element kennt seinen eigenen Inhalt (Hier: Bestellbestätigung)
- Elemente müssen ihre Nachfolger nicht kennen (oder doch? ansonsten geht Informationen verloren)

5. Welche Elemente müsste ein Verwaltungselement kennen?
- alle Elemente? Erstes und letztes aif jeden Fall
- kennt den Inhalt der Elemente nicht
- nur das erste und das letzte Element werden benutzt 

6. Nach welchem Prinzip arbeitet die Datenstruktur? Wie nennt man eine solche Datenstruktur?
- FIFO: First in first out 
- Warteschlange, englisch: queue

7. Welche (Verwaltungs)Operationen sind für diese Datenstruktur sinnvoll?
- Elemente hinzufügen/ einreihen
- das erste Element entfernen / entlassen
   -> aufrücken lassen
- wissen ob die Schlange leer ist
- gib das erste Element 

Fragen:
- Vorgaänger / nachfolger was wird hier wirklich benötigt?
- Was müssen Elemente eigentlich jetzt können (Vllt Inhalt geben)

notizen:
elemente kennen ihren Vorgänger
verwaltungselement kennt erstes und lketztes element(zeiger)
um auf neues erstes element zugreifen zu können, auf letztes zugreifen, vorgänger abfragen (boolean/gucken ob null)
verwaltung gibt verkäufer erstes element -> kann darauf zugreifen
Elemente rücken NICHT auf


 

