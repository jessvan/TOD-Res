# Hybrid Publishing Toolkit Workflow for Print & ePub

Diagram for visual explanation of the process.
![](imgs/Workflow.png)

This workflow applies to all books produced by PublishingLab, including the KnowledgeMile series. 
Note: the Theory on Demand publications have an InDesign template file (.indt) + font files included so that it is quicker for a designer to style content and create a .pdf.
 
The KnowledgeMile and other series may require a more custom approach to the design.

GitHub is also an important part of the workflow, it allows versions and progress of the book to be tracked and archived.

Credit: The greater part of this framework was developed as part of the Digital Publishing Toolkit by Michael Murtaught, with the support of Institute for Network Cultures and Creating 010.

# icml to InDD Workflow explained

This is the process, it has 2 stages: the initial stage sets the book up and results in a pdf that can have a final checked done by the editor.

The final stage is where the icml can be unlinked and manual changes made to finish the book.

## To begin

The Hybrid Publishing Workflow uses markdown and Pandoc to create multiple outputs. A developer (or editor) will convert the author's Word documents to markdown, make changes and then supply the editor with an icml file. Icml files are Adobe inCopy files that are read by inDD. This means designers don't have to refer to a pdf or Word Document to know how the document is marked up.

### Where the designer comes in
The designer is involved once the editor has finished marking up and editing the text. Of course, nothing is perfect, which is why there is a final check (and update) before the last icml is sent, which the designer will update and can unlink.

To be able to do this final check, the pdf is needed.

##icml to InDD

1. Open a new document in InDD (or a template .indt file if it has been provided) and file > place the icml(s).
Don't be alarmed if all the text is set in minion pro (or some default font), it looks like this because the icml can tell InDD to define the styles of the text (which parts are headers etc.), but not do the actual design work. 

2. Check the paragraph & character styles panel to see that the styles have been created and are applied correctly.
3. To make changes, checkout your icml file, go to Edit > InCopy > Checkout
4. Define styles, place images, create a cover, but do not start making manual changes (like fixing widows or adding custom spacing)
5. Once everything is in the book (all images, diagrams) and the styles are correct, export a .pdf for the editor to do a final check.
6. The editor checks, corrects & a new icml file is created and sent to the designer.
7. Relink the icml file - your paragraph changes should remain, but it is likely you will need to relink images. Now that you have the final icml (make sure the editor has confirmed that you do). You can unlink from the icml and finish manual changes.
8. Done - export the final .pdf

See the <a href="">FAQs</a> to find answers to common errors.

Success!

# md to ePub
The instructions can be found here on
<a href="https://github.com/DigitalPublishingToolkit/Hybrid-Publishing-Resources/wiki/From-Manuscript-to-EPUB">GitHub</a>

**ePub styles**
For TOD, you can access the style.epub.css file here:
there are options for tables,
adding a border around text 
you can remove the comments to apply styles.
update the hex (ie #FFFFFF) color values throughout the .css file to match the newest colors chosen in the print book.

## Glossary
markup: a system for annotating a document in a way that is syntactically distinguishable from the text. An example of this is in html is h1 for the most important heading, and # - a pound symbol to indicate a heading 1 in markdown. Authors or Editors can markup documents in Word or markdown.

markdown: is a lightweight markup language with plain text formatting syntax designed so that it can be converted to HTML, icml and many other formats.

InCopy: a professional word processor made by Adobe. InCopy lets copywriters and editors style text, track changes and make simple layout modifications to a document while designers work on the same document simultaneously in InDesign — all without overwriting each other's contributions.

icml: An ICML file is an InCopy Document by Adobe, it is XML-based.

idlk: InDesign Lock file it, indicates that a file is in use.

ePub: 