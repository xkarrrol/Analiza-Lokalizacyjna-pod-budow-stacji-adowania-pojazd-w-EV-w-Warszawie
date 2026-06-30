# 📍 Analiza Lokalizacyjna (Site Selection) pod budowę stacji ładowania pojazdów EV w Warszawie

## 🎯 Cel projektu (Problem biznesowy)
Celem projektu było znalezienie **3 optymalnych lokalizacji** pod budowę nowych stacji ładowania pojazdów elektrycznych (EV) na terenie Warszawy dla dynamicznie rozwijającej się sieci ładowarek. Inwestycja wymagała precyzyjnego podejścia opartego na twardych danych przestrzennych, aby zminimalizować ryzyko nietrafionych lokalizacji i zmaksymalizować zyski z potoków kierowców.

---

## 🛠️ Kryteria decyzyjne i biznesowe
Analiza została przeprowadzona w oparciu o ścisłe wytyczne inwestorskie:
1. **Analiza konkurencji:** Wykluczenie obszarów w promieniu **500 metrów** od istniejących stacji ładowania EV (strefa ochrony przed kanibalizacją rynku).
2. **Generatory ruchu (POI):** Lokalizacja w promieniu do **300 metrów** od punktów użyteczności publicznej przyciągających klientów (centra handlowe, duże restauracje, hotele).
3. **Dostępność komunikacyjna:** Maksymalnie **150 metrów** od głównych arterii drogowych (krajowych, wojewódzkich i zbiorczych) dla zapewnienia łatwego dojazdu.

---

## 💾 Źródła danych
* **Dane przestrzenne (POI, drogi, istniejące stacje):** Pobrano z bazy **OpenStreetMap** przy użyciu wtyczki *QuickOSM*.
* **Granice administracyjne:** Państwowy Rejestr Granic pobrany z krajowego **Geoportalu** (GUGiK).

---

## ⚙️ Wykorzystane narzędzia (GIS Workflow)
Projekt został zrealizowany przy użyciu programu **QGIS / ArcGIS Pro**. W procesie analizy przestrzennej wykorzystano:
* **Buffer (Buforowanie):** Do wyznaczenia stref wpływu wokół dróg, POI oraz stref wykluczenia wokół konkurencji.
* **Intersection / Clip (Przecięcie / Przycinanie):** Operacje nakładkowe w celu znalezienia obszarów wspólnych spełniających wszystkie kryteria jednocześnie.
* **Select by Attribute / Location:** Do selekcji odpowiednich klas dróg oraz obiektów POI.
* **Layout Manager (Zarządca wydruków):** Przygotowanie finalnego arkusza mapy do celów biznesowych.

---

## 📊 Wyniki i Wnioski (Business Insights)
W wyniku zaawansowanej analizy nakładkowej (Overlay Analysis) wyznaczono spójną warstwę *"Obszar spełniający kryteria"*, w ramach której wskazano **3 konkretne, rekomendowane punkty (Punkt 1, Punkt 2, Punkt 3)**. 

Lokalizacje uwzględniają realny kontekst przestrzenny miasta (m.in. strategiczne obszary w rejonie Lotniska Chopina oraz południowych dzielnic w sąsiedztwie Lasu Kabackiego), łącząc wysoki potok kierowców z całkowitym brakiem bliskiej konkurencji.

### 🗺️ Wizualizacja projektu
<img width="3507" height="2480" alt="analiza_lokalizacyjna" src="https://github.com/user-attachments/assets/91d593d9-7e9f-478f-b5da-d6cfdbcf1fd1" />

