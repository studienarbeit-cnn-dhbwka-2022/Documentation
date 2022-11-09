# General Planning File

## Idee

1. Verschiedene Verfahren erkennen Obst.
2. Wir vergleichen wie verlässlich die Verfahren zu welchem Lernzeitpunkt sind
3. Wir bearbeiten die Eingangsdaten (z.B. Filter wie Schwarz/weiß, Kantenglättung, etc.)
4. gehe mit diesen Eingangsdaten zurück zu Schritt 1

## Offene Fragen

Wollen wir nur Obst verlgeichen?
 Welches Obst? (z.B. Äpfel und Birnen oder doch Alles?)
Welche Verfahren gibt es und wie implementieren wir sie?
Wo lassen wir die laufen?
 Wie stellen wir sicher, dass sie fair gleich viele Ressourcen bekommen?

## Todo

Links zu Probedaten sammeln (gern auch hier)
Neues Meetup planen

## Linksammlung
  
- Beispieldaten
  - <https://www.image-net.org/>
  - <https://github.com/awesomedata/awesome-public-datasets>
- Frameworks 
  - https://pytorch.org/
  - https://www.tensorflow.org/tutorials/images/cnn

## Ideensammlung: Welche Verfahren wenden wir auf Die Bilder an? 
- Spiegeln
- bis zu 45° random drehen 
- Ausschneiden (Nur Bildbereich verwenden. Müsste aber klar sein, dass er groß genug ist.) 
- Schwarz/Weiß 
- Unscharf 
- Bereiche ausschneiden (schwärzen um corruption zu simulieren) 
- 
