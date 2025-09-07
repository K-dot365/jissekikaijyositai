<!doctype html>
<html lang="ja">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>香川旅行</title>
  <style>
    :root {
      --bg: #0e0f10;
      --panel: #15191e;
      --border: #2b3139;
      --text: #dfe7ef;
      --muted: #8d99a6;
      --btn: #1e242b;
      --btn-hover: #28313a;
      --accent: #4caf50;
      --accent-glow: #b3ffb8;
      --gold: #f4c542;
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0;
      background: radial-gradient(1000px 600px at 20% -10%, #1b2027, var(--bg));
      color: var(--text);
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Noto Sans JP", "Hiragino Kaku Gothic ProN", "Yu Gothic", Meiryo, sans-serif;
      display: grid;
      place-items: center;
      padding: 24px;
    }
    .app { width: min(1100px, 96vw); }
    header {
      display:flex;
      align-items: center;
      justify-content: space-between; /* または flex-start */
      gap: 12px;
      margin-bottom: 14px;
      flex-wrap: wrap;
    }
    h1 {
      font-size: clamp(18px, 2.3vw, 24px);
      margin: 0;
      letter-spacing: .02em;
    }
    .controls {
      display:flex;
      flex-wrap: wrap;
      gap: 8px;
      align-items: center;
    }
    .control, button, select, input[type="number"] {
      background: var(--btn);
      color: var(--text);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 8px 12px;
      font: inherit;
      transition: transform .02s ease, background .2s ease, border-color .2s ease;
      outline: none;
    }
    button:hover, select:hover, input[type="number"]:hover { background: var(--btn-hover); }
    button:active { transform: translateY(1px); }
    .grid {
      background: linear-gradient(180deg, #13171c, var(--panel));
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 16px;
      position: relative;
    }
    .cells { display: grid; gap: 12px; }
    .cell { position: relative; }
    .cell button {
      width: 100%;
      aspect-ratio: 1 / 1;
      border-radius: 14px;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      background: #0f1419;
      border: 1px solid #212932;
      box-shadow: inset 0 0 0 1px rgba(255,255,255,.03);
      min-width: 44px;
      min-height: 44px;
    }
    .cell button .label {
      position: absolute;
      left: 10px;
      bottom: 8px;
      right: 10px;
      font-size: 12px;
      color: var(--muted);
      line-height: 1.2;
    }
    .cell button .badge {
      position: absolute;
      top: 8px;
      right: 8px;
      font-size: 11px;
      padding: 4px 8px;
      border-radius: 999px;
      background: #1b222a;
      border:1px solid #2a313a;
      color: var(--muted);
    }
    .cell button.lit {
      border-color: rgba(76, 175, 80, .7);
      box-shadow: 0 0 0 1px rgba(76, 175, 80, .7),
                  0 4px 22px 0 rgba(76, 175, 80, .25),
                  inset 0 0 18px rgba(76, 175, 80, .25);
      background: radial-gradient(120px 120px at 30% 20%, rgba(76,175,80,.20), transparent), #0f1419;
    }
    .cell button.lit img,
    .cell button.lit .cell-text {
      filter: brightness(1.3) drop-shadow(0 0 10px rgba(76, 255, 80, 0.8));
      transition: filter 0.3s ease;
    }

    .cell button.legendary.lit {
      box-shadow: 0 0 0 1px rgba(244,197,66,.45),
                  0 6px 26px 0 rgba(244,197,66,.35),
                  inset 0 0 22px rgba(244,197,66,.3);
      background: radial-gradient(120px 120px at 30% 20%, rgba(244,197,66,.22), transparent), #0f1419;
    }

    .cell button.legendary.lit img,
    .cell button.legendary.lit .cell-text {
      filter: brightness(1.3) drop-shadow(0 0 10px rgba(255, 255, 120, 0.9));
    }

    .cell button.lit::after {
      content:"";
      position:absolute;
      inset:-4px;
      border-radius: 16px;
      pointer-events: none;
      box-shadow: 0 0 22px 8px rgba(179,255,184,.12);
    }
    
    .cell button.legendary { border-color: rgba(244,197,66,.7); }

    .footer {
      display:flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 12px;
      color: var(--muted);
      font-size: 13px;
    }
    .count { font-variant-numeric: tabular-nums; }

    /* 📱 スマホ用調整 */
    @media (max-width: 600px) {
      body { padding: 12px; }
      header { flex-direction: column; align-items: flex-start; gap: 8px; }
      .controls { width: 100%; justify-content: flex-start; }
      .cell button .label { font-size: 10px; }
      .cell button .badge { font-size: 9px; padding: 2px 6px; }
      h1 { font-size: 16px; }
    }

    .cell {
      position: relative;
      width: 100%;
      aspect-ratio: 1/1;
      overflow: hidden;
      border-radius: 8px;
    }
    .cell img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
    }
    .cell-text {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.5);
      color: white;
      font-weight: bold;
      text-align: center;
      padding: 4px 0;
      font-size: 12px;
    }

    /* h1 と進捗ボタンを横並びにする */
    .title-row {
      display: flex;
      align-items: center;
      gap: 12px; /* h1 とボタンの間の余白 */
      flex-wrap: wrap; /* スマホで折り返すように */
    }
  </style>
