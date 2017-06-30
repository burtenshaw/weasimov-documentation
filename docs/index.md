# Inleiding

Deze pagina geeft een bescrhrijving en handleiding van AsiBot. Asibot is een web-applicatie waarmee schrijvers een interactie kunnen aangaan met een geavanceerd tekstgeneratie-systeem om tot uniek nieuw materiaal te komen.

# Aanmelden
Omdat AsiBot via het web wordt aangeboden, vragen we je om een account aan te maken via de registratie-pagina. Klik op de link 'registreer' of ga direct naar: http://localhost:5555/register.

# Opzet van AsiBot
De interface van AsiBot is zo simpel mogelijk gehouden. Alle interactie met de applicatie vindt plaats op een enkele pagina met drie onderdelen: (1) een tekst-editor, (2) een toolbar met een reeks knoppen om het tekstgeneratie-systeem aan te sturen, en (3) een panel waarin de tekstsuggesties van het systeem worden weergegeven. Hieronder bespreken we elk onderdeel 
in iets meer detail.

## Generatie-toolbar
![generate bar](/images/generate_bar.png)

De generatie-toolbar geeft een aantal opties om het tekstgeneratie-systeem aan te sturen. De belangrijkste knoppen zijn de pastel-gekleurde knoppen aan de rechterkant, die elk tekst genereren in een bepaalde stijl. Houd de muis op een van de knoppen om de volledige naam van de stijl te zien. Na het klikken op een van de knoppen, geeft het systeem een aantal tekstsuggesties in de gekozen stijl. Deze suggesties zijn aanklikbaar en worden toegevoegd aan de tekst op de plaats waar de cursor in het tekstvak staat. Naast de genereer-knoppen geeft de toolbar nog twee andere opties: een creativiteitsschuif en een lengteschuif. De lengteschuif controleert hoe lang de gegeneerde tekst zal zijn in aantal karakters. (Dit kan soms betekenen dat AsiBot stopt in het midden van een woord) De creativiteitsschuif controleert hoe divers de gegenereerd tekst zal zijn. Lagere waardes zorgen voor conservatievere tekst; hogere voor creatievere tekst. Het is voor elk model wat zoeken naar een ideale waarde. De kans op ongrammaticale zinnen neemt toe met hogere waardes (maar soms worden wel erg leuke suggesties gedaan en worden zelfs nieuwe woorden bedacht). Lagere waardes kunnen soms wat eentonig aandoen, maar zijn vaak wel grammaticaal correct. 

## Tekstsuggesties
Na het klikken op een van de generatie-knoppen, doet het systeem een aantal tekstsuggesties die onderaan de pagina worden weergegeven.
![suggestions](/images/suggestions.png)

- Het panel opent direct na het genereren van tekst;
- Elke generatie geeft vijf nieuwe suggesties;
- Individuele suggesties kunnen bewaard worden of worden verwijderd. **Pas op: als je de pagina ververst zijn de laatste (bewaarde) suggesties niet meer beschikbaar.
- Het suggestiepaneel kan gesloten worden met het pijltje aan de linkerkant.


## Text Editor

AsiBot uses a conventional rich-text editor that enables common inline styling features such
as bolding, underlining, etc... The most ideosyncratic feature of the text editor is that it 
keeps track of the origin of all textual fragments, both human and machine authored, and it
displays this information by means of inline annotation.

### Annotation ###

![annotation](/images/annotation.png)

The visual annotation works as follows.
- Whenever a system suggestion is inserted into the document, the text editor will highlight this fragment
  using the color of the source model.
- Originally computer-generated text can be edited, in which case the original annotation
  color will start to fade towards white in relation to the amount of editing done to the fragment.
- The user's text will appear in white.

# Saving Data

AsiBot incorporates an automated saving system, so you can be reassured that the document will always be save.
You can safely close the browser and the last document state will reappear upon login.
