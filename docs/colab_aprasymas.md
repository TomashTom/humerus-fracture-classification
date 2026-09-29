# „Colab“ dokumentų paaiškinimas

## 1. Vaizdo įrašų apdorojimas

Pirmasis „Colab“ dokumentas apdoroja vaizdo įrašus:

1. Duomenys atsisiunčiami iš „Kaggle“.
2. Iš vaizdo įrašų išskiriamas garsas.
3. „Whisper“ modelis garsą paverčia tekstu.
4. Iš kiekvieno vaizdo įrašo paimamas vidurinis kadras.
5. Rezultatai išsaugomi „Google Drive“.

Taip iš vieno vaizdo įrašo gaunami garso, teksto ir vaizdo duomenys.

## 2. Vaizdų aprašymų kūrimas

Antrasis „Colab“ dokumentas apdoroja iš vaizdo įrašų gautus kadrus:

1. Vaizdai įkeliami iš „Google Drive“.
2. Kiekvienas vaizdas perduodamas „Gemma“ modeliui.
3. Modelis sugeneruoja tekstinį vaizdo aprašymą.
4. Aprašymai išsaugomi tekstiniuose failuose.

## Ryšys su magistriniu darbu

Magistriniame darbe taikomas panašus procesas:

```text
Rentgenograma
→ vaizdo paruošimas
→ neuroninis tinklas
→ lūžio klasė ir vieta
→ rezultato pateikimas gydytojui
