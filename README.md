Wolken-Jäger
Ein dynamisches, browserbasiertes 2D-Schussspiel. Ein einzelner Vogel sitzt auf einem natürlichen Stein und schießt leuchtende Projektile auf vorüberziehende Wolken am Nachthimmel.

Spiel-Screenshot(Tipp: Ersetze den Link oben durch einen Screenshot aus dem assets/ Ordner oder einen direkten Screenshot)

✨ Merkmale
Atmosphärisches Design: Ein tiefes, mehrschichtiges Nachthimmel-Design mit funkelnden Sternen, einem leuchtenden Mond und schattierten Bergsilhouetten.
"Charlytaxi-Air"-Branding: Ein schwebendes, goldenes Logo mit Lichteffekten und dekorativen Elementen ziert den Himmel.
Intelligente Steuerung: Der Vogel dreht sich fließend und dynamisch in die Zielrichtung der Maus.
Verschiedene Wolken-Typen: Von kleinen, fragilen Wolken (1 Treffer) bis hin zu massiven Sturmwolken (3 Treffer). Jede Art bringt unterschiedliche Punkte.
Visuelles Feedback: Zerstörungspartikel, Treffer-Blitze, Risse in beschädigten Wolken und HP-Balken bei mehrfachen Treffern.
Prozeduraler-Sound: Komplett generierte Sound-Effekte (Schuss, Treffer, Zerstörung, Fehlschuss) via Web Audio API – komplett ohne externe Dateien.
Steigernde Schwierigkeit: Je mehr Punkte du sammelst, desto schneller und dichter erscheinen neue Wolken.
Null Abhängigkeiten: Läuft komplett standalone. Keine Frameworks, keine Build-Tools, keine externen Assets.
🎮 So wird gespielt
Zielen: Bewege die Maus (oder deinen Finger auf dem Smartphone) über den Himmel. Der Vogel richtet sich automatisch aus.
Schießen: Klicke (oder tippe) auf eine Wolke, um einen Schuss abzufeuern.
Punkte sammeln: Jede zerstörte Wolke bringt Punkte. Kleine Wolken = 10 Punkte, Große = 30 Punkte.
Durchhalten: Der Vogel hat keine Munitionslimit, aber die Wolken werden mit der Zeit überhandnehmen!
🛠️ Technische Umsetzung
Das Spiel besteht aus einer einzigen Datei und nutzt reines Vanilla JavaScript zusammen mit dem HTML5 Canvas.index.html

Grafik: HTML5 Canvas 2D-Kontext.
Ton: Web Audio API (Oszillatoren, Filter, procedurale Rausch-Generatoren).
Kompatibilität: Enthält einen robusten Ellipsen-Renderer. Falls der Browser die native -Methode nicht unterstützt, wird die Form sicher über trigonometrische Berechnungen gerendert (verhindert Abstürze auf älteren Mobilgeräten).ellipse()
Styling: Reines CSS ohne Preprocessor. Verläßliche Größenanpassung über CSS-Variablen.
Architektur: State-basierte Game-Loop (), strikte Trennung von Update-Logik und Rendering.requestAnimationFrame
🚀 Starten
Da das Spiel keine Server, APIs oder Build-Schritte benötigt, ist der Start extrem einfach:

Lade den Ordner (oder die Datei) herunter.index.html
Öffne die in einem modernen Webbrowser (Chrome, Firefox, Safari, Edge).index.html
Klicke auf "Los geht's" und beginne zu schießen!
