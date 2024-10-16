---
cssclass: drwn, dvl-o, hc, h-line, k-o, table, t-c, t-w, tbl-nalt, tag-notion, tag-bubble, tag-outline, tag-text
Attribute:
  Stärke: 10
  Geschicklichkeit: 13
  Konstitution: 16
  Intelligenz: 12
  Weisheit: 10
  Charisma: 18
Rettungswürfe:
  Stärke: 0
  Geschicklichkeit: 0
  Konstitution: 1
  Intelligenz: 0
  Weisheit: 0
  Charisma: 1
Fertigkeiten:
  Akrobatik: 0
  Arkane_Kunde: 1
  Athletik: 0
  Auftreten: 0
  Einschüchtern: 0
  Fingerfertigkeit: 0
  Geschichte: 0
  Heilkunde: 0
  Heimlichkeit: 0
  Mit_Tieren_umgehen: 0
  Motiv_erkennen: 0
  Nachforschungen: 0
  Naturkunde: 1
  Religion: 1
  Täuschen: 0
  Überlebenskunst: 1
  Überzeugen: 0
  Wahrnehmung: 0
---

<canvas id="radarChart" width="400" height="400"  style="border: 1px solid #ccc;"></canvas>

```js-engine
//Radardiagramm

const staerke = context.metadata.frontmatter.Attribute.Stärke;
const geschicklichkeit = context.metadata.frontmatter.Attribute.Geschicklichkeit;
const konstitution = context.metadata.frontmatter.Attribute.Konstitution;
const intelligenz = context.metadata.frontmatter.Attribute.Intelligenz;
const weisheit = context.metadata.frontmatter.Attribute.Weisheit;
const charisma = context.metadata.frontmatter.Attribute.Charisma;

function initializeRadarChart() {
    const canvas = document.getElementById('radarChart');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: [staerke, geschicklichkeit, konstitution, intelligenz, weisheit, charisma],
        maxValue: 20
    };

    // Zentrum und Radius des Radardiagramms
    const centerX = canvas.width / 2;
    const centerY = canvas.height / 2;
    const radius = 150;

    // Anzahl der Eigenschaften
    const numAttributes = data.labels.length;

    // Zeichne das Radar mit Kreisen und Linien
    function drawRadar() {
        ctx.strokeStyle = '#999';
        ctx.lineWidth = 1;
        // Kreise zeichnen (Skalenringe)
        for (let i = 1; i <= 5; i++) {
            const currentRadius = (radius / 5) * i;
            ctx.beginPath();
            ctx.arc(centerX, centerY, currentRadius, 0, Math.PI * 2);
            ctx.stroke();
        }

        // Achsen zeichnen
        for (let i = 0; i < numAttributes; i++) {
            const angle = (Math.PI * 2 / numAttributes) * i;
            const x = centerX + Math.cos(angle) * radius;
            const y = centerY + Math.sin(angle) * radius;
            ctx.beginPath();
            ctx.moveTo(centerX, centerY);
            ctx.lineTo(x, y);
            ctx.stroke();

            // Fettgedruckte Beschriftung der Achsen
            ctx.fillStyle = '#ffffff';
            ctx.font = 'bold 14px Arial'; // Fettgedruckte Schriftart
            const labelX = centerX + Math.cos(angle) * (radius + 20);
            const labelY = centerY + Math.sin(angle) * (radius + 20);
            ctx.fillText(data.labels[i], labelX - 20, labelY + 5);
        }
    }

    // Zeichne die Datenlinie und schattiere den inneren Bereich
    function drawDataLine() {
        ctx.clearRect(0, 0, canvas.width, canvas.height); // Canvas löschen
        drawRadar(); // Das Radar erneut zeichnen

        // Schattierter Bereich
        ctx.fillStyle = 'rgba(0, 123, 255, 0.2)';
        ctx.beginPath();
        for (let i = 0; i < numAttributes; i++) {
            const value = data.values[i];
            const ratio = value / data.maxValue;
            const angle = (Math.PI * 2 / numAttributes) * i;
            const x = centerX + Math.cos(angle) * radius * ratio;
            const y = centerY + Math.sin(angle) * radius * ratio;

            if (i === 0) {
                ctx.moveTo(x, y);
            } else {
                ctx.lineTo(x, y);
            }
        }
        ctx.closePath();
        ctx.fill(); // Schattierung füllen

        // Linien zeichnen
        ctx.strokeStyle = '#007bff';
        ctx.lineWidth = 2;
        ctx.beginPath();
        for (let i = 0; i < numAttributes; i++) {
            const value = data.values[i];
            const ratio = value / data.maxValue;
            const angle = (Math.PI * 2 / numAttributes) * i;
            const x = centerX + Math.cos(angle) * radius * ratio;
            const y = centerY + Math.sin(angle) * radius * ratio;

            if (i === 0) {
                ctx.moveTo(x, y);
            } else {
                ctx.lineTo(x, y);
            }
        }
        ctx.closePath();
        ctx.stroke();

        // Punkte auf den Datenlinien zeichnen
        ctx.fillStyle = '#007bff';
        for (let i = 0; i < numAttributes; i++) {
            const value = data.values[i];
            const ratio = value / data.maxValue;
            const angle = (Math.PI * 2 / numAttributes) * i;
            const x = centerX + Math.cos(angle) * radius * ratio;
            const y = centerY + Math.sin(angle) * radius * ratio;
            ctx.beginPath();
            ctx.arc(x, y, 4, 0, Math.PI * 2);
            ctx.fill();
        }
    }

    // Radar zeichnen und Datenlinie anzeigen
    drawRadar();
    drawDataLine();
}

// Run the function
initializeRadarChart();

```