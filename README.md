# Žastikaulio lūžių klasifikavimas

Projektas skirtas automatizuotai aptikti ir lokalizuoti žastikaulio lūžius rentgenogramose, naudojant neuroninius tinklus.

## Sistemos veikimas

1. Surenkamos ir anonimizuojamos žastikaulio rentgenogramos.
2. Vaizdai paruošiami modelių mokymui.
3. `DenseNet161` nustato, ar rentgenogramoje yra lūžis.
4. `Grad-CAM` parodo modelio sprendimui svarbias vaizdo sritis.
5. `YOLOv8` ir `Faster R-CNN` lokalizuoja lūžio vietą.
6. Modeliai palyginami pagal jų vertinimo rodiklius.
7. Rezultatai pateikiami medicinos specialistui.

## Duomenys

Kataloge `data/` pateikiami rentgenogramų ir jų klasių `(X, y)` pavyzdžiai:

- `X` – žastikaulio rentgenograma;
- `y = 0` – lūžio nėra;
- `y = 1` – lūžis nustatytas.

Sistema skirta padėti medicinos specialistui, tačiau galutinį diagnostinį sprendimą priima gydytojas.
