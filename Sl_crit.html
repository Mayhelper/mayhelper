<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Введите номер маршрута</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            background: white;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .container {
            width: 100%;
            padding: 5%;
        }
        
        h1 {
            color: #000;
            text-align: left;
            margin-bottom: 5%;
            font-size: 1.5em;
            font-weight: 600;
        }
        
        .input-group {
            width: 100%;
            margin-bottom: 5%;
        }
        
        input {
            width: 100%;
            padding: 4%;
            border: 0.2em solid #d32f2f;
            border-radius: 0.5em;
            font-size: 1em;
            background: white;
        }
        
        input:focus {
            outline: none;
            border-color: #b71c1c;
        }
        
        .btn-group {
            width: 100%;
            display: flex;
            gap: 4%;
            margin-bottom: 5%;
            flex-wrap: wrap;
        }
        
        .btn {
            flex: 1;
            padding: 4%;
            border: none;
            border-radius: 0.5em;
            font-size: 1em;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            min-width: 45%;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #ff6b6b, #d32f2f);
            color: white;
        }
        
        .btn-primary:hover {
            background: linear-gradient(135deg, #d32f2f, #b71c1c);
        }
        
        .btn-secondary {
            background: white;
            color: #d32f2f;
            border: 0.2em solid #d32f2f;
        }
        
        .btn-secondary:hover {
            background: #d32f2f;
            color: white;
        }
        
        .btn-tertiary {
            background: linear-gradient(135deg, #4CAF50, #45a049);
            color: white;
            margin-top: 3%;
        }
        
        .btn-tertiary:hover {
            background: linear-gradient(135deg, #45a049, #4CAF50);
        }
        
        .status {
            width: 100%;
            text-align: center;
            padding: 3%;
            margin: 4% 0;
            border-radius: 0.4em;
            font-weight: 500;
        }
        
        .loading {
            background: #ffebee;
            color: #d32f2f;
        }
        
        .error {
            background: #ffebee;
            color: #d32f2f;
        }
        
        .success {
            background: #f1f8e9;
            color: #2e7d32;
        }
        
        .table-container {
            width: 100%;
            margin-top: 5%;
            overflow-x: auto;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            border-radius: 0.5em;
            border: 0.2em solid #d32f2f;
            margin-bottom: 5%;
        }
        
        th, td {
            padding: 3%;
            text-align: left;
            border-bottom: 0.1em solid #e0e0e0;
            color: #000;
            font-size: 0.9em;
        }
        
        th {
            background: #d32f2f;
            color: white;
            font-weight: 600;
        }
        
        tr:hover {
            background-color: #ffebee;
        }
        
        tr:last-child td {
            border-bottom: none;
        }
        
        .total-row {
            background: #fff8e1;
            font-weight: bold;
        }
        
        .total-row td {
            border-top: 0.2em solid #ffa000;
        }
        
        .percentage-cell {
            font-weight: bold;
            text-align: center;
        }
        
        .percentage-high {
            color: #388e3c;
            background-color: #f1f8e9;
            padding: 0.3em 0.6em;
            border-radius: 0.3em;
        }
        
        .percentage-low {
            color: #d32f2f;
            background-color: #ffebee;
            padding: 0.3em 0.6em;
            border-radius: 0.3em;
        }

        .point-info {
            background: #f8f9fa;
            padding: 4%;
            border-radius: 0.5em;
            margin-bottom: 4%;
            border-left: 0.4em solid #4CAF50;
        }

        .point-info h4 {
            color: #2e7d32;
            margin-bottom: 2%;
        }

        .hidden {
            display: none;
        }

        /* Адаптация для очень маленьких экранов */
        @media (max-width: 480px) {
            .btn-group {
                flex-direction: column;
                gap: 3%;
            }
            
            .btn {
                width: 100%;
                min-width: auto;
            }
            
            th, td {
                padding: 2%;
                font-size: 0.8em;
            }
        }

        /* Для больших экранов */
        @media (min-width: 1200px) {
            .container {
                max-width: 50%;
            }
            
            th, td {
                padding: 2%;
                font-size: 1em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Введите номер маршрута</h1>
        
        <div class="input-group">
            <input type="text" id="routeInput" placeholder="Например, MKG_01" onkeypress="handleKeyPress(event)">
        </div>
        
        <div class="btn-group">
            <button class="btn btn-primary" onclick="updateTable()">Найти маршрут</button>
            <button class="btn btn-secondary" onclick="loadData()">Обновить данные</button>
        </div>
        
        <div id="status" class="status"></div>
        <div id="routeTable" class="table-container"></div>
        <div id="pointsButtonContainer" class="hidden">
            <button class="btn btn-tertiary" onclick="showPoints()">Показать все Точки</button>
        </div>
        <div id="pointsContainer" class="table-container"></div>
    </div>
    
    <script>
        const DATA_URL = 'https://docs.google.com/spreadsheets/d/e/2PACX-1vR5PsEoNd2yril2q-SPldvc3y7fClvJpIzfxwc79mHNTlVKB-h5sViWU501swo7ljssBmR8Gid73GIp/pub?gid=1830940219&single=true&output=csv';
        
        let routeData = [];
        let currentRoute = '';

        function handleKeyPress(event) {
            if (event.key === 'Enter') {
                updateTable();
            }
        }

        function parseCSV(csvText) {
            const rows = csvText.split('\n').filter(row => row.trim() !== '');
            if (rows.length === 0) return [];
            
            const headers = parseCSVRow(rows[0]);
            const result = [];
            
            for (let i = 1; i < rows.length; i++) {
                const values = parseCSVRow(rows[i]);
                if (values.length === headers.length) {
                    const item = {};
                    headers.forEach((header, index) => {
                        let value = values[index] || '';
                        item[header] = value;
                    });
                    result.push(item);
                }
            }
            return result;
        }

        function parseCSVRow(row) {
            const result = [];
            let current = '';
            let inQuotes = false;
            
            for (let i = 0; i < row.length; i++) {
                const char = row[i];
                
                if (char === '"' && (i === 0 || row[i-1] !== '\\')) {
                    inQuotes = !inQuotes;
                } else if (char === ',' && !inQuotes) {
                    result.push(current.trim());
                    current = '';
                } else {
                    current += char;
                }
            }
            result.push(current.trim());
            
            return result.map(field => field.replace(/^"(.*)"$/, '$1'));
        }

        function debugData() {
            console.log('Route Data:', routeData);
        }

        // Функция для форматирования процентных значений
        function formatPercentage(value) {
            // Преобразуем строку в число и округляем до двух знаков
            const num = parseFloat(value.replace('%', '').replace(',', '.'));
            return isNaN(num) ? 0 : Math.round(num * 100) / 100;
        }

        // Функция для определения класса в зависимости от значения процента
        function getPercentageClass(value) {
            const numValue = formatPercentage(value);
            return numValue >= 95 ? 'percentage-high' : 'percentage-low';
        }

        // Функция для расчета среднего значения
        function calculateAverage(value1, value2) {
            const num1 = formatPercentage(value1);
            const num2 = formatPercentage(value2);
            return ((num1 + num2) / 2).toFixed(2) + '%';
        }

        async function loadData() {
            const status = document.getElementById('status');
            status.innerHTML = '<div class="loading">Загрузка данных...</div>';
            
            try {
                const response = await fetch(DATA_URL + '&t=' + Date.now());
                if (!response.ok) throw new Error('Ошибка загрузки данных');
                
                const csvText = await response.text();
                if (!csvText) throw new Error('Пустые данные');
                
                routeData = parseCSV(csvText);
                
                // Отладочная информация
                debugData();
                
                status.innerHTML = '<div class="success">Данные загружены</div>';
                
            } catch (error) {
                console.error('Error loading data:', error);
                status.innerHTML = '<div class="error">Ошибка загрузки данных: ' + error.message + '</div>';
            }
        }

        function updateTable() {
            const route = document.getElementById('routeInput').value.trim();
            const tableContainer = document.getElementById('routeTable');
            const pointsButtonContainer = document.getElementById('pointsButtonContainer');
            
            if (!route) {
                tableContainer.innerHTML = '<div class="error">Введите маршрут</div>';
                pointsButtonContainer.classList.add('hidden');
                return;
            }
            
            if (!routeData.length) {
                tableContainer.innerHTML = '<div class="error">Данные не загружены</div>';
                pointsButtonContainer.classList.add('hidden');
                return;
            }
            
            // Фильтруем данные по маршруту (Маршрут1) для Индивидуальной цели по ЗП
            const zpFilteredData = routeData.filter(item => item.Маршрут1 === route);
            if (!zpFilteredData.length) {
                tableContainer.innerHTML = '<div class="error">Данные не найдены для маршрута: ' + route + '</div>';
                pointsButtonContainer.classList.add('hidden');
                return;
            }
            
            // Фильтруем данные по маршруту (Маршрут4) для Индивидуальной цели по ДП
            const dpFilteredData = routeData.filter(item => item.Маршрут4 === route);
            
            currentRoute = route;
            
            // Получаем данные для ЗП и ДП
            const zpData = zpFilteredData[0];
            const zpPlan = zpData['План_now1'] || '0';
            const zpFact = zpData['Текущий_факт1'] || '0';
            const zpPercentage = zpData['ID__выполнения1'] || '0%';
            
            let dpPlan = '0';
            let dpFact = '0';
            let dpPercentage = '0%';
            
            if (dpFilteredData.length > 0) {
                const dpData = dpFilteredData[0];
                dpPlan = dpData['Textbox562'] || '0';
                dpFact = dpData['Textbox572'] || '0';
                dpPercentage = dpData['ID__выполнения2'] || '0%';
            }
            
            // Рассчитываем среднее значение
            const averagePercentage = calculateAverage(zpPercentage, dpPercentage);
            
            // Создаем таблицу с данными
            let tableHTML = '<h3 style="color: #000; margin-bottom: 1em;">Маршрут: ' + route + '</h3><table>' + 
                '<tr><th>Задача</th><th>План</th><th>Факт</th><th>%</th><th>Итог</th></tr>';
            
            // Добавляем строку для Индивидуальная Цель по ЗП
            tableHTML += '<tr>' +
                '<td>Индивидуальная Цель по ЗП</td>' +
                '<td>' + zpPlan + '</td>' +
                '<td>' + zpFact + '</td>' +
                '<td class="percentage-cell ' + getPercentageClass(zpPercentage) + '">' + zpPercentage + '</td>' +
                '<td rowspan="2" class="percentage-cell ' + getPercentageClass(averagePercentage) + '">' + averagePercentage + '</td>' +
            '</tr>';
            
            // Добавляем строку для Индивидуальная цель по ДП
            tableHTML += '<tr>' +
                '<td>Индивидуальная цель по ДП</td>' +
                '<td>' + dpPlan + '</td>' +
                '<td>' + dpFact + '</td>' +
                '<td class="percentage-cell ' + getPercentageClass(dpPercentage) + '">' + dpPercentage + '</td>' +
            '</tr>';
            
            tableHTML += '</table>';
            tableContainer.innerHTML = tableHTML;
            pointsButtonContainer.classList.remove('hidden');
        }

        function showPoints() {
            if (!currentRoute) return;
            
            const pointsContainer = document.getElementById('pointsContainer');
            pointsContainer.innerHTML = '<div class="loading">Загрузка данных точек...</div>';
            
            // Фильтруем точки по маршруту (factMKB2)
            const routePoints = routeData.filter(item => item.factMKB2 === currentRoute);
            
            console.log('Found points for route', currentRoute, ':', routePoints);
            
            if (!routePoints.length) {
                pointsContainer.innerHTML = '<div class="error">Точки для маршрута ' + currentRoute + ' не найдены</div>';
                return;
            }
            
            let pointsHTML = '<h3 style="color: #000; margin-bottom: 1em;">Точки маршрута: ' + currentRoute + '</h3>';
            
            routePoints.forEach(point => {
                console.log('Point data:', point);
                
                // Получаем данные для отображения информации о точке
                const address = point['Кол_воЗадачПеревыполнение'] || 'Н/Д';
                const network = point['Маршрут1'] || 'Н/Д';
                const pointCode = point['factMKB1'] || 'Н/Д';
                
                // Фильтруем задачи для этой торговой точки по коду ТТ (factMKB1)
                const pointTasks = routeData.filter(item => item.factMKB1 === pointCode);
                
                // Находим задачи по ЗП и ДП
                const zpTask = pointTasks.find(item => item.Руководитель1 === 'Индивидуальная Цель по ЗП');
                const dpTask = pointTasks.find(item => item.Руководитель1 === 'Индивидуальная цель по ДП');
                
                pointsHTML += `
                    <div class="point-info">
                        <h4>Информация о точке</h4>
                        <p><strong>Адрес:</strong> ${address}</p>
                        <p><strong>Сеть:</strong> ${network}</p>
                        <p><strong>Код ТТ:</strong> ${pointCode}</p>
                    </div>
                `;
                
                pointsHTML += `
                    <table>
                        <tr><th>Задача</th><th>План</th><th>Факт</th><th>%</th></tr>
                `;
                
                // Добавляем строку для Индивидуальная цель по ЗП
                if (zpTask) {
                    const zpPlan = zpTask['ID__выполнения1'] || '0';
                    const zpFact = zpTask['Country1'] || '0';
                    const zpPercentage = zpTask['Дивизион6'] || '0%';
                    
                    pointsHTML += `
                        <tr>
                            <td>Индивидуальная цель по ЗП</td>
                            <td>${zpPlan}</td>
                            <td>${zpFact}</td>
                            <td class="percentage-cell ${getPercentageClass(zpPercentage)}">${zpPercentage}</td>
                        </tr>
                    `;
                } else {
                    pointsHTML += `
                        <tr>
                            <td>Индивидуальная цель по ЗП</td>
                            <td colspan="3">Данные не найдены</td>
                        </tr>
                    `;
                }
                
                // Добавляем строку для Индивидуальная цель по ДП
                if (dpTask) {
                    const dpPlan = dpTask['ID__выполнения1'] || '0';
                    const dpFact = dpTask['Country1'] || '0';
                    const dpPercentage = dpTask['Дивизион6'] || '0%';
                    
                    pointsHTML += `
                        <tr>
                            <td>Индивидуальная цель по ДП</td>
                            <td>${dpPlan}</td>
                            <td>${dpFact}</td>
                            <td class="percentage-cell ${getPercentageClass(dpPercentage)}">${dpPercentage}</td>
                        </tr>
                    `;
                } else {
                    pointsHTML += `
                        <tr>
                            <td>Индивидуальная цель по ДП</td>
                            <td colspan="3">Данные не найдены</td>
                        </tr>
                    `;
                }
                
                pointsHTML += `</table>`;
            });
            
            pointsContainer.innerHTML = pointsHTML;
        }

        document.addEventListener('DOMContentLoaded', loadData);
    </script>
</body>
</html>
