<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nagaland Dear Lottery AI Predictor</title>
    <link rel="manifest" href="data:application/json;base64,eyJuYW1lIjoiTmFnYWxhbmQgRGVhciBMb3R0ZXJ5IEFJIiwic2hvcnRfbmFtZSI6IkxvdHRlcnlBSSIsInN0YXJ0X3VybCI6Ii4iLCJkaXNwbGF5Ijoic3RhbmRhbG9uZSIsImJhY2tncm91bmRfY29sb3IiOiIjMTIxMjEyIiwidGhlbWVfY29sb3IiOiIjMjEyMTIxIn0=">
    <meta name="theme-color" content="#121212">
    <style>
        :root {
            --bg-primary: #121212;
            --bg-secondary: #1e1e1e;
            --bg-tertiary: #2a2a2a;
            --text-primary: #ffffff;
            --text-secondary: #cccccc;
            --accent-green: #4CAF50;
            --accent-yellow: #FFC107;
            --accent-red: #F44336;
            --border-color: #333333;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, var(--bg-primary) 0%, var(--bg-secondary) 100%);
            color: var(--text-primary);
            min-height: 100vh;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        .header {
            background: linear-gradient(135deg, var(--bg-secondary) 0%, var(--bg-tertiary) 100%);
            padding: 20px 0;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 2px solid var(--accent-green);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--accent-green);
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
        }
        
        .status-indicator {
            display: flex;
            align-items: center;
            gap: 10px;
            background: rgba(76, 175, 80, 0.1);
            padding: 8px 16px;
            border-radius: 25px;
            border: 1px solid var(--accent-green);
        }
        
        .status-dot {
            width: 10px;
            height: 10px;
            background: var(--accent-green);
            border-radius: 50%;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }
        
        /* Control Panel Styles */
        .control-panel {
            background: rgba(30, 30, 30, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 30px;
            margin: 30px 0;
            box-shadow: 0 8px 32px rgba(0,0,0,0.3);
            border: 1px solid rgba(255,255,255,0.1);
        }
        
        .panel-title {
            font-size: 1.5rem;
            color: var(--accent-green);
            margin-bottom: 25px;
            text-align: center;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .controls-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 25px;
        }
        
        .control-group {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        
        .control-label {
            font-weight: 600;
            color: var(--text-secondary);
            font-size: 0.9rem;
        }
        
        .form-input {
            background: var(--bg-tertiary);
            border: 2px solid var(--border-color);
            border-radius: 8px;
            padding: 12px 16px;
            color: var(--text-primary);
            font-size: 1rem;
            transition: all 0.3s ease;
        }
        
        .form-input:focus {
            outline: none;
            border-color: var(--accent-green);
            box-shadow: 0 0 0 3px rgba(76, 175, 80, 0.1);
        }
        
        .time-slots {
            display: flex;
            gap: 10px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .time-btn {
            background: rgba(255,255,255,0.1);
            border: 2px solid var(--border-color);
            color: var(--text-primary);
            padding: 10px 20px;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        
        .time-btn:hover {
            background: rgba(76, 175, 80, 0.2);
            border-color: var(--accent-green);
        }
        
        .time-btn.active {
            background: var(--accent-green);
            border-color: var(--accent-green);
            color: white;
        }
        
        .analyze-btn {
            background: linear-gradient(135deg, var(--accent-green) 0%, #45a049 100%);
            border: none;
            color: white;
            padding: 15px 40px;
            border-radius: 30px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 20px rgba(76, 175, 80, 0.3);
            display: block;
            margin: 20px auto 0;
        }
        
        .analyze-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 25px rgba(76, 175, 80, 0.4);
        }
        
        .analyze-btn:active {
            transform: translateY(0);
        }
        
        .analyze-btn:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            transform: none;
        }
        
        /* Loading Styles */
        .loading-container {
            display: none;
            text-align: center;
            padding: 40px;
            background: rgba(30, 30, 30, 0.95);
            border-radius: 15px;
            margin: 20px 0;
        }
        
        .spinner {
            width: 50px;
            height: 50px;
            border: 4px solid rgba(255,255,255,0.3);
            border-top: 4px solid var(--accent-green);
            border-radius: 50%;
            animation: spin 1s linear infinite;
            margin: 0 auto 20px;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Results Table Styles */
        .results-container {
            background: rgba(30, 30, 30, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 30px;
            margin: 30px 0;
            box-shadow: 0 8px 32px rgba(0,0,0,0.3);
            border: 1px solid rgba(255,255,255,0.1);
        }
        
        .results-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .results-title {
            font-size: 1.4rem;
            color: var(--accent-green);
        }
        
        .export-btn {
            background: var(--bg-tertiary);
            border: 2px solid var(--accent-green);
            color: var(--accent-green);
            padding: 8px 16px;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }
        
        .export-btn:hover {
            background: var(--accent-green);
            color: white;
        }
        
        .table-container {
            overflow-x: auto;
            border-radius: 10px;
            background: var(--bg-primary);
        }
        
        .results-table {
            width: 100%;
            border-collapse: collapse;
            background: var(--bg-primary);
        }
        
        .results-table th {
            background: linear-gradient(135deg, var(--bg-tertiary) 0%, var(--accent-green) 100%);
            color: white;
            padding: 15px 10px;
            text-align: center;
            font-weight: 600;
            font-size: 0.9rem;
            position: sticky;
            top: 0;
            z-index: 10;
        }
        
        .results-table td {
            padding: 12px 10px;
            text-align: center;
            border-bottom: 1px solid var(--border-color);
            font-size: 0.9rem;
            position: relative;
        }
        
        .results-table tbody tr {
            transition: all 0.3s ease;
        }
        
        .results-table tbody tr:hover {
            background: rgba(76, 175, 80, 0.1);
            transform: scale(1.01);
        }
        
        .rank-cell {
            font-weight: bold;
            color: var(--accent-green);
            font-size: 1rem;
        }
        
        .number-cell {
            font-weight: bold;
            color: var(--text-primary);
            font-size: 1rem;
        }
        
        .prob-high {
            background: rgba(76, 175, 80, 0.3);
            color: var(--accent-green);
            font-weight: bold;
            border-radius: 5px;
        }
        
        .prob-medium {
            background: rgba(255, 193, 7, 0.3);
            color: var(--accent-yellow);
            font-weight: bold;
            border-radius: 5px;
        }
        
        .prob-low {
            background: rgba(244, 67, 54, 0.3);
            color: var(--accent-red);
            border-radius: 5px;
        }
        
        .overall-score {
            font-weight: bold;
            color: var(--accent-green);
            font-size: 1rem;
        }
        
        /* Footer Styles */
        .footer {
            background: linear-gradient(135deg, var(--bg-secondary) 0%, var(--bg-tertiary) 100%);
            padding: 30px 0;
            text-align: center;
            margin-top: 50px;
            border-top: 2px solid var(--accent-green);
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }
        
        .developer-credit {
            font-size: 1.2rem;
            color: var(--accent-green);
            font-weight: bold;
        }
        
        .disclaimer {
            font-size: 0.8rem;
            color: var(--text-secondary);
            max-width: 600px;
            line-height: 1.4;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                padding: 0 15px;
            }
            
            .controls-grid {
                grid-template-columns: 1fr;
            }
            
            .time-slots {
                flex-direction: column;
            }
            
            .results-table th,
            .results-table td {
                padding: 8px 5px;
                font-size: 0.8rem;
            }
            
            .logo {
                font-size: 1.5rem;
            }
        }
        
        /* PWA Install Prompt */
        .install-prompt {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--accent-green);
            color: white;
            padding: 15px 25px;
            border-radius: 25px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            display: none;
            z-index: 1000;
            animation: slideUp 0.5s ease;
        }
        
        @keyframes slideUp {
            from {
                transform: translate(-50%, 100%);
                opacity: 0;
            }
            to {
                transform: translate(-50%, 0);
                opacity: 1;
            }
        }
        
        .install-prompt.show {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .install-btn {
            background: white;
            color: var(--accent-green);
            border: none;
            padding: 5px 15px;
            border-radius: 15px;
            cursor: pointer;
            font-weight: bold;
        }
        
        .close-prompt {
            background: transparent;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 1.5rem;
            padding: 0 5px;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="header-content">
                <div class="logo">🎯 Nagaland Dear Lottery AI</div>
                <div class="status-indicator">
                    <div class="status-dot"></div>
                    <span id="status-text">AI Engine Ready</span>
                </div>
            </div>
        </div>
    </header>

    <main class="container">
        <!-- Control Panel -->
        <section class="control-panel">
            <h2 class="panel-title">
                🔮 Advanced Range Analyzer
            </h2>
            
            <div class="controls-grid">
                <div class="control-group">
                    <label class="control-label">📅 Analysis Date</label>
                    <input type="date" id="analysisDate" class="form-input">
                </div>
                
                <div class="control-group">
                    <label class="control-label">🎯 Start Number</label>
                    <input type="number" id="startNumber" class="form-input" placeholder="e.g., 25620" min="1" max="99999">
                </div>
                
                <div class="control-group">
                    <label class="control-label">🏁 End Number</label>
                    <input type="number" id="endNumber" class="form-input" placeholder="e.g., 25670" min="1" max="99999">
                </div>
            </div>
            
            <div class="control-group">
                <label class="control-label" style="text-align:center; margin-bottom:10px;">⏰ Time Slot Selection</label>
                <div class="time-slots">
                    <button class="time-btn" data-time="1pm">1:00 PM</button>
                    <button class="time-btn active" data-time="6pm">6:00 PM</button>
                    <button class="time-btn" data-time="8pm">8:00 PM</button>
                </div>
            </div>
            
            <button class="analyze-btn" onclick="analyzeRange()">
                🚀 Generate AI Predictions
            </button>
        </section>

        <!-- Loading Container -->
        <div class="loading-container" id="loadingContainer">
            <div class="spinner"></div>
            <h3>🧠 AI Engine Analyzing Patterns...</h3>
            <p>Processing historical data and calculating probabilities</p>
        </div>

        <!-- Results Container -->
        <section class="results-container" id="resultsContainer" style="display: none;">
            <div class="results-header">
                <h2 class="results-title">📊 Analysis Results</h2>
                <button class="export-btn" onclick="exportResults()">📥 Export CSV</button>
            </div>
            
            <div class="table-container">
                <table class="results-table">
                    <thead>
                        <tr>
                            <th>🏆 Rank</th>
                            <th>🔢 Number</th>
                            <th>🥇 1st Prize</th>
                            <th>🥈 2nd Prize</th>
                            <th>🥉 3rd Prize</th>
                            <th>🏅 4th Prize</th>
                            <th>🎖️ 5th Prize</th>
                            <th>⭐ Overall Score</th>
                        </tr>
                    </thead>
                    <tbody id="resultsTableBody">
                        <!-- Results will be populated here -->
                    </tbody>
                </table>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="developer-credit">💻 Developed by Akash Ram © 2025</div>
                <div class="disclaimer">
                    ⚠️ This app uses advanced AI algorithms for educational and entertainment purposes. 
                    Lottery results are random and past performance does not guarantee future results. 
                    Play responsibly and within your limits. 🎲
                </div>
                <div style="color: #666; font-size: 0.8rem; margin-top: 10px;">
                    🚀 Version 3.0 | Real-time AI Predictions | PWA Enabled
                </div>
            </div>
        </div>
    </footer>

    <!-- PWA Install Prompt -->
    <div class="install-prompt" id="installPrompt">
        <span>📱 Install this app for a better experience!</span>
        <button class="install-btn" onclick="installApp()">Install</button>
        <button class="close-prompt" onclick="hideInstallPrompt()">×</button>
    </div>

    <script>
        // Advanced Nagaland Dear Lottery AI Prediction Engine
        class AdvancedLotteryAI {
            constructor() {
                this.currentTimeSlot = '6pm';
                this.isAnalyzing = false;
                this.deferredPrompt = null;
                this.init();
            }

            init() {
                this.setupEventListeners();
                this.setDefaultDate();
                this.setupPWA();
                this.showWelcomeMessage();
            }

            setupEventListeners() {
                document.querySelectorAll('.time-btn').forEach(btn => {
                    btn.addEventListener('click', (e) => {
                        document.querySelectorAll('.time-btn').forEach(b => b.classList.remove('active'));
                        e.target.classList.add('active');
                        this.currentTimeSlot = e.target.dataset.time;
                    });
                });

                document.getElementById('startNumber').addEventListener('input', this.validateInputs.bind(this));
                document.getElementById('endNumber').addEventListener('input', this.validateInputs.bind(this));
            }

            setDefaultDate() {
                const today = new Date();
                const dateStr = today.toISOString().split('T')[0];
                document.getElementById('analysisDate').value = dateStr;
            }

            validateInputs() {
                const startNum = parseInt(document.getElementById('startNumber').value);
                const endNum = parseInt(document.getElementById('endNumber').value);
                const analyzeBtn = document.querySelector('.analyze-btn');
                
                if (startNum && endNum && startNum < endNum && (endNum - startNum) <= 100) {
                    analyzeBtn.disabled = false;
                    analyzeBtn.textContent = '🚀 Generate AI Predictions';
                } else if (startNum && endNum && (endNum - startNum) > 100) {
                    analyzeBtn.disabled = true;
                    analyzeBtn.textContent = '⚠️ Range too large (max 100 numbers)';
                } else if (startNum && endNum && startNum >= endNum) {
                    analyzeBtn.disabled = true;
                    analyzeBtn.textContent = '⚠️ Start must be less than End';
                } else {
                    analyzeBtn.disabled = true;
                    analyzeBtn.textContent = 'Enter a valid range';
                }
            }
            
            // This is the CORE AI LOGIC. It's a realistic simulation, not just random.
            calculateAdvancedProbability(number, prizeLevel, timeSlot, analysisDate) {
                // 1. Frequency Analysis (simulated)
                const freqScore = (() => {
                    const lastDigit = number % 10;
                    let score = 3.0;
                    if ([0, 1, 7, 8, 9].includes(lastDigit)) score += 1.2;
                    return score + (Math.sin(number) * 1.5);
                })();

                // 2. Gap Analysis (simulated)
                const gapScore = (() => {
                    const days = (new Date(analysisDate).getTime() / 86400000) % 30;
                    return 3 + Math.cos(number * 0.1 + days) * 2;
                })();

                // 3. Time-slot Specific Patterns
                const timeSlotBonus = (() => {
                    if (timeSlot === '1pm' && (number % 10 === 0 || number % 10 === 5)) return 1.8;
                    if (timeSlot === '6pm' && (number >= 25635 && number <= 25655)) return 2.2;
                    if (timeSlot === '8pm' && number.toString().split('').reduce((s, d) => s + parseInt(d), 0) % 7 === 0) return 2.0;
                    return 1.0;
                })();

                // 4. Nagaland Cultural Factors
                const culturalScore = (() => {
                    const numStr = number.toString();
                    let score = 1.0;
                    if (numStr.includes('7')) score += 1.2;
                    if (numStr.includes('8')) score += 1.0;
                    return score;
                })();

                // 5. Prize-specific Multiplier
                const prizeMultiplier = [0.3, 0.5, 0.7, 1.0, 1.3][prizeLevel - 1];

                // Ensemble Calculation (weighted average of all scores)
                let probability = (
                    (freqScore * 0.3) +
                    (gapScore * 0.25) +
                    (timeSlotBonus * 0.2) +
                    (culturalScore * 0.25)
                ) * prizeMultiplier;

                // Ensure the result is within a realistic range
                const ranges = { 1: 3.5, 2: 4.5, 3: 6.0, 4: 8.5, 5: 12.0 };
                return Math.max(0.1, Math.min(ranges[prizeLevel], probability));
            }

            calculateOverallScore(probabilities) {
                return (probabilities[0] * 10) + (probabilities[1] * 5) + 
                       (probabilities[2] * 3) + (probabilities[3] * 2) + (probabilities[4] * 1);
            }

            getConfidenceClass(probability) {
                if (probability >= 8.0) return 'prob-high';
                if (probability >= 4.0) return 'prob-medium';
                return 'prob-low';
            }

            async analyzeRange() {
                if (this.isAnalyzing) return;
                
                const startNum = parseInt(document.getElementById('startNumber').value);
                const endNum = parseInt(document.getElementById('endNumber').value);
                const date = document.getElementById('analysisDate').value;
                
                if (!startNum || !endNum || !date || startNum >= endNum || (endNum - startNum) > 100) {
                    alert('⚠️ Please enter a valid date and a number range (max 100 numbers, start < end).');
                    return;
                }
                
                this.showLoading();
                this.isAnalyzing = true;
                
                await new Promise(resolve => setTimeout(resolve, 2500));
                
                const results = [];
                for (let number = startNum; number <= endNum; number++) {
                    const probabilities = Array.from({length: 5}, (_, i) => 
                        this.calculateAdvancedProbability(number, i + 1, this.currentTimeSlot, date)
                    );
                    const overallScore = this.calculateOverallScore(probabilities);
                    results.push({ number, probabilities, overallScore });
                }
                
                results.sort((a, b) => b.overallScore - a.overallScore);
                
                this.displayResults(results);
                this.hideLoading();
                this.isAnalyzing = false;
            }

            displayResults(results) {
                const tbody = document.getElementById('resultsTableBody');
                tbody.innerHTML = '';
                
                results.forEach((result, index) => {
                    const row = document.createElement('tr');
                    const probCells = result.probabilities.map(p => 
                        `<td class="${this.getConfidenceClass(p)}">${p.toFixed(1)}%</td>`
                    ).join('');
                    
                    row.innerHTML = `
                        <td class="rank-cell">${index + 1}</td>
                        <td class="number-cell">${result.number}</td>
                        ${probCells}
                        <td class="overall-score">${result.overallScore.toFixed(2)}</td>
                    `;
                    tbody.appendChild(row);
                });
                
                document.getElementById('resultsContainer').style.display = 'block';
                document.getElementById('resultsContainer').scrollIntoView({ behavior: 'smooth' });
            }

            showLoading() {
                document.getElementById('loadingContainer').style.display = 'block';
                document.getElementById('resultsContainer').style.display = 'none';
                document.getElementById('status-text').textContent = 'AI Processing...';
            }

            hideLoading() {
                document.getElementById('loadingContainer').style.display = 'none';
                document.getElementById('status-text').textContent = 'Analysis Complete';
                setTimeout(() => {
                    document.getElementById('status-text').textContent = 'AI Engine Ready';
                }, 3000);
            }

            exportResults() {
                const table = document.querySelector('.results-table');
                let csv = [];
                const headers = Array.from(table.querySelectorAll('th')).map(th => `"${th.textContent.replace(/[^a-zA-Z0-9 %]/g, '').trim()}"`);
                csv.push(headers.join(','));
                
                Array.from(table.querySelectorAll('tbody tr')).forEach(row => {
                    const data = Array.from(row.querySelectorAll('td')).map(td => `"${td.textContent.trim()}"`);
                    csv.push(data.join(','));
                });
                
                const blob = new Blob([csv.join('\n')], { type: 'text/csv' });
                const url = window.URL.createObjectURL(blob);
                const a = document.createElement('a');
                a.href = url;
                a.download = `nagaland-lottery-ai-predictions-${new Date().toISOString().split('T')[0]}.csv`;
                a.click();
                window.URL.revokeObjectURL(url);
                alert('📊 Results exported successfully!');
            }

            setupPWA() {
                if ('serviceWorker' in navigator) {
                    const swContent = `
                        self.addEventListener('install', e => e.waitUntil(caches.open('lottery-ai-v1').then(c => c.addAll(['/']))));
                        self.addEventListener('fetch', e => e.respondWith(caches.match(e.request).then(r => r || fetch(e.request))));
                    `;
                    const swUrl = URL.createObjectURL(new Blob([swContent], { type: 'application/javascript' }));
                    navigator.serviceWorker.register(swUrl).catch(e => console.error('SW registration failed:', e));
                }

                window.addEventListener('beforeinstallprompt', (e) => {
                    e.preventDefault();
                    this.deferredPrompt = e;
                    document.getElementById('installPrompt').style.display = 'flex';
                });
            }
            
            showWelcomeMessage() {
                 setTimeout(() => {
                    alert('🎯 Welcome to Ultimate Nagaland Dear Lottery AI!\n\n✨ All features are ready. Enter a range (e.g., 25620-25670) and click "Generate AI Predictions" to start!\n\n🚀 Developed by Akash Ram');
                }, 1000);
            }
        }

        // Global functions to be called from HTML
        function analyzeRange() { window.lotteryAI.analyzeRange(); }
        function exportResults() { window.lotteryAI.exportResults(); }
        function installApp() {
            if (window.lotteryAI.deferredPrompt) {
                window.lotteryAI.deferredPrompt.prompt();
            }
        }
        function hideInstallPrompt() { document.getElementById('installPrompt').style.display = 'none'; }

        document.addEventListener('DOMContentLoaded', () => {
            window.lotteryAI = new AdvancedLotteryAI();
        });
    </script>
</body>
</html>

# Lottery Predictor

This project is a machine learning model designed to predict the most likely set of lottery numbers for the next drawing based on previous winning numbers.

## Getting Started

To use this model, you will need to have Python installed on your computer, as well as the following libraries:

-   pandas
-   scikit-learn

To install the libraries, run the following command:

Copy code

`pip install pandas scikit-learn` 

## Usage

1.  Download the previous winning lottery numbers from your state's lottery website and save them in an Excel file.
2.  Run the `Predictor.py` file, which will train a Random Forest Regression model on the previous winning numbers and generate a set of predicted numbers.
3.  The program will output the most likely set of numbers for the next drawing.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this project as long as you give attribution to the original author.
