<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>README — Boulder Inc.</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Segoe UI', system-ui, sans-serif;
      background: #0d1117;
      color: #e6edf3;
      line-height: 1.7;
      padding: 40px 20px;
    }

    .container {
      max-width: 860px;
      margin: 0 auto;
    }

    /* Header */
    .readme-header {
      border-bottom: 1px solid #30363d;
      padding-bottom: 24px;
      margin-bottom: 32px;
    }

    .readme-header h1 {
      font-size: 2rem;
      font-weight: 700;
      color: #e6edf3;
      margin-bottom: 8px;
    }

    .readme-header p {
      color: #8b949e;
      font-size: 1rem;
    }

    .badge {
      display: inline-block;
      background: #087A98;
      color: #fff;
      font-size: 0.75rem;
      font-weight: 600;
      padding: 3px 10px;
      border-radius: 20px;
      margin-right: 6px;
      margin-bottom: 12px;
    }
    .badge.green { background: #238636; }
    .badge.orange { background: #cb731c; }

    /* Sections */
    h2 {
      font-size: 1.25rem;
      font-weight: 600;
      color: #e6edf3;
      margin: 32px 0 12px;
      padding-bottom: 6px;
      border-bottom: 1px solid #21262d;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    p { color: #c9d1d9; margin-bottom: 10px; }

    /* File tree */
    .file-tree {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 20px 24px;
      font-family: 'Courier New', monospace;
      font-size: 0.9rem;
      color: #c9d1d9;
      line-height: 2;
    }

    .file-tree .folder { color: #58a6ff; }
    .file-tree .file   { color: #c9d1d9; }
    .file-tree .comment { color: #8b949e; }

    /* Pages */
    .page-card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 18px 20px;
      margin-bottom: 12px;
    }

    .page-card h3 {
      color: #58a6ff;
      font-size: 1rem;
      margin-bottom: 6px;
    }

    .page-card ul {
      padding-left: 18px;
      color: #8b949e;
      font-size: 0.9rem;
    }

    .page-card ul li { margin-bottom: 4px; }

    /* Features grid */
    .features-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }

    .feature-item {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 12px 16px;
      font-size: 0.9rem;
      color: #c9d1d9;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .feature-item span.icon { font-size: 1.1rem; }

    /* Code block */
    .code-block {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 16px 20px;
      font-family: 'Courier New', monospace;
      font-size: 0.88rem;
      color: #c9d1d9;
      line-height: 1.9;
    }

    .code-block .prompt { color: #238636; }
    .code-block .cmd    { color: #79c0ff; }
    .code-block .comment { color: #8b949e; }

    /* TODO list */
    .todo-list {
      list-style: none;
      padding: 0;
    }

    .todo-list li {
      display: flex;
      align-items: flex-start;
      gap: 10px;
      padding: 8px 0;
      border-bottom: 1px solid #21262d;
      font-size: 0.92rem;
      color: #c9d1d9;
    }

    .todo-list li:last-child { border-bottom: none; }

    .todo-box {
      width: 16px;
      height: 16px;
      border: 1px solid #30363d;
      border-radius: 3px;
      flex-shrink: 0;
      margin-top: 3px;
    }

    .severity {
      font-size: 0.75rem;
      padding: 2px 8px;
      border-radius: 20px;
      font-weight: 600;
      white-space: nowrap;
    }

    .severity.red    { background: #3d1f1f; color: #f85149; }
    .severity.yellow { background: #2f2a1a; color: #e3b341; }
    .severity.green  { background: #1a2f1a; color: #3fb950; }

    /* Author */
    .author-card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 20px;
      display: flex;
      align-items: center;
      gap: 16px;
    }

    .avatar {
      width: 48px;
      height: 48px;
      border-radius: 50%;
      background: linear-gradient(135deg, #087A98, #0b4a5a);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      flex-shrink: 0;
    }

    .author-info h3 { color: #e6edf3; font-size: 1rem; margin-bottom: 4px; }
    .author-info p  { color: #8b949e; font-size: 0.88rem; margin: 0; }

    footer.readme-footer {
      margin-top: 40px;
      padding-top: 20px;
      border-top: 1px solid #21262d;
      text-align: center;
      color: #8b949e;
      font-size: 0.85rem;
    }
  </style>
</head>
<body>
<div class="container">

  <!-- Header -->
  <div class="readme-header">
    <h1>🧗 Boulder Inc. — Bouldering Website</h1>
    <div>
      <span class="badge">HTML5</span>
      <span class="badge green">CSS3</span>
      <span class="badge orange">Static Site</span>
      <span class="badge">Beginner Project</span>
    </div>
    <p>A beginner-friendly static website about bouldering, built with pure HTML and CSS. Created as a learning project while exploring web development fundamentals.</p>
  </div>

  <!-- File Structure -->
  <h2>📁 Project Structure</h2>
  <div class="file-tree">
    <div><span class="folder">project/</span></div>
    <div>&nbsp;&nbsp;├── <span class="file">index.html</span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="comment"># Home page</span></div>
    <div>&nbsp;&nbsp;├── <span class="file">getting-started.html</span> &nbsp;&nbsp; <span class="comment"># Getting Started page</span></div>
    <div>&nbsp;&nbsp;├── <span class="folder">css/</span></div>
    <div>&nbsp;&nbsp;│&nbsp;&nbsp; └── <span class="file">style.css</span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="comment"># Main stylesheet</span></div>
    <div>&nbsp;&nbsp;└── <span class="folder">images/</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── <span class="file">logo.svg</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── <span class="file">bouldering-gym.jpg</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── <span class="file">what-is-bouldering.jpg</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── <span class="file">why-bouldering.jpg</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── <span class="file">getting-started-outdoors.jpg</span></div>
    <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── <span class="file">simple-steps.jpg</span></div>
  </div>

  <!-- Pages -->
  <h2>📄 Pages</h2>
  <div class="page-card">
    <h3>🏠 Home (index.html)</h3>
    <ul>
      <li>Hero heading and gym image</li>
      <li>"What is Bouldering?" section with two-column layout</li>
      <li>"Why Bouldering?" section with a reasons list</li>
      <li>Teal highlight block with motivational blurb</li>
    </ul>
  </div>
  <div class="page-card">
    <h3>🚀 Getting Started (getting-started.html)</h3>
    <ul>
      <li>Introduction to starting bouldering</li>
      <li>"Know Before You Go" safety tips with background image</li>
      <li>Step-by-step guide in a two-column layout</li>
      <li>Outdoor climbing image</li>
    </ul>
  </div>

  <!-- Built With -->
  <h2>🛠️ Built With</h2>
  <div class="features-grid">
    <div class="feature-item"><span class="icon">🌐</span> HTML5 — Semantic structure</div>
    <div class="feature-item"><span class="icon">🎨</span> CSS3 — Grid &amp; Flexbox</div>
    <div class="feature-item"><span class="icon">📱</span> Responsive layout</div>
    <div class="feature-item"><span class="icon">⚡</span> No frameworks or libraries</div>
  </div>

  <!-- Features -->
  <h2>✨ Features</h2>
  <div class="features-grid">
    <div class="feature-item"><span class="icon">🔲</span> Two-column CSS Grid layout</div>
    <div class="feature-item"><span class="icon">🧭</span> Navigation with hover/focus styles</div>
    <div class="feature-item"><span class="icon">🖼️</span> Background image section with text</div>
    <div class="feature-item"><span class="icon">🎨</span> Teal-themed footer &amp; highlight blocks</div>
    <div class="feature-item"><span class="icon">♿</span> Semantic HTML (nav, main, footer)</div>
    <div class="feature-item"><span class="icon">🔗</span> Multi-page internal navigation</div>
  </div>

  <!-- Getting Started -->
  <h2>🚀 Running Locally</h2>
  <div class="code-block">
    <div><span class="comment"># 1. Clone the repo</span></div>
    <div><span class="prompt">$</span> <span class="cmd">git clone https://github.com/your-username/boulder-inc.git</span></div>
    <br>
    <div><span class="comment"># 2. Open in browser — no build step needed</span></div>
    <div><span class="prompt">$</span> <span class="cmd">open index.html</span></div>
    <br>
    <div><span class="comment"># Or just double-click index.html in your file explorer</span></div>
  </div>

  <!-- TODO -->
  <h2>🐛 Known Issues / TODO</h2>
  <ul class="todo-list">
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Fix broken anchor text on Getting Started page — "is surprisingly simple" missing subject "bouldering"</span>
      <span class="severity red">🔴 Bug</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Fix typo: "tart with easy routes" → "Start with easy routes"</span>
      <span class="severity yellow">🟡 Typo</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Scope <code>ul li::marker</code> emoji to sections only — currently affects nav list too</span>
      <span class="severity red">🔴 Bug</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Update copyright year from 2025 → 2026</span>
      <span class="severity yellow">🟡 Minor</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Add <code>lang="en"</code> to both HTML files</span>
      <span class="severity green">🟢 Best Practice</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Add <code>&lt;meta charset&gt;</code> and <code>&lt;meta viewport&gt;</code> to both files</span>
      <span class="severity green">🟢 Best Practice</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Remove duplicate <code>a { color: inherit; }</code> rule from CSS</span>
      <span class="severity yellow">🟡 Dead Code</span>
    </li>
    <li>
      <div class="todo-box"></div>
      <span style="flex:1">Add mobile responsive styles (media queries)</span>
      <span class="severity green">🟢 Enhancement</span>
    </li>
  </ul>

  <!-- Author -->
  <h2>👤 Author</h2>
  <div class="author-card">
    <div class="avatar">🧗</div>
    <div class="author-info">
      <h3>Alen</h3>
      <p>Self-taught web developer based in Bengaluru, India 🇮🇳 · Building toward a React/MERN developer role</p>
    </div>
  </div>

  <!-- License -->
  <h2>📜 License</h2>
  <p>This project is open source and available under the <strong style="color:#58a6ff">MIT License</strong>.</p>

  <footer class="readme-footer">
    <p>Made with 🤍 · Boulder Inc. · 2026</p>
  </footer>

</div>
</body>
</html>
