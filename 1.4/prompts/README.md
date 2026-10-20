# Žastikaulio rentgenogramų analizės DI agentas

Šiame kataloge pateikiami žastikaulio rentgenogramų analizės DI agento užklausų pavyzdžiai.

Agentas veikia kaip vientisas sprendimas:

1. gauna žastikaulio rentgenogramą `X`;
2. patikrina ir paruošia vaizdą;
3. nustato, ar rentgenogramoje matomas lūžis;
4. aptikęs lūžį pažymi jo vietą;
5. nustato preliminarią lūžio anatominę zoną;
6. pateikia galutinį rezultatą `y`.

Sistemoje numatoma naudoti:

- `DenseNet161` – lūžio klasifikavimui;
- `Grad-CAM` – svarbioms vaizdo sritims parodyti;
- `YOLOv8` – lūžio vietai nustatyti;
- `Faster R-CNN` – lokalizavimo rezultatams palyginti.

## Įvestis ir rezultatas

- `X` – žastikaulio rentgenograma.
- `y` – lūžio klasė, tikimybė, vieta ir trumpas paaiškinimas.

Klasės:

- `0` – lūžio nėra;
- `1` – lūžis nustatytas.

Agentas yra pagalbinė priemonė. Galutinį diagnostinį sprendimą priima gydytojas.
