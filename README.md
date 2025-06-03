För att klona repo: ```git clone https://github.com/EliasKristmansson/dbt_rapport.git```.

För Windows: Följ instruktionerna från ChatGPT i bilden i messenger, och ladda ner Strawberry Perl för Windows.

För Mac: Perl ska komma med ert OS men om det inte gör det borde det finnas en Mac-download nånstans på internet. Annars ändra i Latex Workshops settings för en workaround: 
```
"latex-workshop.latex.tools": [
  {
    "name": "pdflatex",
    "command": "pdflatex",
    "args": [
      "-interaction=nonstopmode",
      "-file-line-error",
      "-synctex=1",
      "%DOC%"
    ]
  }
],
"latex-workshop.latex.recipes": [
  {
    "name": "pdflatex",
    "tools": ["pdflatex"]
  }
],
"latex-workshop.latex.autoBuild.run": "onSave"
```

Jag vet inte hur det blir för Mac med Latex-distro men med MikTeX (Windows) fick jag ett 20-tal popups när jag kompilerade Latex-koden i VSCode för att ladda ner packages lokalt. Det är bara att göra.
