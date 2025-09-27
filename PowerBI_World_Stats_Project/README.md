# 🌍 Power BI – Analiza światowych wskaźników krajowych

## 📖 Opis
Projekt został wykonany w Power BI na podstawie danych CIA World Factbook.  
Dane zawierają dane demograficzne, społeczne i ekonomiczne według krajów świata. 

## 📂 Dane
W projekcie wykorzystano następujące zestawy danych:
- **people_and_society.tsv** – dane bazowe (wiek mediany, wskaźnik urodzeń, śmiertelność, oczekiwana długość życia, współczynnik dzietności, otyłość).  
- **education.csv** – wydatki na edukację (% PKB).  
- **military.csv** – wydatki na wojsko (% PKB).  
- **unemployment.csv** – stopa bezrobocia (% populacji aktywnej zawodowo).

## ⚙️ Kroki pracy
1. **Import danych** do Power BI i korekta błędów (zamiana symbolu `#` na separator dziesiętny, poprawa literówek w nazwach regionów).  
2. **Czyszczenie i łączenie** tabel (LEFT JOIN + dopasowania rozmyte po nazwach państw).  
3. **Budowa wizualizacji:**
   - Karty: liczba krajów, mediana wieku, max/min długość życia.  
   - Wykresy słupkowe: śmiertelność i urodzenia (TOP-10 krajów).  
   - Porównanie wydatków na edukację i współczynnika dzietności.  
   - Tabele wg regionów (mediana wieku + stopa bezrobocia).  
   - Mapy (wydatki wojskowe, poziom otyłości).  
   - Wykres punktowy: zależność wieku mediany i współczynnika dzietności.  
4. **Interaktywne filtry** (region, kraj).

## 📊 Wizualizacje
Przykłady raportów:  
- 📌 Liczba krajów i główne wskaźniki (karty).  
- 📌 Porównanie urodzeń i śmiertelności (bar chart).  
- 📌 Zależność edukacja ↔ dzietność.  
- 📌 Mapy wydatków na wojsko i otyłości.  
- 📌 Scatter plot: mediana wieku vs. dzietność. 

## 📁 Pliki
- [World_Stats_Project.pbix](./World_Stats_Project.pbix) – gotowy projekt Power BI.
- [World_Stats_Project.pdf](./World_Stats_Project.pdf)
- [people_and_society.tsv](./people_and_society.tsv)  
- [education.csv](./education.csv)  
- [military.csv](./military.csv)  
- [unemployment.csv](./unemployment.csv)
- [README.md](./README.md)


## ✅ Wnioski
- Wydatki na edukację silnie korelują z poziomem dzietności.  
- Kraje o wysokiej medianie wieku mają zazwyczaj niski poziom urodzeń.  
- Wskaźniki społeczne i ekonomiczne są często ze sobą powiązane (np. stopa bezrobocia i struktura demograficzna). 

### 📈 Analiza zależności: median_age vs. fertility_rate  

Wykres punktowy ze zmiennymi **fertility_rate** (współczynnik dzietności) oraz **median_age** (wiek mediany) ukazuje wyraźną **odwrotną zależność** pomiędzy tymi wskaźnikami.  

- Im wyższy jest median_age w danym kraju, tym niższy współczynnik dzietności.  
- Z kolei państwa o młodej strukturze demograficznej charakteryzują się wysoką dzietnością.  

🔎 **Interpretacja**:  
- W krajach rozwijających się, gdzie populacja jest stosunkowo młoda, rodziny są większe, a poziom urodzeń wyższy.  
- W krajach rozwiniętych, z wyższym median_age, obserwuje się spadek dzietności. Przyczyniają się do tego m.in.:  
  - upowszechnienie planowania rodziny,  
  - wyższy poziom edukacji,  
  - aktywność zawodowa kobiet,  
  - procesy urbanizacji.  

📌 Wniosek:  
Wykres potwierdza istnienie **silnej negatywnej korelacji** między strukturą wiekową społeczeństwa a poziomem dzietności. Jest to jedna z fundamentalnych prawidłowości demograficznych, obserwowana globalnie.  
