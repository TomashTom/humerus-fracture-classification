# 1.6 RAG sistemos demonstracija

Šiame kataloge pateikiama žastikaulio rentgenogramų analizės RAG sistema, sukurta naudojant „ChromaDB“, vaizdų embeddingus ir „Gemini API“.

Sistema naudoja 1 000 MURA `XR_HUMERUS` rentgenogramų. Naujai įvesčiai `X` surandami trys panašiausi pavyzdžiai, jų informacija įtraukiama į išplėstą promptą, o „Gemini“ sugeneruoja galutinį rezultatą `Y`.

Proceso eiga:

`Įvestis X → embeddingas → ChromaDB paieška → 3 panašiausi pavyzdžiai → RAG promptas → rezultatas Y`

> Rezultatai skirti tik mokymosi ir tyrimo tikslams ir nėra medicininė diagnozė.
