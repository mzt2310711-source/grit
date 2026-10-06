<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
  <title>GRIT TRACKER</title>
  
  <!-- PWA & iOS Safari 設定 -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="GRIT">
  <meta name="theme-color" content="#090d16">
  
  <!-- アプリアイコン（SVGをData URIとして直接埋め込み） -->
  <link rel="apple-touch-icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Crect width='512' height='512' rx='128' fill='%23090d16'/%3E%3Cpath d='M256 96L304 224H416L320 296L356 416L256 344L156 416L192 296L96 224H208L256 96Z' fill='%236366f1'/%3E%3C/svg%3E">
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Crect width='512' height='512' rx='128' fill='%23090d16'/%3E%3Cpath d='M256 96L304 224H416L320 296L356 416L256 344L156 416L192 296L96 224H208L256 96Z' fill='%236366f1'/%3E%3C/svg%3E">

  <style>
    :root {
      --bg: #090d16;
      --card-bg: rgba(22, 27, 46, 0.7);
      --card-border: rgba(255, 255, 255, 0.08);
      --accent: #6366f1;
      --accent-glow: rgba(99, 102, 241, 0.35);
      --success: #10b981;
      --text: #f3f4f6;
      --text-sub: #9ca3af;
      --safe-top: env(safe-area-inset-top, 20px);
      --safe-bottom: env(safe-area-inset-bottom, 20px);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
    }

    body {
      background-color: var(--bg);
      color: var(--text);
      font-family: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", Roboto, sans-serif;
      min-height: 100vh;
      padding: calc(var(--safe-top) + 16px) 16px calc(var(--safe-bottom) + 30px);
      display: flex;
      justify-content: center;
      background-image: radial-gradient(circle at 50% 0%, #1e1e38 0%, #090d16 70%);
      background-attachment: fixed;
    }

    .app-container {
      width: 100%;
      max-width: 440px;
      display: flex;
      flex-direction: column;
      gap: 18px;
    }

    /* ヘッダー */
    header {
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      padding: 0 4px 6px;
    }

    .app-title {
      font-size: 24px;
      font-weight: 800;
      letter-spacing: 1.5px;
      background: linear-gradient(135deg, #fff 40%, var(--accent) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .current-date {
      font-size: 13px;
      font-weight: 600;
      color: var(--text-sub);
      letter-spacing: 0.5px;
    }

    /* グリッドカード */
    .card {
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: 20px;
      padding: 18px;
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.4);
    }

    .card-label {
      font-size: 11px;
      font-weight: 700;
      color: var(--text-sub);
      text-transform: uppercase;
      letter-spacing: 1.2px;
      margin-bottom: 12px;
      display: flex;
      justify-content: space-between;
    }

    /* 今日の達成プログレス */
    .progress-bar-container {
      height: 8px;
      background: rgba(255, 255, 255, 0.08);
      border-radius: 99px;
      overflow: hidden;
      margin-top: 6px;
    }

    .progress-fill {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg, var(--accent), #a855f7);
      border-radius: 99px;
      transition: width 0.4s cubic-bezier(0.16, 1, 0.3, 1);
    }

    /* タスクリスト */
    .task-list {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .task-item {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 14px 16px;
      background: rgba(255, 255, 255, 0.03);
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: 14px;
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .task-item:active {
      transform: scale(0.98);
      background: rgba(255, 255, 255, 0.08);
    }

    .task-item.checked {
      background: rgba(99, 102, 241, 0.12);
      border-color: rgba(99, 102, 241, 0.4);
    }

    .task-info {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .task-icon {
      font-size: 20px;
    }

    .task-name {
      font-size: 15px;
      font-weight: 600;
      color: var(--text);
    }

    .checkbox {
      width: 24px;
      height: 24px;
      border-radius: 7px;
      border: 2px solid rgba(255, 255, 255, 0.25);
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.2s ease;
    }

    .task-item.checked .checkbox {
      background: var(--accent);
      border-color: var(--accent);
      box-shadow: 0 0 10px var(--accent-glow);
    }

    .checkbox svg {
      display: none;
      width: 14px;
      height: 14px;
      fill: none;
      stroke: #fff;
      stroke-width: 3;
      stroke-linecap: round;
      stroke-linejoin: round;
    }

    .task-item.checked .checkbox svg {
      display: block;
    }

    /* 統計グリッド */
    .stats-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }

    .stat-card {
      background: rgba(255, 255, 255, 0.03);
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: 14px;
      padding: 12px 14px;
      display: flex;
      flex-direction: column;
      gap: 4px;
    }

    .stat-title {
      font-size: 11px;
      font-weight: 600;
      color: var(--text-sub);
    }

    .stat-value {
      font-size: 18px;
      font-weight: 800;
      color: #fff;
      display: flex;
      align-items: baseline;
      gap: 3px;
    }

    .stat-sub {
      font-size: 11px;
      font-weight: normal;
      color: var(--text-sub);
    }

    /* 過去7日のヒートマップ */
    .history-dots {
      display: flex;
      justify-content: space-between;
      margin-top: 10px;
      padding-top: 12px;
      border-top: 1px solid rgba(255, 255, 255, 0.06);
    }

    .dot-day {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 6px;
    }

    .dot-label {
      font-size: 10px;
      color: var(--text-sub);
      font-weight: 600;
    }

    .dot {
      width: 22px;
      height: 22px;
      border-radius: 6px;
      background: rgba(255, 255, 255, 0.06);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 10px;
      font-weight: 700;
      color: rgba(255, 255, 255, 0.4);
    }

    .dot.full {
      background: var(--success);
      color: #fff;
      box-shadow: 0 0 8px rgba(16, 185, 129, 0.4);
    }

    .dot.partial {
      background: var(--accent);
      color: #fff;
    }
  </style>
</head>
<body>

  <div class="app-container">
    <header>
      <div>
        <div class="app-title">GRIT TRACKER</div>
        <div class="current-date" id="dateDisplay">---</div>
      </div>
    </header>

    <!-- 今日のタスク一覧 -->
    <div class="card">
      <div class="card-label">
        <span>TODAY'S PROTOCOL</span>
        <span id="rateDisplay">0%</span>
      </div>
      <div class="task-list" id="taskList"></div>
      <div class="progress-bar-container">
        <div class="progress-fill" id="progressFill"></div>
      </div>
    </div>

    <!-- 統計・ストリーク -->
    <div class="card">
      <div class="card-label">PERFORMANCE & STREAKS</div>
      <div class="stats-grid">
        <div class="stat-card">
          <div class="stat-title">🏋️ 今週のジム (目標3回)</div>
          <div class="stat-value" id="gymProgress">0 <span class="stat-sub">/ 3回</span></div>
        </div>
        <div class="stat-card">
          <div class="stat-title">🪥 歯磨きストリーク</div>
          <div class="stat-value" id="brushStreak">0 <span class="stat-sub">日連続</span></div>
        </div>
        <div class="stat-card">
          <div class="stat-title">🥤 プロテイン (2回) 連続</div>
          <div class="stat-value" id="proteinStreak">0 <span class="stat-sub">日連続</span></div>
        </div>
        <div class="stat-card">
          <div class="stat-title">🍱 3食完食ストリーク</div>
          <div class="stat-value" id="mealStreak">0 <span class="stat-sub">日連続</span></div>
        </div>
      </div>

      <!-- 直近7日間の達成状況 -->
      <div class="history-dots" id="weekHistory"></div>
    </div>
  </div>

  <script>
    // タスク定義
    const TASKS = [
      { id: 'brush', name: '歯磨きを毎日する', icon: '🪥', weight: 'daily' },
      { id: 'protein1', name: 'プロテイン 1回目', icon: '🥛', weight: 'daily' },
      { id: 'protein2', name: 'プロテイン 2回目', icon: '🥤', weight: 'daily' },
      { id: 'meal', name: '3食しっかり食べる', icon: '🍱', weight: 'daily' },
      { id: 'gym', name: 'ジムでトレーニング (週3回)', icon: '🏋️', weight: 'gym' }
    ];

    // 日付キー生成（YYYY-MM-DD）
    function getDateKey(date = new Date()) {
      const y = date.getFullYear();
      const m = String(date.getMonth() + 1).padStart(2, '0');
      const d = String(date.getDate()).padStart(2, '0');
      return `${y}-${m}-${d}`;
    }

    // データ読み込み & 保存
    function loadLogs() {
      try {
        return JSON.parse(localStorage.getItem('grit_tracker_data') || '{}');
      } catch {
        return {};
      }
    }

    function saveLogs(logs) {
      localStorage.setItem('grit_tracker_data', JSON.stringify(logs));
    }

    const todayKey = getDateKey();
    let logs = loadLogs();
    if (!logs[todayKey]) logs[todayKey] = {};

    // 画面初期化
    function init() {
      // 日付表示
      const now = new Date();
      const days = ['SUN', 'MON', 'TUE', 'WED', 'THU', 'FRI', 'SAT'];
      document.getElementById('dateDisplay').textContent = 
        `${now.getFullYear()}.${String(now.getMonth()+1).padStart(2,'0')}.${String(now.getDate()).padStart(2,'0')} ${days[now.getDay()]}`;

      // タスクリスト生成
      const listEl = document.getElementById('taskList');
      listEl.innerHTML = '';
      TASKS.forEach(task => {
        const isChecked = !!logs[todayKey][task.id];
        const item = document.createElement('div');
        item.className = `task-item ${isChecked ? 'checked' : ''}`;
        item.innerHTML = `
          <div class="task-info">
            <span class="task-icon">${task.icon}</span>
            <span class="task-name">${task.name}</span>
          </div>
          <div class="checkbox">
            <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"></polyline></svg>
          </div>
        `;
        item.onclick = () => toggleTask(task.id);
        listEl.appendChild(item);
      });

      renderStats();
    }

    // タスク切り替え
    function toggleTask(taskId) {
      logs[todayKey][taskId] = !logs[todayKey][taskId];
      saveLogs(logs);
      init();
    }

    // ストリーク計算（指定項目の連続達成日数）
    function calculateStreak(validator) {
      let streak = 0;
      let checkDate = new Date();
      
      // 今日のチェック有無
      const todayDone = validator(logs[getDateKey(checkDate)] || {});
      if (todayDone) streak++;

      // 過去へ1日ずつ遡る
      while (true) {
        checkDate.setDate(checkDate.getDate() - 1);
        const key = getDateKey(checkDate);
        if (logs[key] && validator(logs[key])) {
          streak++;
        } else {
          break;
        }
      }
      return streak;
    }

    // 今週の月曜〜日曜のジム回数
    function calculateWeeklyGym() {
      const now = new Date();
      const currentDay = now.getDay();
      // 月曜起点（0:日曜の場合は6日前、それ以外はday-1前）
      const distanceToMonday = currentDay === 0 ? 6 : currentDay - 1;
      const monday = new Date(now);
      monday.setDate(now.getDate() - distanceToMonday);

      let count = 0;
      for (let i = 0; i < 7; i++) {
        const d = new Date(monday);
        d.setDate(monday.getDate() + i);
        const k = getDateKey(d);
        if (logs[k] && logs[k].gym) count++;
      }
      return count;
    }

    // 統計・進捗の更新描画
    function renderStats() {
      const todayData = logs[todayKey] || {};
      const completedCount = TASKS.filter(t => todayData[t.id]).length;
      const rate = Math.round((completedCount / TASKS.length) * 100);

      document.getElementById('rateDisplay').textContent = `${rate}%`;
      document.getElementById('progressFill').style.width = `${rate}%`;

      // 今週のジム
      const gymCount = calculateWeeklyGym();
      const gymEl = document.getElementById('gymProgress');
      gymEl.innerHTML = `${gymCount} <span class="stat-sub">/ 3回</span>`;
      if (gymCount >= 3) gymEl.style.color = '#10b981';

      // 各項目のストリーク
      document.getElementById('brushStreak').innerHTML = 
        `${calculateStreak(d => d.brush)} <span class="stat-sub">日連続</span>`;
      document.getElementById('proteinStreak').innerHTML = 
        `${calculateStreak(d => d.protein1 && d.protein2)} <span class="stat-sub">日連続</span>`;
      document.getElementById('mealStreak').innerHTML = 
        `${calculateStreak(d => d.meal)} <span class="stat-sub">日連続</span>`;

      // 直近7日間のドットヒートマップ
      const historyEl = document.getElementById('weekHistory');
      historyEl.innerHTML = '';
      const dayLabels = ['日', '月', '火', '水', '木', '金', '土'];
      
      for (let i = 6; i >= 0; i--) {
        const d = new Date();
        d.setDate(d.getDate() - i);
        const k = getDateKey(d);
        const dayLog = logs[k] || {};
        const count = TASKS.filter(t => dayLog[t.id]).length;

        const dotContainer = document.createElement('div');
        dotContainer.className = 'dot-day';

        let statusClass = '';
        if (count === TASKS.length) statusClass = 'full';
        else if (count > 0) statusClass = 'partial';

        dotContainer.innerHTML = `
          <div class="dot ${statusClass}">${count}</div>
          <div class="dot-label">${dayLabels[d.getDay()]}</div>
        `;
        historyEl.appendChild(dotContainer);
      }
    }

    init();
  </script>
</body>
</html>
