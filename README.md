<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
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
    <h1>Bouldering Live Link <a href="https://bouldering-sample.netlify.app">Here</a></h1>
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
    <div><span class="prompt">$</span> <span class="cmd">git clone https://github.com/alenjeeson0/bouldering_sample.git</span></div>
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
