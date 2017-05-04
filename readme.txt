Hinweise:

Spezifische Einstellungen für Diplomarbeit/Bachelorarbeit/Masterarbeit und
wiederkehrende Angaben wie Name, Abgabedatum und Inventarnummer sind in der
Datei settings.tex als eigene Kommandos definiert und sollten nur dort
geändert werden.


Minianleitung zum Übersetzen der Arbeit
inklusive Erstellung des Literaturverzeichnis:

1. latex MUSTER.tex
 -> erzeugt u.a. MUSTER.aux
 
2. bibtex MUSTER
 -> erzeugt MUSTER.bbl  (Bibliographiefile)
 
3. erneut
   latex MUSTER.tex
 -> erzeugt MUSTER.dvi und bindet automatisch
    das nun existierende Bibliographiefile ein
    
 (bei Meldung von "undefined references" möglicherweise einmal
  mehr durchlaufen lassen)
    
4. dvips MUSTER.dvi
 -> erzeugt Postscript
 
alternativ statt Kombination latex/dvips auch möglich:
   pdflatex MUSTER.tex
  -> erzeugt direkt PDF-File
     
