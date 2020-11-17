# 00-Aktuelles-  
In dieser Datei werden aktuelle Änderungen und Ergänzungen aufgeschrieben  

**Allgemeines**  
Seit einiger Zeit bin ich dabei, eine größere Anlage aufzubauen. Ich habe dafür die Anlage Steinheim mit kleinen Änderungen ausgewählt. Die zugehörige Planung konnte man unter "GP3-0090 Märklin C-Gleis-Plan Steinheim 300x230x100cm (DIN A4-Mappe Color)" bei ebay kaufen. Parallel zum Aufbau dieser Anlage werde ich die Decoder auf OTA "umbauen" und dann in diesem repository einstellen.
Warum baue ich an dieser Anlage?  
1. Weil ich gerne baue.  
2. Der Gleisverlauf mit den langen Geraden und Brücken gefällt mir.  
3. Es ist sicherlich eine bereits mittelgroße Anlage. Mit dem Einsatz der CANgurus auf dieder Anlage möchte ich dem Eindruck einzelner Leser meines Buches entgegentreten, die CANgurus würden sich ausschließlich für Minianlagen eignen. Es ist sicherlich zutreffend, dass mit meinem Ansatz maximal 20 Decoder auf einer Anlage eingesetzt werden können. Deshalb überlegen wir mal, wieviel Decoder für diede Anlage notwendig sind.  

**Gleisbesetztmelder:** 3  
Mit den 3 Decodern sind 3*16=48 Meldepunkte möglich. Insgesamt habe ich allerdings nur 35 Sensoren eingesetzt. Mehr machen aus meiner Sicht keinen Sinn. Mit einer Reserve von 13 sind wir für neue Erkenntnisse gut aufgestellt. 

**Weichendecoder:**     5 (3)  
Es sind insgesamt 20 Weichen / Kreuzungen auf der Anlage. Um alle 20 Servos zu bedienen, benötigen wir 5 Decoder (4*5=20). Ich habe allerdings alle Weichen / Kreuzungen mit Servos ausgerüstet. Da ich ausschließlich Linearservos benutzt habe, wurde mir das irgendwann zu teuer und ich habe auch falsch eingestellte Weichen zugelassen, so zum Beispiel an den Ausgängen des Schattenbahnhofes. Mit den 8 Servos habe ich dann 2 Decoder eingespart.

**Signaldecoder:**      4  
Die beiden Lichtsignaldecoder habe ich in der PCA9685-Variante aufgebaut und kann dann 16 (!) LED-Signale aufbauen. Allerdings nur mit dem einfachen Rot/Grün-Bild. Mir reicht das. Wenn jemand mehr benötigt, kann man das mit dem Lichtdecoder umsetzen. Keine Raketenwissenschaft. Zwei weitere Signaldecoder habe ich dann für 8 Formsignale eingesetzt.

**Lichtdecoder:**       5   
Mit den 5 Lichtdecodern kann ich 5*16=80 LED ansteuern. Das reicht für viel Lichtbewegung auf der Anlage. 
Das sind jetzt in Summe 17 bzw. sogar nur 15 Decoder zuzüglich CANguru-Bridge. Wir bleiben als unter der Obergrenze und haben noch eine Reserve von 2 Decodern.  
  
**17.11.2020**  
Ich habe mehr oder weniger alle Repositories neu geordnet. Vielleicht ist es jetzt etwas übersichtlicher.

Weiterhin viel Spaß und Erfolg!

