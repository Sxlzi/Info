---
marp: true
paginate: true
style: |
  /* ==============================================================
     Vorlage für Marp
     Diese Datei ist dein Gerüst. Ändere Werte, niemals die Namen
     der Klassen – die müssen zum Text passen, sonst passiert nichts.

     Wichtig: Diese Vorlage nutzt HTML (<div class="...">). Marp
     blockiert das standardmäßig. Aktiviere HTML:
       - VS Code: Einstellung "markdown.marp.enableHtml"
       - Marp CLI: Option --html
     ============================================================== */

  /* --- Die Farben ------------------------------------------------
     Jede Farbe steht genau einmal hier. Alle Klassen weiter unten
     benutzen nur noch den Namen. Willst du das Aussehen ändern,
     änderst du nur diese sieben Zeilen – nicht die Klassen. */

  :root {
    --blau:      #17324d;   /* Titel, Balken, Linien */
    --blau-hell: #24527a;   /* Akzente, Rand der Karten */
    --flaeche:   #f7f9fc;   /* Hintergründe von Kästen */
    --flaeche-2: #edf5fb;   /* zweiter Hintergrundton */
    --flaeche-3: #e8f1f8;   /* dritter Hintergrundton */
    --flaeche-4: #eef5f9;   /* Karten */
    --gelb:      #f4d35e;   /* Hervorhebung */
  }

  /* --- Die Folie selbst ------------------------------------------
     Jede Folie wird zu einem <section>. Alles hier gilt für alle. */
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100%;
    padding: 40px;
    font-family: Arial, Helvetica, sans-serif;
  }

  /* --- Der Folientitel ------------------------------------------- */
  .titel {
    width: 100%;
    text-align: center;
    color: var(--blau);
    margin-bottom: 24px;
  }

  /* --- Eine einfache Liste --------------------------------------- */
  .liste {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Ein hervorgehobener Satz ---------------------------------- */
  .merksatz {
    width: 80%;
    margin-bottom: 20px;
    padding: 20px;
    background: var(--gelb);
    font-weight: bold;
    border-radius: 20px;
    text-align: left;
  }

  /* --- Ein einzelner Kasten -------------------------------------- */
  .box {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche-2);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Zwei Spalten: legt die Aufteilung fest -------------------- */
  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  /* Spaltenverhältnisse zum Ausprobieren:
       1fr 1fr  -> zwei gleich breite Spalten
       2fr 1fr  -> links doppelt so breit wie rechts
       1fr 2fr  -> rechts doppelt so breit wie links               */

  /* Eine breite und eine schmale Spalte:
     .grid-2 { grid-template-columns: 2fr 1fr; align-items: center; } */

  /* --- Die Spalte: nur das Aussehen ------------------------------ */
  .spalte {
    padding: 18px;
    background: var(--flaeche-3);
    border-radius: 14px;
    text-align: left;
  }

  /* --- Karten: drei Dinge nebeneinander -------------------------- */
  .karten {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    width: 100%;
  }

  .karte {
    min-height: 150px;
    padding: 16px;
    background: var(--flaeche-4);
    border-top: 5px solid var(--blau-hell);
    text-align: left;
  }

  /* --- Bilder ---------------------------------------------------- */
  .bild {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
  }

  .bild img {
    width: 320px;
    height: auto;
  }

  /* --- Die Fußzeile ---------------------------------------------- */
  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 1px solid var(--blau);
    text-align: center;
    font-size: 0.6em;
  }
---

<div class="titel">

# Titel deiner Präsentation

</div>

<div class="liste">

Name:Finn
Klasse:9a
Datum:08.10.26
- Heutige Bedeutung: Damit man einen ort hat wo man seine Passwörter speichern kann um sie sich zu merken und nicht zu verlieren.
- Leitfrage und Ziel: Welcher Passwortmanager
ist am sichersten und wie vereinfacht er den digitalen Alltag?

</div>

<div class="fusszeile">
  Passwortmanager · Finn, 9a
</div>

---

<div class="titel">

# Passwortmanager über die ich sprechen werde:

</div>

<div class="liste">

- Samsung Pass
- passwords.google
- Apple Password

</div>

<div class="fusszeile">
  Drei Manager · Finn, 9a
</div>

---



<div class="titel">

# Pro und Contra Passwortmanager: Samsung Pass

</div>

<div class="grid-2">
  <div class="spalte">

  **Pro**
-Einfache Bedienung
-Siche
-Anmeldung per Fingerabdruck oder Gesichtserkennung
-Kostenlos

  </div>
  <div class="spalte">

  **Kontra**

  -Hauptsächlich für Samsung-Geräte
  -Weniger Funktionen
  -Abhängigkeit vom Samsung-Konto
  
   

  </div>
</div>

<div class="fusszeile">
  Pro&Kontra · Name, Klasse
</div>

---

<div class="titel">

# Fazit zu Samsung Pass

</div>

<div class="liste">

-Sicher und einfach zu nutzen
-Gut für Samsung-Nutzer
-Speichert und füllt Passwörter automatisch aus
-Weniger Funktionen als andere Passwortmanager

</div>

<div class="fusszeile">
  Fazit · Finn, 9a
</div>

---

<div class="titel">

# Pro und Contra Passwortmanager: Google.Passwords

</div>

<div class="grid-2">
  <div class="spalte">

  **Pro**

-Kostenlos
-Einfach zu nutzen
-Speichert Passwörter automatisch

  </div>
  <div class="spalte">

  **Kontra**

-Google-Konto nötig
-Datenschutzbedenken
-Weniger Funktionen als andere Passwortmanager
  
   
  </div>
</div>

<div class="fusszeile">
  Pro&Kontra · Name, Klasse
</div>

---




<div class="titel">

# Fazit zu Google.Passwords

</div>

<div class="liste">

-Einfach und kostenlos
-Praktisch für Google-Nutzer
-Gute Grundfunktionen
-Weniger flexibel als andere Passwortmanager

</div>

<div class="fusszeile">
  Fazit · Finn, 9a
</div>

---

<div class="titel">

# Pro und Contra Passwortmanager: Apple Password

</div>

<div class="grid-2">
  <div class="spalte">

  **Pro**

-Sicher
-Einfach zu nutzen
-Automatische Anmeldung

  </div>
  <div class="spalte">

  **Kontra**

-Vor allem für Apple
-Abhängig von Apple-ID
-Weniger Funktionen
  
   
  </div>
</div>

<div class="fusszeile">
  Pro&Kontra · Name, Klasse
</div>

---

<div class="titel">

# Fazit zu Apple Password

</div>

<div class="liste">

## Fazit:

-Sicher für Passwörter
-Einfach zu bedienen
-Gut für Apple-Geräte
-Weniger geeignet für andere Systeme

</div>

<div class="fusszeile">
  Fazit · Finn, 9a
</div>

---

<div class="titel">

# Endfazit zum Thema Passwortmanager

</div>

<div class="liste">

### Mein Endfazit:

-Sicher und einfach
-Schnelle Anmeldung
-Spart Zeit
-Ideal für Samsung-Nutzer
-Für mich die beste Wahl, da ich Samsung nutze



</div>

<div class="fusszeile">

Endfazit · Finn, 9a
</div>





