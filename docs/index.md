# Introduction
This document explains the basic interaction with AsiBot. AsiBot is a web-application that
enables writers to interact with a text-generation system to create unique ouvres.

# First login
AsiBot is deployed over the web which requires a loging system.
On first use of the application you will have to register a new user and password.

# Structure of AsiBot
AsiBot is designed with simplicity in mind. All the interaction takes place on a single
page that includes a Text Editor, a toolbar controlling the settings of the text-generation 
system (Generate Bar) and a panel displaying the output of the text-generation system 
(Suggestions Panel).

## The Generate Bar
![generate bar](/images/generate_bar.png)

The generate bar displays a number of options controlling the text-generation system:
- Creativity: the higher the more diversity but also the less grammatical the sentences will be.
- Length: maximum number of character to generate.

Additionally, AsiBot deploys a number of text-generation system fine-tuned to generate
text in particular styles. Each system is color coded.

## Suggestions
Generated text is shown in the suggestions panel to the bottom of the page.
![suggestions](/images/suggestions.png)

- The panel will open when you start generating text.
- Each time you generate, you will get 5 new suggestions.
- You can keep a number of suggestions in the suggestion panel (but bear in mind that **they will disappear whenever you refresh the page**).
- You can remove individual items in order to maintain a list of preferred text.
- The panel can be open and closed using the left-hand arrow.

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
