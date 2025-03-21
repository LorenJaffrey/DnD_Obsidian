# Beschreibung

Sobald sich die Spieler nicht in der vorgegebenen Zeit nicht einigen können, entscheidet der Spielleiter über die Initiative Reihenfolge.
Dafür wird dieses Tool verwendet:

## Initiative Tool

[//]: # (needed to get cached path)
![[Argo_portrait.jpeg| 1 ]]

> [!column | 2  no-title]
>> <div style="font-family: Arial, sans-serif; background-color: transparent; display: flex; flex-direction: column; align-items: center; justify-content: center; height: 30vh;">
>> 	<div id="wheel" style="width: 300px; height: 300px; border: 2px solid black; border-radius: 50%; position: relative; overflow: hidden;">
>> 	    <!-- Glücksrad Segmente mit Bildern -->
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(0deg);">
>> 	        <img src="_Attachments/PCs/Aranon.jpg" alt="Aranon" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(60deg);">
>> 	        <img src="_Attachments/PCs/Argo.jpeg" alt="Argo" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(120deg);">
>> 	        <img src="_Attachments/NPCs/Baumel.png" alt="Baumel" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(180deg);">
>> 	        <img src="_Attachments/PCs/Drogan.jpeg" alt="Drogan" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(240deg);">
>> 	        <img src="_Attachments/PCs/Lucian.jpg" alt="Lucian" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	    <div class="wheel-segment" style="position: absolute; width: 50%; height: 50%; top: 0; left: 50%; transform-origin: 0% 100%; clip-path: polygon(50% 100%, 0 0, 100% 0); transform: rotate(300deg);">
>> 	        <img src="_Attachments/PCs/Niptac.jpeg" alt="Niptac" style="width: 100%; height: 100%; object-fit: cover; transform: rotate(-30deg);">
>> 	    </div>
>> 	</div>
>> 	<button id="spinButton" style="margin-top: 20px; padding: 10px 20px; font-size: 18px; cursor: pointer; background-color: rgb(101, 33, 33);">Start Randomator</button>
>> </div>
>
>> <table id="resultTable" style="margin-top: 20px; border-collapse: collapse;">
>>     <thead>
>>         <tr>
>>             <th style="border: 1px solid black; padding: 10px;">#</th>
>>             <th style="border: 1px solid black; padding: 10px;">Name</th>
>>         </tr>
>>     </thead>
>>     <tbody>
>>     </tbody>
>> </table>


```js-engine

function initRadarChart() {
	const spinButton = document.getElementById('spinButton');

    if (!spinButton) {
        // Retry after a short delay if the canvas is not yet in the DOM
        setTimeout(initRadarChart, 100);
        return;
    }

		const names = ['Aranon', 'Argo', 'Baumel', 'Drogan', 'Lucian', 'Niptac'];
        const wheel = document.getElementById('wheel');
        const resultTable = document.getElementById('resultTable').querySelector('tbody');

        spinButton.addEventListener('click', () => {
            // Clear previous results
            resultTable.innerHTML = '';

            // Randomize the names
            const randomizedNames = names
                .map(value => ({ value, sort: Math.random() }))
                .sort((a, b) => a.sort - b.sort)
                .map(({ value }) => value);

            // Simulate a spinning wheel animation
            let rotation = 0;
            const spinDuration = 3000; // Spin for 3 seconds
            const spinInterval = setInterval(() => {
                rotation += 5;
                wheel.style.transform = `rotate(${rotation}deg)`;
            }, 20);

            // Stop the spinning after a duration
            setTimeout(() => {
                clearInterval(spinInterval);
                displayResults(randomizedNames);
            }, spinDuration);
        });

        function displayResults(randomizedNames) {
            randomizedNames.forEach((name, index) => {
                const row = document.createElement('tr');
                const positionCell = document.createElement('td');
                const nameCell = document.createElement('td');

                positionCell.textContent = index + 1;
                positionCell.style.border = '1px solid black';
                positionCell.style.padding = '10px';
                
                nameCell.textContent = name;
                nameCell.style.border = '1px solid black';
                nameCell.style.padding = '10px';

                row.appendChild(positionCell);
                row.appendChild(nameCell);
                resultTable.appendChild(row);
            });
        }

	//add correct path to images
	const vaultPath = app.vault.adapter.basePath.replace(/\\\\/g, '').replace(/\\/g, '/');;
    const images = document.querySelectorAll('#wheel img');
    const referenceImage = document.querySelector('div > p > span > img[alt="Argo.jpeg"]')?.src ?? '';
    const appPart = referenceImage.split('/').slice(0, 3).join('/') + '/';

    images.forEach((img) => {
        const originalSrc = img.getAttribute('src');
        const startIndex = originalSrc.indexOf('_Attachments');

        if(startIndex !== -1) {
	        const outputString = originalSrc.substring(startIndex);
	        img.setAttribute('src', `${appPart}${vaultPath}/${outputString}`);
	    }
    });
}

initRadarChart();
```
