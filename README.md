
DJ Together 
Von Andreas Schindler und Leonie Mohr

Idee & Inspiration
Die Grundidee zu unserem Projekt entstand bereits in einem früheren GIS-Kurs, in dem wir ein kleines Musikprojekt realisiert haben. Damals haben wir gemerkt, wie viel Spaß es macht, Musik und Technik zu kombinieren – besonders, wenn daraus etwas Interaktives entsteht.
Diesen Gedanken haben wir jetzt weiterentwickelt: Mit DJ Together wollten wir eine Web-Anwendung schaffen, die es mehreren Nutzer:innen ermöglicht, in Echtzeit gemeinsam einen Song zu steuern – jede:r kann live Instrumente ein- und ausschalten, und das wirkt sich sofort auf alle anderen im Raum aus. Ziel war ein unkompliziertes, gemeinsames Musikerlebnis, das direkt im Browser funktioniert.

Konzept
Unsere Anwendung besteht aus einer virtuellen 3D-Bühne, auf der Instrumente wie Gesang, Gitarre und Schlagzeug platziert sind. Klickt man auf ein Instrument, wird der zugehörige Loop aktiviert oder stummgeschaltet. Die Aktion wird per WebSocket an alle anderen Teilnehmer:innen übertragen, sodass alle dieselbe Klangkulisse hören.
So entsteht ein einfacher, aber gemeinschaftlicher Musikmoment – man kann zusammen experimentieren, Instrumente layern oder ganz gezielt Beats setzen. Die Idee ist nicht nur unterhaltsam, sondern zeigt auch, wie sich Webtechnologien kreativ einsetzen lassen.

Eingesetzte Technologien
•	A-Frame – zur Darstellung der 3D-Szene und der interaktiven Instrumente
•	Web Audio API – zur Audioverarbeitung, Lautstärkesteuerung, Looping und 3D-Audio
•	WebSockets (über Web-Rooms) – zur Synchronisation aller Aktionen zwischen mehreren Clients
•	GLTF-Modelle und eigene Audiodateien im Loop-Format

Aufgabenverteilung
•	Andi hat sich um die 3D-Umgebung mit A-Frame und die Einbindung sowie Ansteuerung der Audiodateien gekümmert.
•	Leonie hat die Audiofunktionen weiterentwickelt (Looping, Lautstärke, Positionierung) und die Kommunikation über WebSockets umgesetzt, inklusive Echtzeit-Synchronisation.

Erkenntnisse & Herausforderungen
•	Die Kombination von Echtzeitkommunikation, Audio-Looping und Benutzerinteraktion war technisch herausfordernd, aber auch sehr spannend.
•	Besonders die Synchronisation aller Clients über WebSockets war eine Herausforderung – kleine Verzögerungen oder Zustandskonflikte wirken sich sofort hörbar aus.
•	Die Web Audio API hat sich als sehr flexibel erwiesen – viele Funktionen (z. B. räumlicher Klang oder Gain-Steuerung) konnten direkt umgesetzt werden.
•	A-Frame hat uns ermöglicht, schnell eine immersive und intuitive Umgebung zu gestalten, ohne aufwendige 3D-Software nutzen zu müssen.
•	Insgesamt war es spannend, aus einer Kursidee ein technisch funktionsfähiges und interaktives Musiktool zu entwickeln – mit dem Ziel, Menschen kollaborativ Musik „erleben“ zu lassen, nicht nur zu hören.

Nutzung der Anwendung
•	Die Anwendung im Browser öffnen (empfohlen: Chrome oder Firefox).
•	Auf eines der Instrumente (Mikrofon, Gitarre oder Schlagzeug) klicken, um den gemeinsamen Loop zu starten.
•	Weitere Instrumente können durch erneutes Klicken an- oder ausgeschaltet werden.
•	Andere Nutzer:innen, die gleichzeitig im Raum sind, hören dieselben Änderungen in Echtzeit.
•	Jetzt kann’s losgehen – gemeinsam Spaß haben und Musik kreieren!
Tipp:
Aufgrund von Browserrichtlinien kann es bei manchen Nutzer:innen vorkommen, dass der Sound nicht startet, bevor sie selbst eine Aktion im Browser gemacht haben – zum Beispiel eine Mausbewegung oder einen Klick. Das verhindert, dass Audio automatisch abgespielt wird, ohne dass die Person selbst interagiert hat. Deshalb empfehlen wir, vor dem gemeinsamen Musizieren einmal kurz den Bildschirm zu berühren oder zu bewegen. So können andere Nutzer:innen den Sound bei dir problemlos starten.

DJ Together soll zeigen, wie durch kreative Webtechnologien ein gemeinsames Musikerlebnis entstehen kann – einfach, direkt und für alle zugänglich. Das Projekt hat uns nicht nur technisch weitergebracht, sondern auch viel Spaß gemacht.

