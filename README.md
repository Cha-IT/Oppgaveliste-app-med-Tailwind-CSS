# **Oppgave: Lag en Enkel Oppgaveliste-app med Tailwind CSS**

### **Mål:**
- Lære å bruke Tailwind CSS for styling.
- Få praktisk erfaring med grunnleggende JavaScript for å håndtere brukerinteraksjoner.

### **Beskrivelse:**

Du skal lage en enkel **oppgaveliste-app** som lar brukeren legge til oppgaver i en liste og fjerne dem når de er fullført. Bruk **Tailwind CSS** for å style appen og **grunnleggende JavaScript** for å håndtere interaksjoner.

### **Krav til appen:**

1. **App Struktur:**
   - **Header:** En tittel for appen, som "Oppgaveliste".
   - **Input-felt:** Et tekstfelt der brukeren kan skrive inn oppgaver som skal legges til i listen.
   - **Legg til knapp:** En knapp for å legge til oppgaven fra input-feltet til oppgavelisten.
   - **Liste:** En liste som viser alle oppgavene som er lagt til, med en avkrysningsboks ved siden av hver oppgave for å markere dem som fullført.
   - **Footer:** En enkel footer med ekstra informasjon eller en melding.

2. **Styling med Tailwind CSS:**
   - **Header:** Bruk Tailwind-klasser for å gi headeren en passende bakgrunnsfarge og justere teksten.
   - **Input-felt og knapp:** Bruk Tailwind-klasser for å style input-feltet og knappen slik at de ser brukervennlige ut.
   - **Liste:** Stil listen og oppgavene i listen med Tailwind for å gi en enkel og ren layout.
   - **Responsiv design:** Sørg for at appen ser bra ut på både små og store skjermer ved å bruke Tailwinds responsive klasser.

### **Trinn for trinn:**

1. **Lag HTML-strukturen:**
   - Start med en enkel HTML-fil. Lag seksjoner for header, input-felt, liste, og footer.

   **Eksempel:**

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Oppgaveliste-app</title>
     <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
   </head>
   <body class="bg-gray-100 flex flex-col min-h-screen">
     <header class="bg-green-600 text-white text-center p-4">
       <h1 class="text-3xl font-bold">Oppgaveliste</h1>
     </header>
     <main class="flex-grow p-4">
       <div class="max-w-lg mx-auto">
         <div class="flex mb-4">
           <input id="taskInput" type="text" class="flex-grow p-2 border border-gray-300 rounded-l" placeholder="Skriv inn en oppgave">
           <button id="addButton" class="bg-green-500 text-white px-4 py-2 rounded-r">Legg til</button>
         </div>
         <ul id="taskList" class="list-disc pl-5"></ul>
       </div>
     </main>
     <footer class="bg-gray-800 text-white text-center p-4">
       <p>&copy; 2024 Oppgaveliste-app</p>
     </footer>
     <script src="app.js"></script>
   </body>
   </html>
   ```

2. **Legg til Tailwind CSS:**
   - Bruk Tailwind-klasser for å style elementene. Koden ovenfor gir en god start med bruk av Tailwind CSS for layout og styling.

3. **Legg til JavaScript:**
   - Lag en fil `app.js` og skriv JavaScript-kode for å håndtere legge-til funksjonen ved å bruke enklere metoder som `innerHTML`.

   **Eksempel:**

   ```javascript
   document.addEventListener('DOMContentLoaded', () => {
     const addButton = document.getElementById('addButton');
     const taskInput = document.getElementById('taskInput');
     const taskList = document.getElementById('taskList');

     addButton.addEventListener('click', () => {
       const taskText = taskInput.value.trim();
       if (taskText) {
         // Legg til oppgaven til listen
         const taskHTML = `
           <li class="flex items-center mb-2 p-2 bg-white border border-gray-300 rounded">
             <input type="checkbox" class="mr-2">
             ${taskText}
           </li>
         `;
         taskList.innerHTML += taskHTML;
         taskInput.value = '';
       }
     });
   });
   ```

4. **Test responsivitet:**
   - Test appen på forskjellige skjermstørrelser og sørg for at den ser bra ut på både mobil og desktop. Juster Tailwind-klasser for å håndtere responsiv design om nødvendig.

5. **Ferdigstilling:**
   - Gå gjennom appen din for å sikre at alle krav er oppfylt.
   - Sjekk at Tailwind CSS-klassene gir appen et rent og moderne utseende.

### **Ekstra utfordringer:**
- Legg til en funksjon for å fjerne oppgaver ved å legge til en "Fjern" knapp ved siden av hver oppgave.
- Implementer en funksjon for å lagre oppgavene i Local Storage slik at de beholdes etter at siden er oppdatert.

---

**Materialer:**
- [Tailwind CSS Dokumentasjon](https://tailwindcss.com/docs)
- [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)


---

Denne oppgaven bruker `innerHTML` for å legge til oppgaver til listen, noe som er lettere for nybegynnere å forstå og implementere.
