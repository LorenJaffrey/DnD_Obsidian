---
  Argo:
    Attribute:
      Stärke: 10
      Geschicklichkeit: 13
      Konstitution: 16
      Intelligenz: 12
      Weisheit: 10
      Charisma: 18
  Aranon:
    Attribute:
      Stärke: 8
      Geschicklichkeit: 14
      Konstitution: 14
      Intelligenz: 12
      Weisheit: 19
      Charisma: 11
  Lucian:
    Attribute:
      Stärke: 10
      Geschicklichkeit: 14
      Konstitution: 13
      Intelligenz: 14
      Weisheit: 8
      Charisma: 18
  Drogan:
    Attribute:
      Stärke: 18
      Geschicklichkeit: 14
      Konstitution: 16
      Intelligenz: 10
      Weisheit: 12
      Charisma: 8
  Niptac:
    Attribute:
      Stärke: 8
      Geschicklichkeit: 17
      Konstitution: 14
      Intelligenz: 14
      Weisheit: 10
      Charisma: 14
  Jon:
    Attribute:
      Stärke: 12
      Geschicklichkeit: 18
      Konstitution: 14
      Intelligenz: 8
      Weisheit: 14
      Charisma: 10
  Baumel:
    Attribute:
      Stärke: 8
      Geschicklichkeit: 14
      Konstitution: 10
      Intelligenz: 10
      Weisheit: 8
      Charisma: 8
---

> [!column | 3 flex  no-title]
>> <h2>Aranon</h2>
>> <canvas id="radarChartAranon" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Argo</h2>
>> <canvas id="radarChartArgo" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Drogan</h2>
>> <canvas id="radarChartDrogan" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Jon (☠)</h2>
>> <canvas id="radarChartJon" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Lucian</h2>
>> <canvas id="radarChartLucian" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Niptac</h2>
>> <canvas id="radarChartNiptac" width="400" height="400"  style="border: none;"></canvas>
>
>> <h2>Baumel (☠)</h2>
>> <canvas id="radarChartBaumel" width="400" height="400"  style="border: none;"></canvas>
>



```js-engine
//Radardiagramm
const metaData = context.metadata.frontmatter;
const attributes_Argo = [metaData.Argo.Attribute.Stärke, metaData.Argo.Attribute.Geschicklichkeit, metaData.Argo.Attribute.Konstitution, metaData.Argo.Attribute.Intelligenz, metaData.Argo.Attribute.Weisheit, metaData.Argo.Attribute.Charisma];
const attributes_Aranon = [metaData.Aranon.Attribute.Stärke, metaData.Aranon.Attribute.Geschicklichkeit, metaData.Aranon.Attribute.Konstitution, metaData.Aranon.Attribute.Intelligenz, metaData.Aranon.Attribute.Weisheit, metaData.Aranon.Attribute.Charisma];
const attributes_Drogan = [metaData.Drogan.Attribute.Stärke, metaData.Drogan.Attribute.Geschicklichkeit, metaData.Drogan.Attribute.Konstitution, metaData.Drogan.Attribute.Intelligenz, metaData.Drogan.Attribute.Weisheit, metaData.Drogan.Attribute.Charisma];
const attributes_Jon = [metaData.Jon.Attribute.Stärke, metaData.Jon.Attribute.Geschicklichkeit, metaData.Jon.Attribute.Konstitution, metaData.Jon.Attribute.Intelligenz, metaData.Jon.Attribute.Weisheit, metaData.Jon.Attribute.Charisma];
const attributes_Lucian = [metaData.Lucian.Attribute.Stärke, metaData.Lucian.Attribute.Geschicklichkeit, metaData.Lucian.Attribute.Konstitution, metaData.Lucian.Attribute.Intelligenz, metaData.Lucian.Attribute.Weisheit, metaData.Lucian.Attribute.Charisma];
const attributes_Niptac = [metaData.Niptac.Attribute.Stärke, metaData.Niptac.Attribute.Geschicklichkeit, metaData.Niptac.Attribute.Konstitution, metaData.Niptac.Attribute.Intelligenz, metaData.Niptac.Attribute.Weisheit, metaData.Niptac.Attribute.Charisma];
const attributes_Baumel = [metaData.Baumel.Attribute.Stärke, metaData.Baumel.Attribute.Geschicklichkeit, metaData.Baumel.Attribute.Konstitution, metaData.Baumel.Attribute.Intelligenz, metaData.Baumel.Attribute.Weisheit, metaData.Baumel.Attribute.Charisma];


function initializeRadarChart_Argo() {
    const canvas = document.getElementById('radarChartArgo');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Argo, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Argo,
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
        ctx.fillStyle = 'rgba(37, 139, 182, 0.2)';
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
        ctx.strokeStyle = '#258bb6';
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
        ctx.fillStyle = '#258bb6';
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

function initializeRadarChart_Aranon() {
    const canvas = document.getElementById('radarChartAranon');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Aranon, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Aranon,
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
        ctx.fillStyle = 'rgba(48, 181, 57, 0.2)';
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
        ctx.strokeStyle = '#30b539';
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
        ctx.fillStyle = '#30b539';
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

function initializeRadarChart_Drogan() {
    const canvas = document.getElementById('radarChartDrogan');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Drogan, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Drogan,
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
        ctx.fillStyle = 'rgba(224, 88, 88, 0.2)';
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
        ctx.strokeStyle = '#e05858';
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
        ctx.fillStyle = '#e05858';
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

function initializeRadarChart_Jon() {
    const canvas = document.getElementById('radarChartJon');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Jon, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Jon,
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
        ctx.fillStyle = 'rgba(255, 255, 255, 0.2)';
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
        ctx.strokeStyle = '#ffffff';
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
        ctx.fillStyle = '#ffffff';
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

function initializeRadarChart_Lucian() {
    const canvas = document.getElementById('radarChartLucian');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Lucian, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Lucian,
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
        ctx.fillStyle = 'rgba(194, 147, 46, 0.2)';
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
        ctx.strokeStyle = '#c2932e';
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
        ctx.fillStyle = '#c2932e';
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

function initializeRadarChart_Niptac() {
    const canvas = document.getElementById('radarChartNiptac');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Niptac, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Niptac,
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
        ctx.fillStyle = 'rgba(132, 84, 222, 0.2)';
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
        ctx.strokeStyle = '#8454de';
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
        ctx.fillStyle = '#8454de';
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

function initializeRadarChart_Baumel() {
    const canvas = document.getElementById('radarChartBaumel');
    if (!canvas) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initializeRadarChart_Baumel, 100);
        return;
    }

    const ctx = canvas.getContext('2d');

    // Werte für die Charaktere
    const data = {
        labels: ['Stärke', 'Geschicklichkeit', 'Konstitution', 'Intelligenz', 'Weisheit', 'Charisma'],
        //values: [10, 13, 16, 12, 10, 18],
        values: attributes_Baumel,
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
        ctx.fillStyle = 'rgba(168, 76, 50, 0.2)';
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
        ctx.strokeStyle = '#a84c32';
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
        ctx.fillStyle = '#a84c32';
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
initializeRadarChart_Argo();
initializeRadarChart_Aranon();
initializeRadarChart_Drogan();
initializeRadarChart_Jon();
initializeRadarChart_Lucian();
initializeRadarChart_Niptac();
initializeRadarChart_Baumel();

```