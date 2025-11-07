<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Smart Health Companion</title>
  <style>
    /* ---------- THEME VARIABLES (light defaults) ---------- */
    :root{
      --bg-grad-start:#667eea;
      --bg-grad-end:#764ba2;
      --container-bg:#ffffff;
      --text:#333333;
      --muted:#666666;
      --chip-bg:#f7f9fc;
      --rec-item-bg:#ffffff;
      --start-btn:#667eea;
      --stop-btn:#ef4444;
      --voice-bar:#667eea;
      --shadow:0 20px 60px rgba(0,0,0,0.3);
      --tiny-shadow:0 2px 5px rgba(0,0,0,0.05);
      --card-border: rgba(0,0,0,0.06);
      --ok:#10b981;
      --warn:#f59e0b;
      --bad:#ef4444;
    }
    html.dark{
      --bg-grad-start:#111827;
      --bg-grad-end:#1f2937;
      --container-bg:#1f2937;
      --text:#e5e7eb;
      --muted:#9ca3af;
      --chip-bg:#111827;
      --rec-item-bg:#1e293b;
      --start-btn:#3b82f6;
      --stop-btn:#ef4444;
      --voice-bar:#8ab4ff;
      --shadow:0 20px 60px rgba(0,0,0,0.6);
      --tiny-shadow:0 2px 5px rgba(255,255,255,0.06);
      --card-border: rgba(255,255,255,0.08);
    }

    *{margin:0;padding:0;box-sizing:border-box;}

    body{
      font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background:linear-gradient(135deg,var(--bg-grad-start) 0%,var(--bg-grad-end) 100%);
      min-height:100vh;
      display:flex;justify-content:center;align-items:center;
      padding:20px;
      color:var(--text);
      transition:background .4s ease, color .2s ease;
    }

    .container{
      background:var(--container-bg);
      border-radius:20px;
      box-shadow:var(--shadow);
      max-width:500px;width:100%;
      padding:30px;
      transition:background .3s ease, color .2s ease, box-shadow .3s ease;
      position:relative;
    }

    .header{text-align:center;margin-bottom:30px;}
    .header h1{color:#667eea;font-size:24px;margin-bottom:10px;}
    .header p{color:var(--muted);font-size:14px;}

    /* ---------- Registration Page ---------- */
    .registration-page{display:block;}
    .registration-page.hidden{display:none;}
    
    .form-group{margin-bottom:20px;}
    .form-group label{
      display:block;
      font-size:14px;
      font-weight:600;
      margin-bottom:8px;
      color:var(--text);
    }
    .form-group input{
      width:100%;
      padding:12px 16px;
      border:2px solid var(--card-border);
      border-radius:10px;
      font-size:14px;
      background:var(--chip-bg);
      color:var(--text);
      transition:all .3s ease;
    }
    .form-group input:focus{
      outline:none;
      border-color:#667eea;
      box-shadow:0 0 0 3px rgba(102,126,234,0.1);
    }
    html.dark .form-group input{
      background:var(--rec-item-bg);
      border-color:var(--card-border);
    }
    
    .error-message{
      color:var(--bad);
      font-size:12px;
      margin-top:5px;
      display:none;
    }
    .error-message.show{display:block;}
    
    .register-btn{
      width:100%;
      padding:16px;
      border:none;
      border-radius:12px;
      font-size:16px;
      font-weight:600;
      cursor:pointer;
      background:#667eea;
      color:#fff;
      transition:all .3s ease;
      margin-top:10px;
    }
    .register-btn:hover{
      filter:brightness(0.95);
      transform:translateY(-2px);
      box-shadow:0 5px 15px rgba(102,126,234,0.4);
    }
    .register-btn:disabled{
      background:#ccc;
      cursor:not-allowed;
      transform:none;
    }

    /* ---------- Main App Page ---------- */
    .main-app{display:none;}
    .main-app.active{display:block;}

    .user-info{
      background:var(--chip-bg);
      border-radius:10px;
      padding:12px 16px;
      margin-bottom:20px;
      font-size:13px;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }
    .user-info strong{color:#667eea;}
    .logout-btn{
      background:transparent;
      border:1px solid var(--card-border);
      padding:6px 12px;
      border-radius:6px;
      font-size:12px;
      cursor:pointer;
      color:var(--text);
      transition:all .2s ease;
    }
    .logout-btn:hover{
      background:var(--chip-bg);
      border-color:#667eea;
    }

    .ambient-data{
      background:var(--chip-bg);
      border-radius:12px;
      padding:15px;margin-bottom:20px;
      display:grid;grid-template-columns:repeat(2,1fr);gap:10px;
      transition:background .3s ease;
    }
    .ambient-item{display:flex;align-items:center;gap:8px;font-size:13px;color:#555;}
    html.dark .ambient-item{color:#cbd5e1;}

    .wellness-index{text-align:center;margin:30px 0;}
    .index-circle{
      width:180px;height:180px;margin:0 auto 15px;border-radius:50%;
      display:flex;flex-direction:column;justify-content:center;align-items:center;
      font-size:48px;font-weight:bold;color:#fff;
      box-shadow:0 10px 30px rgba(0,0,0,0.2);
      transition:all .5s ease;
    }
    .index-label{font-size:14px;font-weight:normal;margin-top:5px;color:#fff;}

    .status-text{font-size:18px;font-weight:600;margin-bottom:5px;}
    .status-desc{font-size:13px;color:var(--muted);}

    .control-btn{
      width:100%;padding:16px;border:none;border-radius:12px;
      font-size:16px;font-weight:600;cursor:pointer;transition:all .3s ease;
      margin-bottom:15px;
    }
    .start-btn{background:var(--start-btn);color:#fff;}
    .start-btn:hover{filter:brightness(0.95);transform:translateY(-2px);box-shadow:0 5px 15px rgba(102,126,234,0.4);}
    .stop-btn{background:var(--stop-btn);color:#fff;}
    .stop-btn:hover{filter:brightness(0.95);}
    .control-btn:disabled{background:#ccc;cursor:not-allowed;transform:none;}

    .recording-indicator{display:none;align-items:center;justify-content:center;gap:10px;color:#ef4444;font-size:14px;margin-bottom:15px;}
    .recording-indicator.active{display:flex;}
    .pulse{width:12px;height:12px;background:#ef4444;border-radius:50%;animation:pulse 1.5s infinite;}
    @keyframes pulse{0%,100%{opacity:1;transform:scale(1);}50%{opacity:.5;transform:scale(1.2);}}

    .recommendations{background:var(--chip-bg);border-radius:12px;padding:20px;margin-top:20px;transition:background .3s ease;}
    .rec-title{font-size:16px;font-weight:600;color:#333;margin-bottom:15px;display:flex;align-items:center;gap:8px;}
    html.dark .rec-title{color:#e5e7eb;}
    .rec-list{list-style:none;}
    .rec-item{
      padding:12px;background:var(--rec-item-bg);border-radius:8px;margin-bottom:8px;
      font-size:13px;color:#555;display:flex;align-items:center;gap:10px;
      box-shadow:var(--tiny-shadow);
      transition:background .3s ease,color .2s ease;
    }
    html.dark .rec-item{color:#d1d5db;}
    .rec-icon{font-size:20px;flex-shrink:0;}

    .voice-viz{display:none;height:60px;background:var(--chip-bg);border-radius:8px;margin:15px 0;position:relative;overflow:hidden;transition:background .3s ease;}
    .voice-viz.active{display:block;}
    .voice-bar{position:absolute;bottom:0;width:3px;background:var(--voice-bar);border-radius:3px 3px 0 0;transition:height .1s ease;}

    #cam-video,#cam-canvas{position:absolute;width:1px;height:1px;opacity:0;pointer-events:none;}

    .dark-toggle{
      position:fixed;top:16px;right:16px;z-index:9999;
      background:#e5e7eb;color:#111827;border:none;border-radius:999px;
      padding:8px 14px;font-size:13px;font-weight:700;cursor:pointer;
      box-shadow:0 4px 12px rgba(0,0,0,0.15);
      transition:background .25s ease,color .25s ease, transform .1s ease;
    }
    .dark-toggle:active{transform:scale(0.98);}
    html.dark .dark-toggle{background:#374151;color:#f9fafb;}

    .psy{
      display:none;
      margin-top:16px;
      background:var(--chip-bg);
      border-radius:12px;
      padding:18px;
      border:1px solid var(--card-border);
    }
    .psy-title{
      font-size:16px;
      font-weight:700;
      margin-bottom:10px;
      display:flex;align-items:center;gap:8px;
    }
    .psy-controls{
      display:flex;gap:10px;align-items:center;flex-wrap:wrap;
      margin:6px 0 14px;
      font-size:13px;color:var(--muted);
    }
    .doc-list{
      list-style:none;display:flex;flex-direction:column;gap:8px;margin:0;padding:0;
    }
    .doc{
      background:var(--rec-item-bg);
      border:1px solid var(--card-border);
      border-radius:10px;
      padding:12px;
      display:flex;gap:10px;align-items:flex-start;
    }
    .doc strong{color:var(--text);}
    .badge{
      font-size:11px;padding:3px 8px;border-radius:999px;background:#dbeafe;color:#1e40af;
      margin-left:auto;align-self:flex-start;
    }
    html.dark .badge{background:#111827;color:#93c5fd;border:1px solid #1f2937;}

    .psy-hide{
      margin-left:auto;font-size:12px;cursor:pointer;opacity:0.8;text-decoration:underline;
    }

    .vsa{
      display:none;
      margin-top:12px;
      background:var(--chip-bg);
      border:1px solid var(--card-border);
      border-radius:10px;
      padding:12px;
    }
    .vsa-title{
      font-weight:700;font-size:14px;margin-bottom:6px;display:flex;gap:8px;align-items:center;
    }
    .vsa-grid{
      display:grid;grid-template-columns:repeat(2,1fr);gap:8px;font-size:12px;color:var(--muted);
    }
    .vsa-pill{
      margin-left:auto;font-size:11px;padding:2px 8px;border-radius:999px;background:#e5e7eb;color:#111827;
    }
    html.dark .vsa-pill{background:#374151;color:#f9fafb;}
    .vsa-score{font-weight:700;}
  </style>
</head>
<body>
  <button class="dark-toggle" id="theme-toggle">🌙 Dark Mode</button>

  <div class="container">
    <!-- Registration Page -->
    <div class="registration-page" id="registration-page">
      <div class="header">
        <h1>🏥 Smart Health Companion</h1>
        <p>Welcome! Please register to continue</p>
      </div>

      <div class="form-group">
        <label for="reg-name">Full Name *</label>
        <input type="text" id="reg-name" placeholder="Enter your full name" required>
        <div class="error-message" id="name-error">Please enter your name</div>
      </div>

      <div class="form-group">
        <label for="reg-email">Email Address *</label>
        <input type="email" id="reg-email" placeholder="your.email@example.com" required>
        <div class="error-message" id="email-error">Please enter a valid email</div>
      </div>

      <div class="form-group">
        <label for="reg-contact">Contact Number *</label>
        <input type="tel" id="reg-contact" placeholder="+91 XXXXX XXXXX" required>
        <div class="error-message" id="contact-error">Please enter a valid contact number</div>
      </div>

      <button class="register-btn" id="register-btn">Register & Continue</button>
    </div>

    <!-- Main App Page -->
    <div class="main-app" id="main-app">
      <div class="header">
        <h1>🏥 Smart Health Companion</h1>
        <p>AI-Driven Stress & Fatigue Detection</p>
      </div>

      <div class="user-info" id="user-info">
        <div>Welcome, <strong id="user-name-display">User</strong></div>
        <button class="logout-btn" id="logout-btn">Logout</button>
      </div>

      <div class="ambient-data">
        <div class="ambient-item"><span class="ambient-icon">💡</span><span>Light: <strong id="light-level">Normal</strong></span></div>
        <div class="ambient-item"><span class="ambient-icon">🔊</span><span>Noise: <strong id="noise-level">Low</strong></span></div>
        <div class="ambient-item"><span class="ambient-icon">🕐</span><span>Time: <strong id="time-day">--:--</strong></span></div>
        <div class="ambient-item"><span class="ambient-icon">📅</span><span>Day: <strong id="day-week">---</strong></span></div>
      </div>

      <div class="wellness-index">
        <div class="index-circle" id="wellness-circle">
          <div>
            <span id="wellness-score">--</span>
            <div class="index-label">Wellness Index</div>
          </div>
        </div>
        <div class="status-text" id="status-text">Ready to Analyze</div>
        <div class="status-desc" id="status-desc">Click start to begin voice & light analysis</div>
      </div>

      <div class="recording-indicator" id="recording-indicator">
        <div class="pulse"></div>
        <span>Recording & Analyzing...</span>
      </div>

      <div class="vsa" id="vsa-panel">
        <div class="vsa-title">
          🗣️ Voice Stress Analysis
          <span class="vsa-pill" id="vsa-state">Calibrating…</span>
        </div>
        <div class="vsa-grid">
          <div>Pitch: <span id="vsa-pitch">--</span> Hz</div>
          <div>HF Ratio: <span id="vsa-hfr">--</span></div>
          <div>ZCR: <span id="vsa-zcr">--</span></div>
          <div>Centroid: <span id="vsa-centroid">--</span> Hz</div>
          <div>VSA Stress: <span class="vsa-score" id="vsa-stress">--</span>/100</div>
        </div>
      </div>

      <div class="voice-viz" id="voice-viz"></div>

      <button class="control-btn start-btn" id="start-btn">🎤 Start Voice Analysis</button>
      <button class="control-btn stop-btn" id="stop-btn" style="display:none;">⏹️ Stop Analysis</button>

      <div class="recommendations" id="recommendations" style="display:none;">
        <div class="rec-title"><span>💡</span><span>Personalized Recommendations</span></div>
        <ul class="rec-list" id="rec-list"></ul>
      </div>

      <div class="psy" id="psy-section">
        <div class="psy-title">
          🧠 Our Recommended Psychiatrists
          <span class="psy-hide" id="psy-hide">Hide</span>
        </div>
        <div class="psy-controls">
          <span>Choose location:</span>
          <label><input type="radio" name="loc" value="A" checked> Location A</label>
          <label><input type="radio" name="loc" value="B"> Location B</label>
        </div>
        <ul class="doc-list" id="doc-list"></ul>
      </div>
    </div>
  </div>

  <video id="cam-video" playsinline muted></video>
  <canvas id="cam-canvas"></canvas>

  <script>
    /* ---------- User Registration State ---------- */
    let currentUser = null;

    /* ---------- Theme toggle ---------- */
    const themeToggle = document.getElementById('theme-toggle');
    function applyTheme(mode){
      const root = document.documentElement;
      if(mode === 'dark'){
        root.classList.add('dark');
        themeToggle.textContent = '☀️ Light Mode';
        localStorage.setItem('theme','dark');
      }else{
        root.classList.remove('dark');
        themeToggle.textContent = '🌙 Dark Mode';
        localStorage.setItem('theme','light');
      }
    }
    applyTheme(localStorage.getItem('theme') === 'dark' ? 'dark' : 'light');
    themeToggle.addEventListener('click',()=>{
      const isDark = document.documentElement.classList.contains('dark');
      applyTheme(isDark ? 'light' : 'dark');
    });

    /* ---------- Registration Logic ---------- */
    const registrationPage = document.getElementById('registration-page');
    const mainApp = document.getElementById('main-app');
    const registerBtn = document.getElementById('register-btn');
    const regName = document.getElementById('reg-name');
    const regEmail = document.getElementById('reg-email');
    const regContact = document.getElementById('reg-contact');
    const userNameDisplay = document.getElementById('user-name-display');
    const logoutBtn = document.getElementById('logout-btn');

    // Check if user is already registered
    function checkRegistration(){
      const savedUser = localStorage.getItem('healthCompanionUser');
      if(savedUser){
        currentUser = JSON.parse(savedUser);
        showMainApp();
      }
    }

    function validateEmail(email){
      return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
    }

    function validateContact(contact){
      return /^[+]?[\d\s-]{10,}$/.test(contact);
    }

    registerBtn.addEventListener('click', ()=>{
      const name = regName.value.trim();
      const email = regEmail.value.trim();
      const contact = regContact.value.trim();

      let isValid = true;

      // Validate name
      if(!name){
        document.getElementById('name-error').classList.add('show');
        isValid = false;
      }else{
        document.getElementById('name-error').classList.remove('show');
      }

      // Validate email
      if(!validateEmail(email)){
        document.getElementById('email-error').classList.add('show');
        isValid = false;
      }else{
        document.getElementById('email-error').classList.remove('show');
      }

      // Validate contact
      if(!validateContact(contact)){
        document.getElementById('contact-error').classList.add('show');
        isValid = false;
      }else{
        document.getElementById('contact-error').classList.remove('show');
      }

      if(isValid){
        currentUser = {name, email, contact, registeredAt: new Date().toISOString()};
        localStorage.setItem('healthCompanionUser', JSON.stringify(currentUser));
        showMainApp();
      }
    });

    function showMainApp(){
      registrationPage.classList.add('hidden');
      mainApp.classList.add('active');
      userNameDisplay.textContent = currentUser.name;
    }

    logoutBtn.addEventListener('click', ()=>{
      if(confirm('Are you sure you want to logout?')){
        localStorage.removeItem('healthCompanionUser');
        currentUser = null;
        mainApp.classList.remove('active');
        registrationPage.classList.remove('hidden');
        regName.value = '';
        regEmail.value = '';
        regContact.value = '';
      }
    });

    // Initialize
    checkRegistration();

    /* ---------- Voice Analysis State ---------- */
    let audioContext, analyser, microphone, dataArray;
    let isRecording = false;
    let analysisInterval;
    let sessionMinIndex = Infinity;

    let vsaEnabled = true;
    let vsaCalibrating = false;
    let vsaCalibStart = 0;
    let vsaBaseline = { pitch: [], zcr: [], centroid: [], hfr: [] };
    let vsaHasBaseline = false;
    const VSA_CALIB_MS = 3000;

    let camStream = null;
    let brightnessInterval = null;
    let cameraActive = false;
    const videoEl = document.getElementById('cam-video');
    const canvasEl = document.getElementById('cam-canvas');
    const ctx = canvasEl.getContext('2d');

    let stressAccumulator = [];

    const startBtn = document.getElementById('start-btn');
    const stopBtn = document.getElementById('stop-btn');
    const recordingIndicator = document.getElementById('recording-indicator');
    const wellnessCircle = document.getElementById('wellness-circle');
    const wellnessScore = document.getElementById('wellness-score');
    const statusText = document.getElementById('status-text');
    const statusDesc = document.getElementById('status-desc');
    const recommendations = document.getElementById('recommendations');
    const recList = document.getElementById('rec-list');
    const voiceViz = document.getElementById('voice-viz');

    const vsaPanel = document.getElementById('vsa-panel');
    const vsaState = document.getElementById('vsa-state');
    const vsaPitchEl = document.getElementById('vsa-pitch');
    const vsaZCREl = document.getElementById('vsa-zcr');
    const vsaCentroidEl = document.getElementById('vsa-centroid');
    const vsaHFREl = document.getElementById('vsa-hfr');
    const vsaStressEl = document.getElementById('vsa-stress');

    const psySection = document.getElementById('psy-section');
    const docList = document.getElementById('doc-list');
    const psyHide = document.getElementById('psy-hide');

    psySection.style.display = 'none';
    vsaPanel.style.display = 'none';

    for (let i=0;i<30;i++){
      const bar = document.createElement('div');
      bar.className='voice-bar';
      bar.style.left = `${i*4+10}px`;
      voiceViz.appendChild(bar);
    }

    function updateAmbientData(){
      const now = new Date();
      const hours = now.getHours();
      const timeString = now.toLocaleTimeString('en-US',{hour:'2-digit',minute:'2-digit'});
      const dayString = now.toLocaleDateString('en-US',{weekday:'short'});
      document.getElementById('time-day').textContent = timeString;
      document.getElementById('day-week').textContent = dayString;

      if (!cameraActive){
        let lightLevel='Normal';
        if (hours < 6 || hours > 20) lightLevel='Dark';
        else if (hours >= 12 && hours <= 14) lightLevel='Bright';
        document.getElementById('light-level').textContent = lightLevel;
      }
    }
    updateAmbientData();
    setInterval(updateAmbientData,60000);

    startBtn.addEventListener('click', async ()=>{
      try{
        sessionMinIndex = Infinity;
        psySection.style.display = 'none';

        const audioStream = await navigator.mediaDevices.getUserMedia({audio:true});
        audioContext = new (window.AudioContext || window.webkitAudioContext)();
        analyser = audioContext.createAnalyser();
        analyser.fftSize = 1024;
        microphone = audioContext.createMediaStreamSource(audioStream);
        dataArray = new Uint8Array(analyser.frequencyBinCount);
        microphone.connect(analyser);

        await startBrightnessDetection();

        if (vsaEnabled){
          vsaCalibrating = true;
          vsaHasBaseline = false;
          vsaBaseline = { pitch:[], zcr:[], centroid:[], hfr:[] };
          vsaCalibStart = performance.now();
          vsaPanel.style.display = 'block';
          vsaState.textContent = 'Calibrating…';
        }

        isRecording = true;
        startBtn.style.display='none';
        stopBtn.style.display='block';
        recordingIndicator.classList.add('active');
        voiceViz.classList.add('active');

        analyzeVoice();
      }catch(err){
        alert('Microphone access denied. Please allow microphone access to use this feature.');
        console.error('Permission error:', err);
      }
    });

    stopBtn.addEventListener('click', ()=>{ stopAnalysis(); });

    function stopAnalysis(){
      isRecording = false;
      if (analysisInterval) clearInterval(analysisInterval);

      try{
        if (microphone){
          microphone.disconnect();
          if (microphone.mediaStream){
            microphone.mediaStream.getTracks().forEach(t=>t.stop());
          }
        }
      }catch(e){}

      if (audioContext){
        audioContext.close();
        audioContext = null;
      }

      stopBrightnessDetection();

      startBtn.style.display='block';
      stopBtn.style.display='none';
      recordingIndicator.classList.remove('active');
      voiceViz.classList.remove('active');

      if (sessionMinIndex < 35){
        const currentLoc = (document.querySelector('input[name="loc"]:checked') || {}).value || 'A';
        renderPsychiatrists(currentLoc);
        psySection.style.display = 'block';
      } else {
        psySection.style.display = 'none';
      }

      vsaPanel.style.display = 'none';
    }

    function analyzeVoice(){
      const timeBuf = new Float32Array(2048);
      analysisInterval = setInterval(()=>{
        if (!isRecording) return;

        analyser.getByteFrequencyData(dataArray);
        let tdSize = Math.min(analyser.fftSize, timeBuf.length);
        const td = new Float32Array(tdSize);
        analyser.getFloatTimeDomainData(td);

        const bars = voiceViz.querySelectorAll('.voice-bar');
        bars.forEach((bar,i)=>{
          const idx = i*2;
          const value = dataArray[idx] || 0;
          bar.style.height = `${(value/255)*100}%`;
        });

        const volume = dataArray.reduce((a,b)=>a+b,0)/dataArray.length;
        if (volume > 80) document.getElementById('noise-level').textContent='High';
        else if (volume > 40) document.getElementById('noise-level').textContent='Moderate';
        else document.getElementById('noise-level').textContent='Low';

        const half = dataArray.length/2;
        const highFreq = dataArray.slice(half).reduce((a, b) => a + b, 0) / half;
        const lowFreq = dataArray.slice(0, half).reduce((a, b) => a + b, 0) / half;

        const baseIndicators = {
          volumeVariation: Math.abs(volume - 50) / 50,
          frequencyRatio: highFreq / (lowFreq + 1),
          energyLevel: volume / 100
        };
        let baseStress = (
          baseIndicators.volumeVariation * 0.3 +
          baseIndicators.frequencyRatio * 0.4 +
          baseIndicators.energyLevel * 0.3
        ) * 100;

        let vsaStress = null;
        if (vsaEnabled){
          const sr = audioContext.sampleRate || 44100;
          const pitch = estimatePitch(td, sr);
          const zcr = zeroCrossingRate(td);
          const { centroid, hfr } = spectralFeatures(dataArray, sr);

          if (vsaPanel.style.display !== 'block') vsaPanel.style.display = 'block';
          vsaPitchEl.textContent = pitch ? Math.round(pitch) : '--';
          vsaZCREl.textContent = zcr.toFixed(3);
          vsaCentroidEl.textContent = Math.round(centroid);
          vsaHFREl.textContent = hfr.toFixed(2);

          const now = performance.now();
          if (vsaCalibrating){
            pushSafe(vsaBaseline.pitch, pitch || 0);
            pushSafe(vsaBaseline.zcr, zcr);
            pushSafe(vsaBaseline.centroid, centroid);
            pushSafe(vsaBaseline.hfr, hfr);

            vsaState.textContent = 'Calibrating…';
            if (now - vsaCalibStart >= VSA_CALIB_MS){
              vsaCalibrating = false;
              vsaHasBaseline = true;
              vsaState.textContent = 'Live';
              trimTo(vsaBaseline.pitch, 60);
              trimTo(vsaBaseline.zcr, 60);
              trimTo(vsaBaseline.centroid, 60);
              trimTo(vsaBaseline.hfr, 60);
            }
          } else if (vsaHasBaseline) {
            const devPitch = relZ(pitch || 0, mean(vsaBaseline.pitch), std(vsaBaseline.pitch));
            const devZCR = relZ(zcr, mean(vsaBaseline.zcr), std(vsaBaseline.zcr));
            const devCent = relZ(centroid, mean(vsaBaseline.centroid), std(vsaBaseline.centroid));
            const devHFR = relZ(hfr, mean(vsaBaseline.hfr), std(vsaBaseline.hfr));

            const devs = clamp01(
              ( Math.abs(devPitch)*0.35 + Math.abs(devCent)*0.25 + Math.abs(devHFR)*0.25 + Math.abs(devZCR)*0.15 ) / 4
            );
            vsaStress = devs * 100;
            vsaStressEl.textContent = Math.round(vsaStress);

            if (vsaStress < 30) vsaState.textContent = 'Live • Calm';
            else if (vsaStress < 60) vsaState.textContent = 'Live • Elevated';
            else vsaState.textContent = 'Live • High';

            baseStress = clamp01( (0.7 * (baseStress/100)) + (0.3 * (vsaStress/100)) ) * 100;
          } else {
            vsaState.textContent = 'Calibrating…';
          }
        }

        stressAccumulator.push(baseStress);
        if (stressAccumulator.length>20) stressAccumulator.shift();

        const avgStress = stressAccumulator.reduce((a,b)=>a+b,0)/stressAccumulator.length;
        const wellnessIndex = Math.max(0, Math.min(100, 100-avgStress));
        sessionMinIndex = Math.min(sessionMinIndex, Math.round(wellnessIndex));

        updateWellnessIndex(Math.round(wellnessIndex));
      }, 200);
    }

    function updateWellnessIndex(score){
      wellnessScore.textContent = score;

      let color, status, desc, recs;

      if (score >= 75){
        color= getComputedStyle(document.documentElement).getPropertyValue('--ok').trim(); 
        status='Excellent'; desc="You're doing great! Keep it up.";
        recs=[{icon:'✨',text:'Maintain your current routine'},
              {icon:'🎯',text:'Continue regular breaks'},
              {icon:'😊',text:'Keep up the positive mindset'}];
      }else if (score >= 50){
        color= getComputedStyle(document.documentElement).getPropertyValue('--warn').trim();
        status='Moderate Stress'; desc='Some signs of stress detected.';
        recs=[{icon:'💧',text:'Drink a glass of water'},
              {icon:'🧘',text:'Try 5-minute breathing exercise'},
              {icon:'🚶',text:'Take a short walk'},
              {icon:'🎵',text:'Listen to calming music'}];
      }else if (score >= 25){
        color= getComputedStyle(document.documentElement).getPropertyValue('--bad').trim();
        status='High Stress'; desc='Significant stress indicators detected.';
        recs=[{icon:'⚠️',text:'Take an immediate break'},
              {icon:'🧘‍♀️',text:'Practice deep breathing (4-7-8 technique)'},
              {icon:'💧',text:'Hydrate - drink 2 glasses of water'},
              {icon:'🌳',text:'Step outside for fresh air'},
              {icon:'📞',text:'Consider talking to someone'}];
      }else{
        color='#dc2626'; status='Critical - Rest Needed'; desc='Severe stress/fatigue detected.';
        recs=[{icon:'🛑',text:'STOP current activity immediately'},
              {icon:'😴',text:'Consider taking a 20-minute rest'},
              {icon:'💧',text:'Hydrate well'},
              {icon:'🌙',text:'Ensure proper sleep tonight'},
              {icon:'🏥',text:'Consult healthcare professional if persistent'}];
      }

      wellnessCircle.style.background = `linear-gradient(135deg, ${color}, ${color}dd)`;
      statusText.textContent = status;
      statusText.style.color = color;
      statusDesc.textContent = desc;

      recommendations.style.display='block';
      recList.innerHTML='';
      recs.forEach(rec=>{
        const li=document.createElement('li');
        li.className='rec-item';
        li.innerHTML = `<span class="rec-icon">${rec.icon}</span><span>${rec.text}</span>`;
        recList.appendChild(li);
      });
    }

    function renderPsychiatrists(location){
      docList.innerHTML = '';

      let doctors;
      if (location === 'A'){
        doctors = [
          { name:'Dr. John', tag:'Suggested near you', exp:'12+ yrs • Adult Psychiatry', address:'Location A • City Center' },
          { name:'Dr. Priya Sharma', tag:'Recommended', exp:'9+ yrs • Stress & Anxiety', address:'Location A • Green Park' },
          { name:'Dr. Arjun Mehta', tag:'Recommended', exp:'7+ yrs • Sleep & Mood', address:'Location A • Lake View' },
        ];
      }else{
        doctors = [
          { name:'Dr. Jane', tag:'Suggested near you', exp:'11+ yrs • Adolescent & Adult', address:'Location B • Riverside' },
          { name:'Dr. Rahul Verma', tag:'Recommended', exp:'10+ yrs • Workplace Stress', address:'Location B • Tech Park' },
          { name:'Dr. Meera Iyer', tag:'Recommended', exp:'8+ yrs • CBT & Mindfulness', address:'Location B • Old Town' },
        ];
      }

      doctors.forEach(d=>{
        const li = document.createElement('li');
        li.className = 'doc';
        li.innerHTML = `
          <div>🩺 <strong>${d.name}</strong><br/>
            <span style="font-size:12px;color:var(--muted);">${d.exp}</span><br/>
            <span style="font-size:12px;color:var(--muted);">📍 ${d.address}</span>
          </div>
          <span class="badge">${d.tag}</span>
        `;
        docList.appendChild(li);
      });
    }

    document.addEventListener('change', (e)=>{
      if (e.target && e.target.name === 'loc' && psySection.style.display === 'block'){
        renderPsychiatrists(e.target.value);
      }
    });

    psyHide.addEventListener('click', ()=>{
      psySection.style.display = 'none';
    });

    async function startBrightnessDetection(){
      try{
        camStream = await navigator.mediaDevices.getUserMedia({
          video:{width:{ideal:320},height:{ideal:240},facingMode:{ideal:'environment'}}
        });

        videoEl.srcObject = camStream;
        await videoEl.play();

        const w = videoEl.videoWidth || 320;
        const h = videoEl.videoHeight || 240;
        canvasEl.width = w; canvasEl.height = h;

        cameraActive = true;

        brightnessInterval = setInterval(()=>{
          if (!cameraActive) return;
          try{
            ctx.drawImage(videoEl,0,0,w,h);
            const frame = ctx.getImageData(0,0,w,h).data;

            let sum=0;
            for (let i=0;i<frame.length;i+=4){
              const r=frame[i], g=frame[i+1], b=frame[i+2];
              const Y = 0.2126*r + 0.7152*g + 0.0722*b;
              sum += Y;
            }
            const pixels = frame.length/4;
            const avgLuma = sum/pixels;

            updateLightLevel(avgLuma);
          }catch(e){
            console.warn('Brightness sampling error:', e);
            stopBrightnessDetection();
          }
        },200);
      }catch(e){
        console.warn('Camera not available for brightness detection:', e);
        cameraActive = false;
      }
    }

    function stopBrightnessDetection(){
      cameraActive = false;
      if (brightnessInterval){ clearInterval(brightnessInterval); brightnessInterval = null; }
      if (camStream){ camStream.getTracks().forEach(t=>t.stop()); camStream = null; }
    }

    function updateLightLevel(avgLuma){
      let label='Normal';
      if (avgLuma < 40) label='Dark';
      else if (avgLuma < 90) label='Dim';
      else if (avgLuma < 160) label='Normal';
      else if (avgLuma < 210) label='Bright';
      else label='Very Bright';

      document.getElementById('light-level').textContent = `${label}`;
    }

    function pushSafe(arr, v){ if (Number.isFinite(v)) arr.push(v); }
    function trimTo(arr, n){ while (arr.length>n) arr.shift(); }
    function mean(a){ if(!a.length) return 0; return a.reduce((x,y)=>x+y,0)/a.length; }
    function std(a){ if(a.length<2) return 1; const m=mean(a); const v=a.reduce((s,x)=>s+(x-m)*(x-m),0)/(a.length-1); return Math.sqrt(v)||1; }
    function clamp01(x){ return Math.min(1, Math.max(0, x)); }
    function relZ(x, m, s){ return (x - m) / (s || 1); }

    function zeroCrossingRate(buf){
      let zc = 0;
      for (let i=1;i<buf.length;i++){
        if ((buf[i-1] >= 0 && buf[i] < 0) || (buf[i-1] < 0 && buf[i] >= 0)) zc++;
      }
      return zc / buf.length;
    }

    function spectralFeatures(freqBytes, sampleRate){
      const N = freqBytes.length;
      const binHz = (sampleRate/2) / N;
      let num=0, den=0, high=0;

      for (let i=0;i<N;i++){
        const mag = freqBytes[i];
        const f = i * binHz;
        num += f * mag;
        den += mag;
        if (i > N/2) high += mag;
      }
      const centroid = den>0 ? (num/den) : 0;
      const total = den || 1;
      const hfr = high / total;
      return { centroid, hfr };
    }

    function estimatePitch(timeBuf, sampleRate){
      let rms = 0;
      for (let i=0;i<timeBuf.length;i++) rms += timeBuf[i]*timeBuf[i];
      rms = Math.sqrt(rms/timeBuf.length);
      if (rms < 0.01) return null;

      const size = timeBuf.length;
      const corr = new Float32Array(size);
      for (let lag=0; lag<size; lag++){
        let sum=0;
        for (let i=0; i<size-lag; i++){
          sum += timeBuf[i] * timeBuf[i+lag];
        }
        corr[lag] = sum;
      }
      let d=0; while (d < size-1 && corr[d] >= corr[d+1]) d++;
      let peakIndex=d, peak=corr[d];
      for (let i=d+1;i<size;i++){
        if (corr[i] > peak){
          peak = corr[i];
          peakIndex = i;
        }
      }
      if (peakIndex === 0) return null;
      const freq = sampleRate / peakIndex;
      if (freq < 60 || freq > 400) return null;
      return freq;
    }
  </script>
</body>
</html>
