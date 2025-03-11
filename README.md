# sjpi-accessibility-1
**Mayday, Mayday – hjälp mig rädda webbplatsen!**

---

## Reflektion
Att göra den här uppgiften var både utmanande och lärorik. Det svåraste var att identifiera alla tillgänglighetsproblem som inte syntes direkt, som bristande kontrast eller saknade ARIA-attribut. Jag lärde mig hur viktigt det är att använda semantisk HTML och att testa sidan med verktyg som Lighthouse för att säkerställa att den är tillgänglig för alla användare. Att strukturera koden på ett sätt som är lätt att förstå och underhålla var också en viktig lärdom. Dessutom insåg jag hur viktigt det är att tänka på prestanda, till exempel genom att optimera bilder och videor.

---

## De 5 största problemen jag hittade (och hur jag fixade dem)

### 1. Bilder Saknade alt-attribut
- **Problem:** Bilder hade ingen beskrivning, vilket gör det svårt för skärmläsare att förstå vad de visar.
- **Lösning:** Jag la till alt-attribut med korta beskrivningar.

### 2. Dålig kontrast mellan text och bakgrund
- **Problem:** Texten var svår att läsa eftersom färgerna låg för nära varandra.
- **Lösning:** Jag ändrade färger i CSS så att texten syns tydligare.

### 3. Fel HTML-taggar (inte semantiska)
- **Problem:** Det användes `<div>` och `<span>` där det borde vara t.ex. `<nav>`, `<header>` eller `<button>`.
- **Lösning:** Jag bytte ut taggarna till mer tydliga, semantiska taggar, och la till ARIA-attribut.

### 4. Ingen fokusindikering
- **Problem:** När man använde tangentbordet kunde man inte se vilket element som var aktivt.
- **Lösning:** Jag la till CSS så att det syns tydligt vilket element som är i fokus.

### 5. Onödig JavaScript
- **Problem:** Det fanns gammal kod, som `document.write`, som inte behövdes och gjorde sidan långsammare.
- **Lösning:** Jag tog bort onödig kod och behöll bara det som faktiskt används.

---

## Sammanfattning
Genom att lösa dessa problem har sidan blivit mer tillgänglig, användarvänlig och prestandaoptimerad. Jag lärde mig att tillgänglighet inte bara handlar om att hjälpa användare med funktionsnedsättning, utan också om att skapa en bättre upplevelse för alla. Att använda verktyg som **Lighthouse** var ovärderligt för att identifiera och åtgärda problemen. Det här var en riktigt bra övning för mig som fortfarande lär mig grunderna i webbutveckling. Jag känner mig mycket säkrare på tillgänglighet nu än innan jag började.