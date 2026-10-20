# Prompt 1 – paprastas „zero-shot“ pavyzdys

„Zero-shot“ atveju DI agentui pateikiama viena nauja rentgenograma be papildomų žinomų pavyzdžių.

## Įvestis X

Agentui pateikiama originali žastikaulio rentgenograma:

![Originali rentgenograma](zero_shot_input.png)

## Užklausa DI agentui

Išanalizuok pateiktą žastikaulio rentgenogramą kaip vientisas DI agentas.

Atlik šiuos veiksmus:

1. įvertink rentgenogramos kokybę;
2. nustatyk, ar joje matomas lūžis;
3. aptikęs lūžį pažymėk galimą jo vietą;
4. nustatyk preliminarią anatominę zoną;
5. pateik pasitikėjimo įverčius;
6. rezultatą pateik struktūrizuotu JSON formatu.

## Gautas rezultatas y

![DI agento rezultatas](zero_shot_output.png)

```json
{
  "fracture_detected": true,
  "predicted_zone": "shaft",
  "zone_overlap": 0.481,
  "detections": [
    {
      "label": "galima lūžio vieta",
      "confidence": 0.873
    },
    {
      "label": "galima lūžio vieta",
      "confidence": 0.546
    }
  ],
  "recommendation": "Rezultatą turi patvirtinti gydytojas."
}
```

## Rezultato paaiškinimas

Agentas rentgenogramoje aptiko galimą žastikaulio lūžį. Didžiausias lūžio aptikimo pasitikėjimas siekė 87,3 %. Didžiausias aptiktos srities persidengimas nustatytas su žastikaulio kūno (`shaft`) zona ir siekė 48,1 %.

Sistema pateikia pagalbinį rezultatą, tačiau galutinį diagnostinį sprendimą turi priimti gydytojas.
