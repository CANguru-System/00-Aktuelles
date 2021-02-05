# 00-Aktuelles-  
In dieser Datei werden aktuelle Änderungen und Ergänzungen aufgeschrieben  
   
**05.02.2021**  
Noch ein Fehler bei der CANguru-Bridge. Bei WinDigiPet konnte die Zentrale nicht ausgelesen werden. Auch die Dateien im Verzeichnis 01x-CANguru, die in das Verzeichnis C:/CANguru kopiert werden müssen, waren nicht ganz in Ordung.    
   
**27.01.2021**  
Bei der CANguru-Bridge gab es ein Problem, wenn kein Decoder angeschlossen ist.    
   
**12.01.2021**  
Bei der CANguru-Bridge gab es durch eine aktualisierte Library ein LCD-Problem. Es wird wieder die alte benutzt.    
  
**09.01.2021**  
Der Maxi-Signaldecoder erscheint nun auch unter diesem Namen im CANguru-Server.    
  
**29.12.2020**  
Unter 10-Aktuelle-OTA-Versionenhabe ich einen Maxi-Signaldecoder eingebracht. Damit können 16 Formsignale und 8 LED-Signale gesteuert werden. Dafür wurden 2 Bausteine PCA9685 verwendet. Dieser Decoder ist der erste, der mit dem CANguru-Server durch den Button RESET (unterhalb von OTA) angesprochen werden kann. Dadurch werden die Parameter in diesem Decoder auf Standardwerte zurückgesetzt. Diese Funktion ist insbesondere für Menschen interessant, die an dem Decoder basteln und häufig wieder Standardwerte verwenden müssen.
       
**25.12.2020**  
Alle Module im Repository 10-Aktuelle-OTA-Versionen wurden entschlackt, indem alle gemeinsam genutzten Dateien aus den einzelnen Modulen entfernt und in gemeinsame Ordner verlegt wurden. Das ist hilfreich, wenn Änderungen eingebracht werden, die mehrere Decoder betreffen. Möglicherweise kann man diesen Streamlining-Prozess noch weiter fortführen. Vielleicht mache ich das auch irgendwann.   
Es ist wichig, die Struktur der Dateien so zu belassen, so dass die gemeinsamen Dateien auch vom PlatformIO gefunden werden.
  
**17.11.2020**  
Ich habe mehr oder weniger alle Repositories neu geordnet. Vielleicht ist es jetzt etwas übersichtlicher.  
Insbesondere habe ich alle aktuellen Versionen in einem neuen Repository zusammengestellt. Weiterhin gibt es eine deutlich einfachere Methode, die OTA-Versionen aufs Board zu laden.  
Die ursprünglichen Nicht-OTA-Versionen werden nicht mehr weiter entwickelt.
  
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
   
Weiterhin viel Spaß und Erfolg!

