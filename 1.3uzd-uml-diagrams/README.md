# UML diagramos ir generatyvinio dirbtinio intelekto integracija

### Užduotis 1.3 – Įmonės pasirinkimas ir GDI integravimo į informacinę sistemą modeliavimas

Šiame dokumente pristatomas įmonės, kurios veikla susijusi su kuriamu
magistrinio darbo produktu, pasirinkimas ir generatyvinio dirbtinio
intelekto (GDI) integravimo į informacinę sistemą „RadiologyConsultAI“
galimybės.

Naudojant **PlantUML** parengtos trys UML diagramos, vaizduojančios
sistemos funkcionalumą, architektūrą ir GDI integravimo procesą.

---

## 1. Įmonės pasirinkimas

### Pasirinkta įmonė – „Aidoc“

| Informacija | Aprašymas |
|---|---|
| **Įmonė** | Aidoc |
| **Veiklos sritis** | Dirbtinio intelekto sprendimai medicininių vaizdų analizei |
| **Technologijų taikymas** | Radiologija, medicininių vaizdų analizė, klinikinių darbo procesų optimizavimas |
| **Oficiali svetainė** | https://www.aidoc.com/ |

### 1.1. Įmonės veiklos aprašymas

**„Aidoc“** – medicininių technologijų įmonė, kurianti dirbtiniu
intelektu pagrįstus sprendimus radiologijos ir kitoms sveikatos
priežiūros sritims.

Įmonės kuriamos technologijos padeda medicinos specialistams
analizuoti medicininius vaizdus, aptikti galimus patologinius
pakitimus ir efektyviau organizuoti klinikinius darbo procesus.

„Aidoc“ sprendimai gali būti integruojami su sveikatos priežiūros
įstaigų informacinėmis sistemomis, įskaitant medicininių vaizdų
archyvavimo ir perdavimo sistemas (PACS).

### 1.2. Įmonės pasirinkimo pagrindimas

„Aidoc“ pasirinkta todėl, kad jos veiklos kryptis glaudžiai
susijusi su magistrinio darbo metu kuriama informacine sistema
**„RadiologyConsultAI“**.

Abi sistemos orientuotos į dirbtinio intelekto panaudojimą
medicininių vaizdų analizei ir gydytojų sprendimų palaikymui.

#### „Aidoc“ ir „RadiologyConsultAI“ palyginimas

| „Aidoc“ veiklos kryptis | „RadiologyConsultAI“ funkcionalumas |
|---|---|
| Medicininių vaizdų analizė | Žastikaulio rentgenogramų analizė |
| Patologinių pakitimų aptikimas | Žastikaulio lūžių nustatymas |
| DI algoritmų naudojimas | DenseNet161, YOLO, Faster R-CNN ir Grad-CAM |
| DI rezultatų pateikimas specialistams | Lūžio tikimybės, lokalizacijos ir vizualizacijų pateikimas |
| Integracija į klinikinius darbo procesus | Gydytojų konsultacijos ir galutinių išvadų rengimas |
| Medicininių informacinių sistemų integravimas | ASP.NET Core MVC, FastAPI ir SQL Server |

**Išvada:** „Aidoc“ yra tinkamas pasirinkimas nagrinėjant
dirbtinio intelekto taikymą radiologijoje ir jo integravimo
į klinikinius procesus galimybes.

> **Pastaba:** „Aidoc“ pasirinkta kaip panašios veiklos įmonės
> pavyzdys. „RadiologyConsultAI“ nėra šios įmonės produktas,
> o jos technologijos nėra tiesiogiai integruotos į kuriamą sistemą.

---

## 2. Kuriamos informacinės sistemos pristatymas

### 2.1. „RadiologyConsultAI“ paskirtis

**„RadiologyConsultAI“** – magistrinio darbo metu kuriama
internetinė informacinė sistema, skirta automatizuotam
žastikaulio lūžių aptikimui, lokalizavimui ir gydytojų
sprendimų palaikymui naudojant rentgeno nuotraukas.

Sistemos tikslas – palengvinti medicininių vaizdų analizę,
pateikti gydytojui papildomą informaciją apie galimą lūžį
ir sudaryti sąlygas efektyvesniam klinikiniam vertinimui.

### 2.2. Pagrindinis funkcionalumas

Sistemoje numatytos ir įgyvendintos šios funkcijos:

1. Tyrimo atvejų kūrimas, redagavimas ir valdymas.
2. Rentgeno nuotraukų įkėlimas.
3. Automatizuota žastikaulio lūžių analizė.
4. Galimos lūžio vietos nustatymas.
5. DI rezultatų ir vizualizacijų pateikimas.
6. Gydytojų konsultacijų valdymas.
7. Galutinių medicininių aprašų rengimas.
8. Gydytojo išvadų peržiūra ir patvirtinimas.
9. Tyrimų audito istorijos ir statistikos peržiūra.
10. Galutinių aprašų eksportavimas PDF formatu.

### 2.3. Naudojamos technologijos

| Technologija | Paskirtis |
|---|---|
| **ASP.NET Core MVC** | Internetinės informacinės sistemos realizavimas |
| **C#** | Serverio logikos įgyvendinimas |
| **Python / FastAPI** | DI analizės tarnyba |
| **DenseNet161** | Rentgenogramų klasifikavimas |
| **Faster R-CNN** | Lūžio lokalizavimas |
| **YOLO** | Objektų aptikimas ir lokalizavimas |
| **Grad-CAM** | Klasifikavimo rezultatų vizualizavimas |
| **SQL Server** | Tyrimų ir analizės duomenų saugojimas |
| **PlantUML** | UML diagramų kūrimas |

---

## 3. Generatyvinio dirbtinio intelekto integracija

### 3.1. Esama dirbtinio intelekto analizė

Dabartinėje sistemoje naudojami giliaisiais neuroniniais
tinklais pagrįsti medicininių vaizdų analizės metodai.

**DenseNet161** naudojamas rentgenogramoms klasifikuoti
pagal galimo lūžio buvimą.

**Faster R-CNN ir YOLO** naudojami galimai lūžio vietai
aptikti bei lokalizuoti.

**Grad-CAM** naudojamas klasifikavimo modelio aktyvacijos
sritims vizualizuoti.

Papildomi modeliai leidžia nustatyti anatominę
žastikaulio sritį:

- Proksimalinė dalis – arčiau peties.
- Diafizė – žastikaulio kūnas.
- Distalinė dalis – arčiau alkūnės.

Gauti rezultatai pateikiami gydytojui, kuris juos gali
peržiūrėti ir panaudoti rengdamas medicininę išvadą.

### 3.2. Siūloma GDI integracija

Siekiant išplėsti sistemos galimybes, numatoma
integruoti **didelį kalbos modelį (LLM)**.

Pagrindinė šio komponento funkcija – automatiškai
parengti pirminio radiologinio aprašo projektą,
naudojant struktūrizuotus DI analizės rezultatus.

Numatomas veikimo principas:

**Rentgenograma → DI analizė → Struktūrizuoti rezultatai → LLM → Aprašo projektas → Gydytojo patvirtinimas**

LLM neanalizuotų rentgenogramos tiesiogiai. Jis gautų
specializuotų DI modelių apskaičiuotus rezultatus
ir pagal juos sugeneruotų tekstinį aprašo projektą.

### 3.3. Duomenų perdavimo pavyzdys

Pavyzdžiui, atlikus rentgenogramos analizę,
LLM galėtų būti perduodami tokie duomenys:

```json
{
  "fractureDetected": true,
  "fractureProbability": 0.94,
  "detectedZone": "Shaft",
  "detectionConfidence": 0.89
}
