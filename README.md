<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Ahmad Saleh — Profile</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css"/>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700&family=Space+Grotesk:wght@400;500;600&display=swap" rel="stylesheet"/>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body { background: #010409; display: flex; justify-content: center; align-items: flex-start; min-height: 100vh; padding: 40px 16px; }

.profile-wrap {
  font-family: 'JetBrains Mono', monospace;
  background: #0d1117;
  color: #c9d1d9;
  border-radius: 12px;
  overflow: hidden;
  width: 100%;
  max-width: 680px;
  border: 1px solid #21262d;
  position: relative;
}

.grid-bg {
  position: absolute; inset: 0; pointer-events: none; z-index: 0;
  background-image:
    linear-gradient(rgba(88,166,255,0.04) 1px, transparent 1px),
    linear-gradient(90deg, rgba(88,166,255,0.04) 1px, transparent 1px);
  background-size: 40px 40px;
}

.header-bar {
  background: #161b22;
  border-bottom: 1px solid #21262d;
  padding: 10px 16px;
  display: flex; align-items: center; gap: 8px;
  position: relative; z-index: 1;
}
.dot { width: 12px; height: 12px; border-radius: 50%; }
.dot-r { background: #ff5f57; }
.dot-y { background: #febc2e; }
.dot-g { background: #28c840; }
.header-title { color: #6e7681; font-size: 12px; margin-left: 8px; letter-spacing: 0.5px; }

.content { position: relative; z-index: 1; padding: 24px 28px; }

.intro-block { display: flex; gap: 20px; align-items: flex-start; margin-bottom: 24px; }

.avatar-ring {
  flex-shrink: 0;
  width: 72px; height: 72px;
  border-radius: 50%;
  background: linear-gradient(135deg, #58a6ff, #bc8cff, #79c0ff);
  padding: 2px;
  display: flex; align-items: center; justify-content: center;
}
.avatar-inner {
  width: 100%; height: 100%; border-radius: 50%;
  background: #0d1117;
  display: flex; align-items: center; justify-content: center;
  font-size: 22px; font-weight: 700; color: #58a6ff;
  letter-spacing: -1px;
}

.name { font-size: 22px; font-weight: 700; color: #e6edf3; font-family: 'Space Grotesk', sans-serif; }
.role { font-size: 13px; color: #58a6ff; margin: 4px 0 2px; letter-spacing: 0.3px; }
.location { font-size: 12px; color: #6e7681; }

.status-pill {
  display: inline-flex; align-items: center; gap: 6px;
  background: rgba(35,134,54,0.15); border: 1px solid rgba(35,134,54,0.4);
  border-radius: 20px; padding: 3px 10px; font-size: 11px; color: #3fb950; margin-top: 8px;
}
.status-dot { width: 7px; height: 7px; border-radius: 50%; background: #3fb950; animation: pulse 2s infinite; }
@keyframes pulse { 0%,100%{opacity:1} 50%{opacity:0.4} }

.section-label {
  font-size: 11px; color: #58a6ff; letter-spacing: 1.5px; text-transform: uppercase;
  margin-bottom: 12px; display: flex; align-items: center; gap: 8px;
}
.section-label::after { content: ''; flex: 1; height: 1px; background: #21262d; }

.code-block {
  background: #161b22;
  border: 1px solid #21262d;
  border-radius: 8px;
  padding: 16px;
  font-size: 12px;
  line-height: 1.8;
  margin-bottom: 20px;
}
.kw  { color: #ff7b72; }
.fn  { color: #d2a8ff; }
.str { color: #a5d6ff; }
.cm  { color: #8b949e; }
.var { color: #ffa657; }
.cl  { color: #79c0ff; }
.indent1 { padding-left: 16px; display: block; }
.indent2 { padding-left: 32px; display: block; }

.skills-grid {
  display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; margin-bottom: 20px;
}
.skill-card {
  background: #161b22; border: 1px solid #21262d; border-radius: 8px; padding: 12px;
  transition: border-color 0.2s;
}
.skill-card:hover { border-color: rgba(88,166,255,0.3); }
.skill-cat { font-size: 10px; color: #8b949e; letter-spacing: 1px; text-transform: uppercase; margin-bottom: 8px; }
.skill-tags { display: flex; flex-wrap: wrap; gap: 5px; }
.tag {
  font-size: 10px; padding: 2px 8px; border-radius: 4px;
  background: rgba(88,166,255,0.1); border: 1px solid rgba(88,166,255,0.2); color: #58a6ff;
}
.tag.green  { background: rgba(63,185,80,0.1);  border-color: rgba(63,185,80,0.2);  color: #3fb950; }
.tag.purple { background: rgba(188,140,255,0.1); border-color: rgba(188,140,255,0.2); color: #bc8cff; }
.tag.orange { background: rgba(255,166,87,0.1);  border-color: rgba(255,166,87,0.2);  color: #ffa657; }

.links-row { display: flex; gap: 10px; flex-wrap: wrap; }
.link-btn {
  display: inline-flex; align-items: center; gap: 7px;
  background: #161b22; border: 1px solid #21262d; border-radius: 6px;
  padding: 8px 14px; font-size: 12px; color: #c9d1d9; text-decoration: none;
  font-family: 'JetBrains Mono', monospace;
  transition: border-color 0.2s, color 0.2s;
}
.link-btn:hover { border-color: #58a6ff; color: #58a6ff; }
.link-btn i { font-size: 14px; }

.quote-bar {
  margin-top: 20px;
  border-left: 3px solid #58a6ff;
  padding: 10px 14px;
  background: rgba(88,166,255,0.05);
  border-radius: 0 6px 6px 0;
  font-size: 12px; color: #8b949e; font-style: italic; line-height: 1.6;
}
.quote-bar span { color: #6e7681; }
</style>
</head>
<body>
<div class="profile-wrap">
  <div class="grid-bg"></div>
  <div class="header-bar">
    <div class="dot dot-r"></div>
    <div class="dot dot-y"></div>
    <div class="dot dot-g"></div>
    <span class="header-title">~/AhmadHakeem03/README.md</span>
  </div>
  <div class="content">

    <!-- Intro -->
    <div class="intro-block">
      <div class="avatar-ring">
        <div class="avatar-inner">AS</div>
      </div>
      <div>
        <div class="name">Ahmad Saleh</div>
        <div class="role">Data Scientist &amp; ML Engineer</div>
        <div class="location">
          <i class="ti ti-map-pin" style="font-size:13px;vertical-align:-1px;margin-right:4px;"></i>
          Jordan, Amman
        </div>
        <div class="status-pill">
          <span class="status-dot"></span>Building intelligent systems 🚀
        </div>
      </div>
    </div>

    <!-- About -->
    <div class="section-label">about</div>
    <div class="code-block">
      <span><span class="kw">class</span> <span class="cl">DataScientist</span>:</span>
      <span class="indent1"><span class="kw">def</span> <span class="fn">__init__</span>(<span class="var">self</span>):</span>
      <span class="indent2"><span class="var">self</span>.name     = <span class="str">"Ahmad Saleh"</span></span>
      <span class="indent2"><span class="var">self</span>.focus    = [<span class="str">"ML"</span>, <span class="str">"Deep Learning"</span>, <span class="str">"Data Science"</span>]</span>
      <span class="indent2"><span class="var">self</span>.backend  = [<span class="str">"FastAPI"</span>, <span class="str">"REST APIs"</span>, <span class="str">"LLM Integration"</span>]</span>
      <span class="indent2"><span class="var">self</span>.langs    = [<span class="str">"Python"</span>, <span class="str">"C++"</span>, <span class="str">"Java"</span>]</span>
      <span class="indent1"><span class="cm"># "Without data, you're just another person with an opinion."</span></span>
    </div>

    <!-- Skills -->
    <div class="section-label">skills</div>
    <div class="skills-grid">
      <div class="skill-card">
        <div class="skill-cat">ML / Deep Learning</div>
        <div class="skill-tags">
          <span class="tag purple">PyTorch</span>
          <span class="tag purple">TensorFlow</span>
          <span class="tag purple">Scikit-Learn</span>
          <span class="tag purple">XGBoost</span>
          <span class="tag purple">OpenCV</span>
        </div>
      </div>
      <div class="skill-card">
        <div class="skill-cat">Data Science</div>
        <div class="skill-tags">
          <span class="tag green">Pandas</span>
          <span class="tag green">NumPy</span>
          <span class="tag green">Matplotlib</span>
          <span class="tag green">Seaborn</span>
          <span class="tag green">Plotly</span>
        </div>
      </div>
      <div class="skill-card">
        <div class="skill-cat">Backend &amp; APIs</div>
        <div class="skill-tags">
          <span class="tag orange">FastAPI</span>
          <span class="tag orange">REST APIs</span>
          <span class="tag orange">LLM Integration</span>
        </div>
      </div>
      <div class="skill-card">
        <div class="skill-cat">Languages &amp; Tools</div>
        <div class="skill-tags">
          <span class="tag">Python</span>
          <span class="tag">C++</span>
          <span class="tag">Git</span>
          <span class="tag">Linux</span>
          <span class="tag">VS Code</span>
        </div>
      </div>
    </div>

    <!-- Connect -->
    <div class="section-label">connect</div>
    <div class="links-row">
      <a class="link-btn" href="https://www.linkedin.com/in/ahmad-saleh0309/" target="_blank">
        <i class="ti ti-brand-linkedin"></i> LinkedIn
      </a>
      <a class="link-btn" href="mailto:ahmadsaleh0309@gmail.com">
        <i class="ti ti-mail"></i> ahmadsaleh0309@gmail.com
      </a>
      <a class="link-btn" href="https://github.com/AhmadHakeem03" target="_blank">
        <i class="ti ti-brand-github"></i> AhmadHakeem03
      </a>
    </div>

    <div class="quote-bar">
      "Driven by curiosity, powered by code." —
      <span>turning data into decisions, one model at a time.</span>
    </div>

  </div>
</div>
</body>
</html>
