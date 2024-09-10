# Lage en webside med Tailwind CSS

### Oppgave: Lag en Webside med Tailwind CSS

#### Mål:
- Lære det grunnleggende om hvordan du bruker Tailwind CSS for å style nettsider.
- Utforske Tailwind CSS for å lage en responsiv, stilren webside med minimal custom CSS.

### Del 1: Kom i gang med Tailwind CSS

1. **Opprett en enkel HTML-fil**.
   - Lag en HTML-fil som heter `index.html`.
   - Legg til en `<link>`-tagg i `<head>`-seksjonen for å inkludere Tailwind CSS via CDN:
     ```html
     <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
     ```

2. **Opprett strukturen for siden**.
   - Legg til følgende HTML-elementer på siden:
     - En tittel for nettsiden i et `<h1>`-element.
     - En kort introduksjon eller beskrivelse i et `<p>`-element.
     - Lag en navigasjonsmeny (`<nav>`) med lenker til minst tre ulike seksjoner på siden.
     - Opprett tre seksjoner som inneholder relevant innhold, f.eks. "Om oss", "Tjenester" og "Kontakt oss".
     - Legg til en footer som inneholder en lenke til en annen nettside, f.eks. skolens nettside.

### Del 2: Styling med Tailwind CSS

1. **Bruk Tailwind CSS for å style nettsiden**:
   - Bruk Tailwind-klasser til å style de ulike elementene på siden. Du må inkludere minst:
     - **Tekststørrelse og tekstfarger**: Bruk klasser som `text-xl`, `text-gray-700`, `text-center`, osv.
     - **Bakgrunnsfarger**: Legg til bakgrunnsfarger på seksjonene eller andre elementer ved hjelp av `bg-blue-500`, `bg-gray-100`, osv.
     - **Margin og padding**: Bruk `mt-4`, `px-6`, `py-8`, osv. for å justere mellomrom rundt og inni elementene.
     - **Rammer og avrundede hjørner**: Eksperimenter med `border`, `border-gray-400`, og `rounded-lg` for å legge til visuelle rammer og avrundede hjørner.
     - **Bilder**: Hvis du legger til bilder, bruk Tailwind-klasser som `rounded-full` for å gjøre bilder sirkulære.

### Del 3: Responsiv design

1. **Gjør nettsiden responsiv**:
   - Legg til Tailwinds responsive klasser for å sikre at siden ser bra ut på ulike skjermstørrelser:
     - Bruk klasser som `md:text-2xl` for å endre tekststørrelsen på større skjermer.
     - Bruk `grid`, `grid-cols-1`, `md:grid-cols-2`, osv. for å lage responsive kolonneoppsett.
     - Sørg for at bilder og tekst ser bra ut både på mobil og større skjermer.

### Del 4: Utforsk Tailwind CSS

1. **Utforsk og eksperimenter**:
   - Bruk Tailwinds **hover-effekter** for å lage interaktive elementer. F.eks. kan du bruke `hover:bg-blue-700` for å endre bakgrunnsfargen på knapper når man holder musepekeren over dem.
   - Bruk Tailwinds innebygde **flex** eller **grid system** for å lage mer avanserte layouts. Test ut `flex justify-center` eller `grid grid-cols-3`.
   - Legg til Tailwind's **skygge- og overgangseffekter** for å forbedre brukeropplevelsen. Du kan f.eks. bruke `shadow-lg` eller `transition duration-300`.

### Ekstra utfordring (valgfritt):
- Legg til en enkel knapp på siden som brukeren kan trykke på. Bruk Tailwind til å style knappen med forskjellige tilstander, som `hover`, `focus`, eller `active` effekter.
- Opprett en egen branch i GitHub, og bruk branches til å eksperimentere med endringer i designet.

---

### Krav:
- Bruk Tailwind CSS-klasser for å style alle elementer på nettsiden.
- Gjør nettsiden responsiv slik at den fungerer godt på både mobil og desktop.
- Siden skal være ryddig og ha en strukturert layout.

### Levering:
- Last opp prosjektet ditt til GitHub og del lenken med læreren din.
- Nettsiden skal også kunne publiseres via GitHub Pages for enkel deling og visning. 

Lykke til! 🎨
