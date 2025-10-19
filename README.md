[index.html](https://github.com/user-attachments/files/22990747/index.html)
<!doctype html>
<html lang="he" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>הנאום המלא — דף נחיתה</title>
  <style>
    :root{--bg:#f7fafc;--card:#ffffff;--muted:#6b7280;--accent:#2563eb}
    body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial; background:var(--bg); color:#0f172a}
    .container{max-width:1100px;margin:30px auto;padding:20px}
    header{background:#fff;padding:18px;border-radius:10px;box-shadow:0 1px 6px rgba(2,6,23,0.06);display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:8px;background:linear-gradient(135deg,#2563eb,#7c3aed);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700}
    nav a{margin:0 8px;color:var(--muted);text-decoration:none}
    .hero{display:flex;gap:30px;align-items:center;margin-top:24px}
    .hero .left{flex:1}
    h1{font-size:28px;margin:0 0 8px}
    p.lead{margin:0;color:var(--muted)}
    .search{display:flex;gap:8px;margin-top:18px}
    input.searchbox{flex:1;padding:10px 12px;border-radius:8px;border:1px solid #e6e9ef}
    button.btn{background:var(--accent);color:#fff;border:none;padding:10px 14px;border-radius:8px;cursor:pointer}
    .features{display:grid;grid-template-columns:repeat(2,1fr);gap:10px;margin-top:18px}
    .card{background:var(--card);padding:12px;border-radius:8px;box-shadow:0 1px 4px rgba(2,6,23,0.05)}
    .list{margin-top:12px}
    .speech{display:flex;justify-content:space-between;padding:12px 0;border-bottom:1px solid #f0f3f7}
    .meta{color:var(--muted);font-size:13px}
    .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(320px,1fr));gap:12px;margin-top:12px}
    article{background:var(--card);padding:12px;border-radius:8px}
    .actions a{margin-left:10px;color:var(--accent);text-decoration:none;font-size:13px}
    footer{margin-top:28px;color:var(--muted);font-size:13px;text-align:center}
    @media (max-width:800px){.hero{flex-direction:column}.features{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">ה</div>
        <div>
          <div style="font-weight:700">הנאום המלא</div>
          <div style="font-size:13px;color:var(--muted)">תמליל נאומים בזמן אמת — ישראל והעולם</div>
        </div>
      </div>
      <nav>
        <a href="#features">מה אנחנו עושים</a>
        <a href="#latest">נאומים אחרונים</a>
        <a href="#pricing">תמחור</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="left">
          <h1>התמליל של כל נאום — מהר יותר ממה שחשבת</h1>
          <p class="lead">קרא תמליל מלא של נאום בתוך דקות מרגע סיומו. חפש, העתיק ציטוטים, הורד טקסט או קבל סיכום — הכל במקום אחד.</p>

          <form id="searchForm" class="search" onsubmit="return false;">
            <input id="q" class="searchbox" placeholder="חפש לפי דובר, מילות מפתח או ציטוט" />
            <button id="searchBtn" class="btn">חפש</button>
          </form>

          <div class="features">
            <div class="card">📄 <strong>תמלילים מלאים</strong><div style="color:var(--muted);font-size:13px">כל נאום בתמליל טקסט מלא עם timestamps</div></div>
            <div class="card">⚡ <strong>מהירות</strong><div style="color:var(--muted);font-size:13px">תמליל בתוך דקות מרגע סיום הנאום</div></div>
            <div class="card">🔎 <strong>חיפוש חכם</strong><div style="color:var(--muted);font-size:13px">איתור מיידי של מילות מפתח, שמות וציטוטים</div></div>
            <div class="card">📝 <strong>עריכה אנושית</strong><div style="color:var(--muted);font-size:13px">שיפור בדקדוק ושמות קריטיים לפי הצורך</div></div>
          </div>
        </div>

        <aside style="width:360px">
          <div class="card">
            <div style="font-weight:600">דוגמא — נאומים אחרונים</div>
            <div class="list" id="recentList"></div>
            <div style="margin-top:10px"><a href="#latest">צפה בכל הנאומים</a></div>
          </div>
        </aside>
      </section>

      <section id="features" style="margin-top:22px">
        <h3>איך זה עובד</h3>
        <ol style="color:var(--muted);">
          <li>קבלת שידור חי או קובץ וידאו — חיבור ל-YouTube/RTMP/העלאה</li>
          <li>תמלול אוטומטי בזמן-אמת + בדיקה אנושית מהירה לשמות וציטוטים</li>
          <li>פרסום התמליל עם חיפוש, תיוג ויכולת הורדה בתוך דקות עד שעה</li>
        </ol>

        <div style="display:flex;gap:10px;margin-top:10px">
          <div class="card" style="flex:1;text-align:center"><div style="font-weight:700">20 דקות</div><div style="color:var(--muted)">זמן ממוצע לפרסום</div></div>
          <div class="card" style="flex:1;text-align:center"><div style="font-weight:700">עברית, אנגלית</div><div style="color:var(--muted)">שפות נתמכות (MVP)</div></div>
          <div class="card" style="flex:1;text-align:center"><div style="font-weight:700">TXT, PDF, DOCX</div><div style="color:var(--muted)">פורמטים להורדה</div></div>
        </div>
      </section>

      <section id="latest">
        <h3 style="margin-top:18px">נאומים אחרונים</h3>
        <div class="grid" id="speechesGrid"></div>
      </section>

      <section id="subscribe" style="margin-top:18px">
        <div class="card" style="display:flex;justify-content:space-between;align-items:center">
          <div>
            <div style="font-weight:700">רוצה לקבל עדכון מיד אחרי כל נאום רלוונטי?</div>
            <div style="color:var(--muted)">הירשם למערכת התראות לפי דובר, נושא או מיקום</div>
          </div>
          <form id="subForm" style="display:flex;gap:8px">
            <input id="email" type="email" placeholder="האימייל שלך" style="padding:8px;border-radius:6px;border:1px solid #e6e9ef" />
            <button class="btn">הירשם</button>
          </form>
        </div>
      </section>

      <section id="pricing" style="margin-top:18px">
        <h3>תמחור (MVP)</h3>
        <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:10px;margin-top:10px">
          <div class="card"><strong>חינם</strong><div style="color:var(--muted);font-size:13px;margin-top:6px">גישה לנאומים אחרונים בחינם לזמן מוגבל</div></div>
          <div class="card" style="border:2px solid #2563eb"><strong>מנוי מקצועי</strong><div style="color:var(--muted);font-size:13px;margin-top:6px">גישה לארכיון מלא, API והורדות מתקדמות</div></div>
          <div class="card"><strong>לקוחות עסקיים</strong><div style="color:var(--muted);font-size:13px;margin-top:6px">חבילות מותאמות לעיתונות ולארגונים</div></div>
        </div>
      </section>

      <footer>
        <div style="margin-top:26px">הנאום המלא • © " + new Date().getFullYear() + " כל הזכויות שמורות</div>
      </footer>
    </main>
  </div>

  <script>
    // דוגמת נתונים — החלף/הרחב עם תוכן אמיתי בעת השקת ה-MVP
    const sampleSpeeches = [
      {
        id: '1',
        title: 'נאום מנהיג — איום וביטחון',
        speaker: 'י. כהן',
        date: '18 באוקטובר 2025',
        location: 'ת\"א',
        duration: '12:34',
        preview: 'בנאום זה דיבר הדובר על מדיניות החוץ והדגשים כלפי השכנים...',
        text: 'בנאום זה דיבר הדובר על מדיניות החוץ והדגשים כלפי השכנים ואמצעי ביטחון חדשים...'
      },
      {
        id: '2',
        title: 'נאום גלובלי — שינוי אקלים',
        speaker: 'S. Johnson',
        date: '17 באוקטובר 2025',
        location: 'ניו יורק',
        duration: '9:12',
        preview: 'הדוברת הציגה חזון להפחתת פליטות ולהשקעה באנרגיות מתחדשות...',
        text: 'הדוברת הציגה חזון להפחתת פליטות ולהשקעה באנרגיות מתחדשות...'
      },
      {
        id: '3',
        title: 'נאום טקס פרסי ספרות',
        speaker: 'H. Levi',
        date: '15 באוקטובר 2025',
        location: 'ירושלים',
        duration: '6:02',
        preview: 'נאום מרגש על חשיבות התרבות במציאות עכשווית...',
        text: 'נאום מרגש על חשיבות התרבות במציאות עכשווית...'
      }
    ];

    function renderRecent() {
      const el = document.getElementById('recentList');
      el.innerHTML = '';
      sampleSpeeches.slice(0,5).forEach(s => {
        const div = document.createElement('div');
        div.className = 'speech';
        div.innerHTML = `<div><div class="meta">${s.date} • ${s.location}</div><div style="font-weight:600">${s.title}</div><div class="meta">${s.speaker}</div></div><div class="meta">${s.duration}</div>`;
        el.appendChild(div);
      });
    }

    function renderGrid(items) {
      const grid = document.getElementById('speechesGrid');
      grid.innerHTML = '';
      items.forEach(s => {
        const art = document.createElement('article');
        art.innerHTML = `
          <div style="display:flex;justify-content:space-between;align-items:flex-start">
            <div>
              <div style="font-weight:700">${escapeHtml(s.title)}</div>
              <div class="meta">${escapeHtml(s.speaker)} • ${escapeHtml(s.date)} • ${escapeHtml(s.location)}</div>
            </div>
            <div class="meta">${escapeHtml(s.duration)}</div>
          </div>
          <p style="margin-top:10px;color:var(--muted)">${escapeHtml(s.preview)}</p>
          <div style="margin-top:10px" class="actions">
            <a href="#" onclick="viewFull('${s.id}');return false">קרא תמליל מלא</a>
            <a href="#" onclick="downloadText('${s.id}');return false">הורד</a>
            <a href="#" onclick="summary('${s.id}');return false">סיכום 3 שורות</a>
          </div>
        `;
        grid.appendChild(art);
      });
    }

    function escapeHtml(str){
      if(!str) return '';
      return str.replace(/[&<>"']/g, function(m){return {'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":"&#39;"}[m]});
    }

    function viewFull(id){
      const s = sampleSpeeches.find(x=>x.id===id);
      if(!s) return alert('נאום לא נמצא');
      const w = window.open('', '_blank');
      w.document.write('<!doctype html><html lang="he" dir="rtl"><head><meta charset="utf-8"><title>'+escapeHtml(s.title)+'</title></head><body style="font-family:Arial, sans-serif;padding:20px">');
      w.document.write('<h2>'+escapeHtml(s.title)+'</h2>');
      w.document.write('<div style="color:#6b7280">'+escapeHtml(s.speaker)+' • '+escapeHtml(s.date)+' • '+escapeHtml(s.location)+'</div>');
      w.document.write('<pre style="white-space:pre-wrap;margin-top:18px;line-height:1.6">'+escapeHtml(s.text)+'</pre>');
      w.document.write('</body></html>');
    }

    function downloadText(id){
      const s = sampleSpeeches.find(x=>x.id===id);
      if(!s) return alert('נאום לא נמצא');
      const blob = new Blob([s.text], {type: 'text/plain;charset=utf-8'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = (s.title||'speech') + '.txt';
      document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
    }

    function summary(id){
      const s = sampleSpeeches.find(x=>x.id===id);
      if(!s) return alert('נאום לא נמצא');
      // Very simple auto-summary (placeholder)
      const lines = s.text.split('.').filter(Boolean).slice(0,3).map(t=>t.trim()).join('. ') + '.';
      alert('סיכום: "' + lines + '"');
    }

    document.getElementById('searchBtn').addEventListener('click', ()=>{
      const q = document.getElementById('q').value.trim().toLowerCase();
      if(!q){ renderGrid(sampleSpeeches); return; }
      const res = sampleSpeeches.filter(s => (s.title+s.speaker+s.text).toLowerCase().includes(q));
      renderGrid(res);
    });

    document.getElementById('q').addEventListener('keydown', (e)=>{ if(e.key==='Enter'){ e.preventDefault(); document.getElementById('searchBtn').click(); }});

    document.getElementById('subForm').addEventListener('submit', (e)=>{ e.preventDefault(); alert('תודה — נשלח אליך אימייל כאשר יפורסם נאום חדש.'); });

    // init
    renderRecent(); renderGrid(sampleSpeeches);
  </script>
</body>
</html>