</head>
<body>
  <div class="app">
    <header>
      <div class="title-row">
        <h1>香川旅行</h1>
      </div>
      
      <div class="controls">
        <select id="preset">
          <option value="day1">Day 1</option>
          <option value="day2">Day 2</option>
        </select>
        <button id="reset">すべて消灯</button>
      </div>
    </header>

    <section class="grid">
      <div id="cells" class="cells"></div>
      <div class="footer">
        <div class="count"><span id="litCount">0</span> / <span id="totalCount">0</span> 解放</div>
        <div class="hint">セルをクリックで点灯/消灯</div>
      </div>
    </section>
  </div>

  <script>
    const cellsEl = document.getElementById('cells');
    const resetBtn = document.getElementById('reset');
    const presetEl = document.getElementById('preset');
    const litCountEl = document.getElementById('litCount');
    const totalCountEl = document.getElementById('totalCount');
    // const globalProgressBtn = document.getElementById("globalProgressBtn"); // 削除

    const PRESETS = {
      "day1": {
        size:[3,3],
        labels:[
          {img:"実績解除画像/ex001.jpg",text:"9:30集合に間に合う"},
          {img:"実績解除画像/ex001.jpg",text:"11時半お昼ご飯でうどんを食べる"},
          {img:"実績解除画像/ex001.jpg",text:"14時ごろ栗林公園で記念撮影！"},
          {img:"実績解除画像/ex001.jpg",text:"16時までにチェックイン"},
          {img:"実績解除画像/ex001.jpg",text:"17時アンチックよろずやに寄る？？"},
          {img:"実績解除画像/ex001.jpg",text:"17時~18時大急ぎ金毘羅表参道"},
          {img:"実績解除画像/ex001.jpg",text:"ついでに金毘羅宮を参拝"},
          {img:"実績解除画像/ex001.jpg",text:"夜ご飯を見つけよう！"},
          {img:"実績解除画像/ex001.jpg",text:"20時半~宿でまったり"},
          {img:"実績解除画像/ex051.jpg",text:"初日を楽しんだぞ！！"},
        ],
        legendary:[8]
      },
      "day2": {
        size:[4,3],
        labels:[
          {img:"実績解除画像/st001.jpg",text:"おはよう"},
          {img:"実績解除画像/ex001.jpg",text:"10時チェックアウト"},
          {img:"実績解除画像/ex001.jpg",text:"10時半～四国水族館"},
          {img:"実績解除画像/ex001.jpg",text:"さすがにうどん以外の昼ご飯"},
          {img:"実績解除画像/ex001.jpg",text:"15時~17時天空の鳥居？？"},
          {img:"実績解除画像/ex001.jpg",text:"17時~18時半夕日の父母ヶ浜"},
          {img:"実績解除画像/ex001.jpg",text:"夜ご飯はやっぱりうどん！"},
          {img:"実績解除画像/ex001.jpg",text:"19時半~20時半天空の鳥居？？"},
          {img:"実績解除画像/ex001.jpg",text:"23時ごろ着 無事に帰りましょう！"},
          {img:"実績解除画像/ex001.jpg",text:"旅行めちゃめちゃ楽しかった！"},
          null,
          null,
        ],
        legendary:[9]
      },
    };
    
    let R = 4, C = 5;
    let labels = [];
    let legendary = new Set();
    let currentPreset = presetEl.value; // ✅ 初期化をここで

    function buildGrid(r=R, c=C, givenLabels=null) {
      R = r;
      C = c;
      cellsEl.style.gridTemplateColumns = `repeat(${C}, minmax(50px, 1fr))`;

      if (givenLabels && givenLabels.length) {
        labels = givenLabels;
      } else {
        labels = Array.from({length: r*c}, (_,i)=>`実績 ${i+1}`);
      }
      
      cellsEl.innerHTML = '';

      for (let i=0; i<r*c; i++) {
        const label = labels[i] || null;
        const cell = document.createElement('div');
        cell.className = 'cell';
        
        if (label === null) {
          cellsEl.appendChild(cell);
          continue;
        }

        const btn = document.createElement('button');
        btn.type = 'button';
        btn.dataset.idx = i;
        btn.setAttribute('aria-pressed', 'false');
        if (legendary.has(i)) btn.classList.add('legendary');

        let imgSrc = "images/placeholder.png";
        let textLabel = "";

        if (typeof label === "object") {
          imgSrc = label.img || imgSrc;
          textLabel = label.text || "";
        } else if (typeof label === "string") {
          if (label.match(/\.(jpg|png|gif)$/)) imgSrc = label;
          else textLabel = label;
        }

        btn.innerHTML =`
          <span class="badge">#${i+1}</span>
          <img src="${imgSrc}" alt="" loading="lazy">
          <span class="cell-text">${textLabel}</span>`;

        btn.addEventListener('click', () => toggle(btn));
        cell.appendChild(btn);
        cellsEl.appendChild(cell);
      }
    }

    function toggle(btn){
      const idx = +btn.dataset.idx;
      const specialPresets = ["day1", "day2"]; // プリセット名を更新

      // 最後のマスはクリック禁止 (day1, day2の最後のセルは自動解除されるため)
      if (specialPresets.includes(presetEl.value)) {
        const allBtns = Array.from(cellsEl.querySelectorAll('button'))
                        .filter(b => labels[b.dataset.idx] !== null);
        const lastBtn = allBtns[allBtns.length - 1];
        if (btn === lastBtn) return;
      }

      const lit = btn.classList.toggle('lit');
      btn.setAttribute('aria-pressed', String(lit));
      updateCounts();
      save();//クリックごとに自動保存
      // checkProgressButtons(); // 進捗ボタン削除のためコメントアウトまたは削除
    }

    function resetAll() {
      // 表示中のセルを消灯
      cellsEl.querySelectorAll('button.lit').forEach(b => {
        b.classList.remove('lit');
        b.setAttribute('aria-pressed','false');
      });

      localStorage.removeItem(getStorageKey(presetEl.value));

      updateCounts(); // カウントを更新し、特殊解除を再評価
      // checkProgressButtons(); // 進捗ボタン削除のためコメントアウトまたは削除
    }

    function updateCounts(){
      // ✅ day2 (旧stargazing-specialist) 専用処理
      if (presetEl.value === "day2") {
        const allButtons = Array.from(cellsEl.querySelectorAll('button[data-idx]'));
        const lastBtn = cellsEl.querySelector('button[data-idx="25"]'); // #26
        if (lastBtn) {
          // 最初の5つ (インデックス0〜4)
          const firstFiveLit = [0,1,2,3,4].every(i =>
            cellsEl.querySelector(`button[data-idx="${i}"]`)?.classList.contains('lit')
          );

          // 6〜25 番 (インデックス5〜24)
          let litCount = 0;
          for (let i = 5; i <= 24; i++) {
            if (cellsEl.querySelector(`button[data-idx="${i}"]`)?.classList.contains('lit')) {
              litCount++;
            }
          }

          if (firstFiveLit && litCount >= 15) {
            lastBtn.classList.add('lit');
            lastBtn.setAttribute('aria-pressed','true');
          } else {
            lastBtn.classList.remove('lit');
            lastBtn.setAttribute('aria-pressed','false');
          }
        }
      }

      // ✅ day1 (旧tenkenmin) の特殊処理 (最後が自動解除されるプリセット)
      const specialPresetsForLastBtn = ["day1"]; // day2は上記の専用処理で賄われるためday1のみ
      if (specialPresetsForLastBtn.includes(presetEl.value)) {
          const allButtons = cellsEl.querySelectorAll('button[data-idx]');
          const lastBtnCandidate = Array.from(cellsEl.querySelectorAll('button'))
                            .filter(b => labels[b.dataset.idx] !== null)
                            .pop();

          let lastIdx = -1;
          if (lastBtnCandidate) {
              lastIdx = +lastBtnCandidate.dataset.idx;
          }

          if (lastIdx !== -1) { // lastBtnCandidate が存在する場合のみ処理
              const otherBtns = Array.from(allButtons).filter(b => +b.dataset.idx !== lastIdx);
              const allLit = otherBtns.every(b => b.classList.contains('lit'));

              if (allLit) {
                  lastBtnCandidate.classList.add('lit');
                  lastBtnCandidate.setAttribute('aria-pressed', 'true');
              } else {
                  lastBtnCandidate.classList.remove('lit');
                  lastBtnCandidate.setAttribute('aria-pressed', 'false');
              }
          }
      }

      // ✅ litCount を正しく計算（legendary も含む）
      const litButtons = Array.from(cellsEl.querySelectorAll('button.lit'))
        .filter(b => labels[b.dataset.idx] !== null); // 無効セル(null)は除外

      litCountEl.textContent = litButtons.length;
      totalCountEl.textContent = labels.filter(l => l !== null).length; // totalCountEl もここで更新

      // updateGlobalProgress(); // 全体進捗ボタン削除のためコメントアウトまたは削除
      // checkProgressButtons(); // 進捗インジケーター削除のためコメントアウトまたは削除
    }

    // 進捗インジケーター更新（削除）
    function checkProgressButtons() {
      // この関数は進捗ボタンの削除に伴い、呼び出されないため処理を空にするか削除します。
      // 今回は完全に削除します。
    }

    function getStorageKey(presetName) {
      return `achievements-${presetName}`;
    }

    function save(presetName = presetEl.value) {
      const lit = Array.from(cellsEl.querySelectorAll('button.lit'))
        .map(b => +b.dataset.idx);

      const data = { lit };
      localStorage.setItem(getStorageKey(presetName), JSON.stringify(data));
    }

    // ✅ 状態読み込み
    function load(presetName = presetEl.value) {
      const raw = localStorage.getItem(getStorageKey(presetName));
      // 一度すべて消灯
      cellsEl.querySelectorAll('button').forEach(b=>{
        b.classList.remove('lit');
        b.setAttribute('aria-pressed','false');
      });

      if (!raw) {
        updateCounts(); // 保存データがない場合もカウントを更新し、特殊解除を再評価
        return;
      }
      try {
        const data = JSON.parse(raw);
        if (!data || !Array.isArray(data.lit)) {
          updateCounts(); // データが不正な場合もカウントを更新
          return;
        }

        // 保存されていたインデックスを再点灯
        data.lit.forEach(idx=>{
          const btn = cellsEl.querySelector(`button[data-idx="${idx}"]`);
          if (btn) {
            btn.classList.add('lit');
            btn.setAttribute('aria-pressed','true');
          }
        });

        updateCounts();
      } catch(e) {
        console.error("load failed", e);
        updateCounts(); // エラー時もカウントを更新
      }
    }

    function usePreset(name){
      const p = PRESETS[name];
      if (!p) return;
      legendary = new Set(p.legendary || []);
      buildGrid(p.size[0], p.size[1], p.labels);
    }
    
    presetEl.addEventListener('change', (e)=>{
      const newPreset = e.target.value;
      if (!newPreset) return;

      save(currentPreset);     // 旧プリセットを保存
      usePreset(newPreset);     // 新プリセットに切替 (DOM再構築)
      load(newPreset);          // 新プリセットの保存済み状態を読み込み
      currentPreset = newPreset; // 更新

      // 最後に選択したプリセットを保存
      localStorage.setItem('lastPreset', newPreset);
    });

    resetBtn.addEventListener('click', resetAll);

    // ✅ 全体進捗更新関数（削除）
    function updateGlobalProgress() {
      // この関数は全体進捗ボタンの削除に伴い、呼び出されないため処理を空にするか削除します。
      // 今回は完全に削除します。
    }

    // ✅ ページ読み込み時
    window.addEventListener('DOMContentLoaded', () => {
      const last = localStorage.getItem("lastPreset");
      let initialPreset = "day1"; // デフォルトプリセットをday1に
      if (last && PRESETS[last]) {
        initialPreset = last;
      }
      
      presetEl.value = initialPreset;
      currentPreset = initialPreset; // currentPresetもここで初期化
      
      usePreset(initialPreset); // 初回表示
      load(initialPreset);      // 保存データを読み込み
    });

  </script>
</body>
</html>
