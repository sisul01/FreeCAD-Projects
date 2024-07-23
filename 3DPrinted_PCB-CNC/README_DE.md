Small PCB-CNC (Mostly printed)


Dies ist eine kleine, hauptsächlich gedruckte kleine Tischfräse für alle, die einfach mal probieren wollen, ob eine CNC-Fräse oder Graviermaschine etwas für sie ist. Idealerweis hat man bereits einige der benötigten Teile wie Schrittmotoren, Netzteile etc. herumliegen.

Ich wollte schon seit längerer Zeit eine CNC-Fräse oder eine CNC-Graviermaschine bauen. Einfach aus technischer Neugier, einen realen Nutzen ausser das gravieren von PCBs konnte ich mir nicht vorstellen. Daher sollte es kostengünstig sein, aber doch mit möglicht guten Eigenschaften.
Auf Thingiverse stiess ich dann auf die ['Small PCB CNC'](https://www.thingiverse.com/thing:4251212) von [Moe_Fpv_Team](https://www.thingiverse.com/Moe_Fpv_Team). Die Grundidee fand ich gut, die technische Ausführung ist meiner Meinung aber nach sehr verbesserungswürdig. 
So habe ich die Idee übernommen, eine CNC-Maschine mit möglicht vielen 3D-gedruckten Teilen zu konstruieren und damit die Kosten klein zu halten. Die Teile passen alle  auf das Druckbett (220mm x 220mm) meines 3D-Druckers.

Herausgekommen ist eine Maschine mit folgenden Daten:

Arbeitsfläche (xyz)mm: 120 x 120 x 60
Rahmen (xyz)mm: 275 x 275 x 320
Motor: DC Motor, 24V, 200W, 52mm Durchmesser
Spindel: 10000rpm
Achsen: 3 x NEMA17
Steuerung: Arduino Uno mit GRBL-Shield
Firmware: GRBL 1.1
Besonderheiten: backlash prevention, Endstop, Kabelmanagement
Unterstützte Materialien: Weichmetalle, Acryl, Holz, PVC und PCB

Kosten wenn man alles kaufen muss: ca. 160$ - 200$

Die aktuelle Version ist relativ starr, für den Rahmen habe ich PLA eingesetzt, was ein stabiler, harter Kunststoff ist. Die thermische Belastung dieser Bauteile ist gering, daher ist PLA gut geeignet und zudem ein günstiges Material. Im weiteren tragen die Führungsstangen mit Durchmesser 10mm in den X und Y Achsen und die geringe Länge ebenfalls zu Stabilität bei.
Ich habe mich entschieden, für die erste Version die Schrauben ohne Gewindehülsen direkt in den Kunststoff zu drehen. Die Schrauben lassen sich bei den kleineren Gewinden direkt ohne vorherigen Einsatz eines Gewindebohrers direkt in den Kunststoff drehen. Da sich die Schrauben während des erstmaligen Einschraubens relativ stark erwärmen, empfehle ich, vor dem endgültigen Festziehen einen Moment zu warten. Die M5-Gewinde sollten vorgeschnitten werden. 
Die optionalen Endschalter habe ich mit Adapterplatten befestigt. So kann relativ einfach der Auslösepunkt eingestellt werden. Werden andere als die von mir gewählten Endschalter eingesetzt, ist es ohne Probleme möglich, die Adapterplatten mit kleinem Aufwand zu modifizieren. In der Praxis hat sich gezeigt, dass die Kabel der Endschalter sehr anfällig auf Störungen sind. Daher habe ich für die Verdrahtung geschirmtes Audiokabel verwendet und zusätzlich eine galvanisch Trennung des Signals mit Optokopplern gemäss Anleitung ['Wiring Limit Switches'](https://github.com/gnea/grbl/wiki/Wiring-Limit-Switches) in der GRBL-Wiki eingesetzt.

Ebenfalls optional ist die Verwendung der backlash prevention nuts. Werden diese eingesetzt, habe ich festgestellt, dass die mitgelieferte Feder eher schwach ist. Idealerweise sollte die Feder durch eine stärkere Variante mit gleichen Durchmesser ersetzt werden.
Das Kabelmanagement ist durch eine Kabel-Kette auf der X-Achse und Durchführungen für Kabelbinder an den Seitenpanels realisiert.
Als Steuerung habe ich ein Arduino Uno mit GRBL-Shield und A4988-Schrittmotortreibern verwendet. Auf weitere Hinweise zur Verkabelung verzichte ich hier. Ich gehe davon aus, dass jeder, der so eine Maschine baut, weiss was er tut oder in der Lage ist, den unzähligen Ableitungen dazu im Internet zu folgen.

Bei den 3D-Druckteilen sollte man bei den mechanisch beanspruchten Teilen auf eine genügende Wandstärke achten, d.h. die Perimeterstärke sollte 1.6mm - 2mm betragen. Nicht zu vergessen sind auch die horizontalen Schichten, die ebenfalls diese Masse aufweisen sollten. Zu den mechanisch beanspruchten Teilen gehören: Base-Frame, SidePanel_Left, SidePanel_Right, RearStrut, Y-Sled, X-Sled, Z-Sled, X-Sled_BottomPlate und X-Sled_TopPlate. Für die meisten Teile kann PLA verwendet werden. Das ergiebt bei der Rahmenkonstruktion durch die Materialeigenschaften des PLA die benötigte Steifigkeit. Die X-, Y- und Z-Schlitten habe ich in PETG gedruckt, da hier die meisten Vibrationen anfallen und dieser Werkstoff diese besser abfangen kann.

Alle Druckteile sind als STL und STEP-Datein verfügbar. Die STL-Dateien sind bereits für den Druck entsprechend ausgerichtet. Ebenfalls veöffentlich ist eine Stückliste und ein Zusammenbau mit sämtlichen Teilen inkl. Schrauben, so dass eine guter Überblick über das Projekt möglich ist.