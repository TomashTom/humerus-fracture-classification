
# DI agento užklausų pavyzdžiai

Šiame kataloge pateikiami žastikaulio rentgenogramų analizės DI agento užklausų pavyzdžiai.

Agentas veikia kaip vientisas sprendimas:

1. gauna naują žastikaulio rentgenogramą `X`;
2. patikrina ir paruošia vaizdą;
3. nustato, ar matomas lūžis;
4. aptikęs lūžį pažymi jo vietą;
5. paaiškina, kurios vaizdo sritys turėjo įtakos sprendimui;
6. grąžina struktūrizuotą rezultatą `y`.

Numatomi sistemos komponentai:

- `DenseNet161` – lūžio klasifikavimas;
- `Grad-CAM` – svarbių vaizdo sričių parodymas;
- `YOLOv8` – lūžio vietos nustatymas;
- `Faster R-CNN` – papildomas lokalizavimo modelis palyginimui.

## Įvestis ir išvestis

- `X` – žastikaulio rentgenograma.
- `y` – klasė, lūžio tikimybė, lūžio vietos koordinatės ir trumpas paaiškinimas.

Klasės:

- `0` – lūžio nėra;
- `1` – lūžis nustatytas.

Sistema yra pagalbinė priemonė. Galutinį diagnostinį sprendimą priima gydytojas.
