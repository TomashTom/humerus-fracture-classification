# Duomenų pavyzdžiai

Šiamė pvz. pateikiu žastikaulio lūžių aptikimo ir klasifikavimo užduočių `(X, y)` pavyzdžiai.

- `X` – žastikaulio rentgenograma.
- `y` – rentgenogramos klasė arba lūžio vietos koordinatės.

## Klasifikavimas

Klasifikavimo užduotyje modeliui pateikiama rentgenograma, o rezultatas yra viena iš dviejų klasių:

- `y = 0` – žastikaulio lūžio nėra;
- `y = 1` – nustatytas žastikaulio lūžis.

Pavyzdys:

```text
X = žastikaulio rentgenograma
y = 1
```

## Lokalizavimas

Lokalizavimo užduotyje modeliui pateikiama rentgenograma, o `y` sudaro lūžio klasė ir pažymėtos lūžio srities koordinatės.

Pavyzdys:

```text
X = žastikaulio rentgenograma
y = [lūžio klasė, x_min, y_min, x_max, y_max]
```

„YOLOv8“ modeliui naudojamas normalizuotas žymėjimo formatas:

```text
<klasė> <x_centras> <y_centras> <plotis> <aukštis>
```

Pavyzdys:

```text
0 0.506 0.341 0.244 0.291
```

## Naudojami modeliai

- `DenseNet161` – lūžio klasifikavimas;
- `Grad-CAM` – modelio sprendimo paaiškinimas;
- `YOLOv8` – lūžio lokalizavimas;
- `Faster R-CNN` – papildomas lokalizavimo modelis palyginimui.

