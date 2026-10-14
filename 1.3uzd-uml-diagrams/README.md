
# UML diagramos

Šiame aplanke pateikiamos UML diagramos, vaizduojančios
žastikaulio lūžių aptikimo ir gydytojų konsultavimo
informacinės sistemos „RadiologyConsultAI“ architektūrą
bei generatyvinio dirbtinio intelekto (GDI) integravimo galimybes.

## Diagramos

### 1. Panaudojimo atvejų diagrama
Vaizduoja gydytojo ir konsultuojančio specialisto
sąveiką su informacine sistema.

### 2. Komponentų diagrama
Vaizduoja sistemos architektūrą, naudojamus
dirbtinio intelekto modelius ir numatomą
generatyvinio dirbtinio intelekto integraciją.

### 3. Sekos diagrama
Vaizduoja rentgenogramos apdorojimo procesą:
nuo vaizdo įkėlimo ir lūžio aptikimo iki
pirminio medicininio aprašo generavimo
ir gydytojo patvirtinimo.

## Naudojamos technologijos

- ASP.NET Core MVC – internetinė informacinė sistema.
- Python / FastAPI – dirbtinio intelekto modelių integracija.
- DenseNet161 – lūžio klasifikavimas.
- Faster R-CNN – lūžio lokalizavimas.
- Grad-CAM – DI sprendimų vizualizavimas.
- SQL Server – duomenų saugojimas.
- PlantUML – UML diagramų kūrimas.

## Generatyvinio dirbtinio intelekto integracija

Numatoma galimybė integruoti didįjį kalbos modelį (LLM),
kuris, remdamasis DI analizės rezultatais, generuotų
pirminio radiologinio aprašo projektą.

Sugeneruotą aprašą peržiūrėtų, prireikus redaguotų
ir patvirtintų gydytojas.

**Pastaba:** generatyvinio DI integracija yra siūlomas
sistemos išplėtimas, o ne šiuo metu įgyvendinta funkcija.
