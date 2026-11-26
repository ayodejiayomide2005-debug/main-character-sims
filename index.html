<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Main Character Sim</title>
  <style>
    :root {
      --bg: #0b0b0f;
      --card: #15151d;
      --card-2: #1d1d28;
      --accent: #c084fc;
      --pink: #f472b6;
      --green: #34d399;
      --red: #fb7185;
      --blue: #38bdf8;
      --gold: #fbbf24;
      --text: #f4f4f6;
      --muted: #9ca3af;
      --border: #282836;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; }

    body {
      background-color: #050507;
      color: var(--text);
      display: flex;
      justify-content: center;
      min-height: 100vh;
    }

    .phone-frame {
      width: 100%;
      max-width: 430px;
      background: var(--bg);
      border-left: 1px solid var(--border);
      border-right: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      height: 100vh;
      overflow: hidden;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 13px 16px;
      border-bottom: 1px solid var(--border);
      background: var(--bg);
    }

    .logo { font-weight: 800; font-size: 1.02rem; color: var(--accent); letter-spacing: -0.4px; }
    .badge { background: rgba(192, 132, 252, 0.15); color: var(--accent); padding: 4px 10px; border-radius: 20px; font-size: 0.74rem; font-weight: 700; }

    .scroll-area {
      flex: 1;
      overflow-y: auto;
      padding: 13px 16px;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 13px;
    }

    /* Visual Character Look Card */
    .look-stage {
      display: flex;
      align-items: center;
      gap: 12px;
      background: linear-gradient(135deg, rgba(192, 132, 252, 0.12), rgba(244, 114, 182, 0.08));
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 10px 12px;
    }

    .char-portrait {
      position: relative;
      width: 66px;
      height: 66px;
      border-radius: 18px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      border: 2px solid var(--accent);
      overflow: hidden;
    }

    .hair-crown {
      position: absolute;
      top: -4px;
      left: 50%;
      transform: translateX(-50%);
      width: 48px;
      height: 22px;
      border-radius: 20px 20px 8px 8px;
      z-index: 2;
      transition: all 0.25s ease;
    }

    .hair-crown.locs { width: 54px; height: 28px; border-radius: 14px; border-bottom: 4px dashed rgba(0,0,0,0.25); }
    .hair-crown.pixie { width: 42px; height: 18px; border-radius: 18px 18px 4px 16px; }
    .hair-crown.curls { width: 56px; height: 26px; border-radius: 24px; }
    .hair-crown.sleek { width: 46px; height: 15px; border-radius: 12px 12px 2px 2px; }

    .face-emoji {
      position: relative;
      z-index: 3;
      font-size: 1.85rem;
      margin-top: 8px;
    }

    .outfit-strip {
      position: absolute;
      bottom: 0;
      width: 100%;
      height: 14px;
      font-size: 0.6rem;
      font-weight: 800;
      display: flex;
      align-items: center;
      justify-content: center;
      letter-spacing: 0.4px;
      z-index: 4;
    }

    .vibe-pill {
      display: inline-block;
      margin-top: 4px;
      font-size: 0.7rem;
      padding: 2px 8px;
      border-radius: 999px;
      background: rgba(251, 191, 36, 0.14);
      color: var(--gold);
      font-weight: 700;
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 6px;
      margin-top: 10px;
    }

    .stat-box { background: #101016; padding: 7px 4px; border-radius: 10px; border: 1px solid var(--border); text-align: center; }
    .stat-label { font-size: 0.64rem; color: var(--muted); }
    .stat-val { font-size: 0.82rem; font-weight: 700; margin-top: 2px; }

    .event-card {
      background: var(--card-2);
      border-left: 3px solid var(--accent);
      padding: 13px;
      border-radius: 12px;
      font-size: 0.88rem;
      line-height: 1.45;
    }

    .tag {
      display: inline-block;
      font-size: 0.68rem;
      font-weight: 700;
      padding: 2px 8px;
      border-radius: 6px;
      margin-bottom: 6px;
      text-transform: uppercase;
    }
    .tag-club { background: rgba(244, 114, 182, 0.2); color: var(--pink); }
    .tag-school { background: rgba(52, 211, 153, 0.2); color: var(--green); }
    .tag-drama { background: rgba(251, 113, 133, 0.2); color: var(--red); }
    .tag-social { background: rgba(56, 189, 248, 0.2); color: var(--blue); }

    .btn-stack { display: flex; flex-direction: column; gap: 7px; margin-top: 8px; }

    button {
      background: var(--accent);
      color: #0b0b0f;
      border: none;
      padding: 10px 13px;
      border-radius: 12px;
      font-weight: 700;
      font-size: 0.85rem;
      cursor: pointer;
      transition: transform 0.1s, opacity 0.2s;
    }
    button:active { transform: scale(0.98); }
    button.secondary { background: #232331; color: var(--text); font-weight: 600; text-align: left; }
    button.secondary:hover { background: #2d2d3f; }
    button.outline { background: transparent; border: 1px solid var(--accent); color: var(--accent); }

    .post-box {
      background: #101016;
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 11px;
      margin-top: 8px;
      font-size: 0.83rem;
    }
    .comment-bubble {
      background: #1a1a24;
      padding: 7px 10px;
      border-radius: 10px;
      margin-top: 6px;
      font-size: 0.79rem;
      border-left: 2px solid var(--pink);
    }
    .dm-card {
      background: #111118;
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 10px;
      margin-bottom: 8px;
    }

    .person-card {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px;
      background: #111118;
      border: 1px solid var(--border);
      border-radius: 12px;
      margin-bottom: 8px;
    }
    .mini-btn { padding: 6px 9px; font-size: 0.74rem; border-radius: 8px; }

    nav {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      background: #111117;
      border-top: 1px solid var(--border);
      padding: 6px 2px;
    }
    .nav-btn {
      background: transparent;
      color: var(--muted);
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2px;
      font-size: 0.67rem;
      padding: 6px 2px;
      border-radius: 8px;
    }
    .nav-btn.active { color: var(--accent); background: rgba(192, 132, 252, 0.12); }

    input, select {
      width: 100%;
      padding: 9px;
      margin-top: 4px;
      margin-bottom: 10px;
      background: #101016;
      border: 1px solid var(--border);
      border-radius: 10px;
      color: var(--text);
      font-size: 0.86rem;
    }

    .hidden { display: none !important; }
  </style>
</head>
<body>

<div class="phone-frame">
  <!-- SETUP SCREEN -->
  <div id="setup-screen" class="scroll-area">
    <div>
      <div class="logo" style="font-size: 1.45rem;">✨ Main Character Sim</div>
      <p style="color: var(--muted); font-size: 0.82rem; margin-top: 2px;">Style your look, choose your background, and run your era.</p>
    </div>

    <div class="card">
      <button class="outline" style="width: 100%; margin-bottom: 11px;" onclick="randomizeSetup()">🎲 Randomize Look & Background</button>

      <label class="stat-label">Character Name</label>
      <input type="text" id="char-name" value="Maya" />

      <label class="stat-label">Skin Tone & Hair Style</label>
      <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
        <select id="skin-tone">
          <option value="#f3c6a5">Warm Light</option>
          <option value="#d69e76">Golden Tan</option>
          <option value="#a86b43" selected>Rich Caramel</option>
          <option value="#5c3822">Deep Espresso</option>
        </select>
        <select id="hair-style">
          <option value="curls">Big Curls</option>
          <option value="locs">Braids / Locs</option>
          <option value="pixie">Wolf Pixie</option>
          <option value="sleek">Sleek Bob</option>
        </select>
      </div>

      <label class="stat-label">Hair Color & Signature Aesthetic</label>
      <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
        <select id="hair-color">
          <option value="#18181b" selected>Jet Black</option>
          <option value="#7c2d12">Auburn / Chestnut</option>
          <option value="#d97706">Honey Blonde</option>
          <option value="#9d174d">Burgundy Wine</option>
        </select>
        <select id="outfit-style">
          <option value="Clean Girl">Clean Girl & Gold</option>
          <option value="Streetwear">Y2K / Streetwear</option>
          <option value="Baddie Night">Late-Night Club Fit</option>
          <option value="Soft Luxury">Soft Luxury Blazer</option>
        </select>
      </div>

      <label class="stat-label">Pronouns & Romantic Interest</label>
      <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
        <select id="char-pronouns">
          <option value="She/Her">She/Her</option>
          <option value="He/Him">He/Him</option>
          <option value="They/Them">They/Them</option>
        </select>
        <select id="char-orientation">
          <option value="Women">Likes Women</option>
          <option value="Men">Likes Men</option>
          <option value="Everyone">Likes Everyone</option>
          <option value="Single">Focused on Bag</option>
        </select>
      </div>

      <label class="stat-label">Family Wealth & Parenting Style</label>
      <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
        <select id="family-wealth">
          <option value="Rich">Rich Family</option>
          <option value="Middle Class">Middle Class</option>
          <option value="Struggling">Struggling / Poor</option>
        </select>
        <select id="parent-style">
          <option value="Chill">Chill Parents</option>
          <option value="Strict">Strict Parents</option>
        </select>
      </div>

      <label class="stat-label">School / Career Path</label>
      <select id="char-major">
        <option value="Nursing & Medicine">🩺 Nursing & Medicine</option>
        <option value="Business & Finance">📈 Business & Finance</option>
        <option value="Media & Fashion">🎥 Media & Fashion</option>
        <option value="Tech & Software">💻 Tech & Software</option>
      </select>

      <button style="width: 100%; margin-top: 4px;" onclick="startGame()">Step Into Your Era →</button>
    </div>
  </div>

  <!-- MAIN GAME SCREEN -->
  <div id="game-screen" class="hidden" style="display: flex; flex-direction: column; height: 100%;">
    <header>
      <div class="logo">✨ Main Character Sim</div>
      <div class="badge" id="age-display">Age 17 • High School</div>
    </header>

    <!-- TOP PROFILE + CHARACTER LOOK CARD -->
    <div style="padding: 10px 16px 0 16px;">
      <div class="card" style="padding: 10px;">
        <div class="look-stage">
          <div class="char-portrait" id="char-portrait" style="background: #a86b43;">
            <div class="hair-crown curls" id="hair-crown" style="background: #18181b;"></div>
            <div class="face-emoji" id="face-emoji">😌</div>
            <div class="outfit-strip" id="outfit-strip" style="background: var(--gold); color: #0b0b0f;">CLEAN GIRL</div>
          </div>
          <div style="flex: 1; min-width: 0;">
            <div style="display: flex; justify-content: space-between; align-items: center;">
              <span style="font-weight: 800; font-size: 0.98rem;" id="display-name">Maya</span>
              <span style="font-size: 0.7rem; color: var(--green); font-weight: 700;" id="display-car">🚶🏽‍♀️ No Car</span>
            </div>
            <div style="font-size: 0.72rem; color: var(--muted); white-space: nowrap; overflow: hidden; text-overflow: ellipsis;" id="display-meta">She/Her • Rich & Chill</div>
            <span class="vibe-pill" id="vibe-pill">✨ Clean Girl & Gold</span>
          </div>
        </div>

        <div class="stats-grid">
          <div class="stat-box">
            <div class="stat-label">🏦 Bank</div>
            <div class="stat-val" id="stat-money" style="color: var(--green);">$2,500</div>
          </div>
          <div class="stat-box">
            <div class="stat-label">⚡ Energy</div>
            <div class="stat-val" id="stat-energy">90%</div>
          </div>
          <div class="stat-box">
            <div class="stat-label">📱 Followers</div>
            <div class="stat-val" id="stat-followers">850</div>
          </div>
          <div class="stat-box">
            <div class="stat-label">✨ Aura</div>
            <div class="stat-val" id="stat-aura">40</div>
          </div>
        </div>
      </div>
    </div>

    <!-- TAB 1: LIFE -->
    <div id="tab-life" class="scroll-area">
      <div id="event-feed"></div>
      <button id="next-btn" style="width: 100%;" onclick="advanceLife()">Advance Life (+6 Months) →</button>
    </div>

    <!-- TAB 2: SOCIAL -->
    <div id="tab-social" class="scroll-area hidden">
      <div class="card">
        <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 8px;">
          <span style="font-weight: 700;">📱 TikTok & X Feed</span>
          <span class="badge" id="social-handle">@maya.era</span>
        </div>
        <div class="btn-stack">
          <button class="secondary" onclick="postSocial('tiktok')">🎵 Post GRWM / Look Check TikTok (+Followers, +Aura)</button>
          <button class="secondary" onclick="postSocial('x_drama')">🐦 Post Sub-Tweet on X (Drama Risk!)</button>
          <button class="secondary" onclick="postSocial('soft_launch')">📸 Post Soft Launch w/ Crush</button>
        </div>
        <div id="social-feed-box"></div>
      </div>

      <div class="card">
        <div style="font-weight: 700; margin-bottom: 8px;">💌 Direct Messages</div>
        <div id="dm-list"></div>
      </div>
    </div>

    <!-- TAB 3: CIRCLE -->
    <div id="tab-circle" class="scroll-area hidden">
      <div class="card">
        <div style="font-weight: 700; margin-bottom: 8px;">❤️ People & Relationships</div>
        <div id="circle-list"></div>
      </div>
    </div>

    <!-- TAB 4: STYLE & BANK (Closet, Hair, Cars, School, Bank) -->
    <div id="tab-hustle" class="scroll-area hidden">
      <div class="card">
        <div style="font-weight: 700; margin-bottom: 6px;">💇🏽‍♀️ Hair & Outfit Switch-Up</div>
        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px;">
          <select id="live-hair-style" onchange="updateLookFromLive()">
            <option value="curls">Big Curls</option>
            <option value="locs">Braids / Locs</option>
            <option value="pixie">Wolf Pixie</option>
            <option value="sleek">Sleek Bob</option>
          </select>
          <select id="live-outfit-style" onchange="updateLookFromLive()">
            <option value="Clean Girl">Clean Girl & Gold</option>
            <option value="Streetwear">Y2K / Streetwear</option>
            <option value="Baddie Night">Late-Night Club Fit</option>
            <option value="Soft Luxury">Soft Luxury Blazer</option>
          </select>
        </div>
      </div>

      <div class="card">
        <div style="font-weight: 700; margin-bottom: 4px;">🎓 School & Work (<span id="major-label">Nursing</span>)</div>
        <p style="font-size: 0.76rem; color: var(--muted); margin-bottom: 8px;" id="career-status">GPA: 3.5 • High School</p>
        <div class="btn-stack">
          <button class="secondary" onclick="doAction('study')">📚 Study & Attend Class (+0.2 GPA, -15 Energy)</button>
          <button class="secondary" onclick="doAction('work')">💼 Work Shift / Gig (+$220, -25 Energy)</button>
          <button class="secondary" onclick="doAction('rest')">😴 Sleep & Recharge (+45 Energy)</button>
        </div>
      </div>

      <div class="card">
        <div style="font-weight: 700; margin-bottom: 4px;">🚘 Cars & Apartments</div>
        <div class="btn-stack">
          <button class="secondary" onclick="buyCar('Used Honda Civic', 2500, 20)">🚗 Used Honda Civic ($2,500 • +20 Aura)</button>
          <button class="secondary" onclick="buyCar('Mercedes C-Class', 8500, 55)">🏎️ Mercedes C-Class ($8,500 • +55 Aura)</button>
          <button class="secondary" onclick="buyCar('G-Wagon', 25000, 120)">🚙 Matte Black G-Wagon ($25,000 • +120 Aura)</button>
          <button class="secondary" onclick="moveOut('shared')">🏢 Move to Shared Apt ($700)</button>
          <button class="secondary" onclick="moveOut('luxury')">🏙️ Move to Penthouse ($3,000)</button>
        </div>
      </div>
    </div>

    <!-- TAB 5: OUTSIDE -->
    <div id="tab-outside" class="scroll-area hidden">
      <div class="card">
        <div style="font-weight: 700; margin-bottom: 4px;">🥂 Outside & Nightlife</div>
        <div class="btn-stack">
          <button class="secondary" onclick="goOutside('club')">🪩 Late-Night Clubbing (-$90, +20 Aura, -30 Energy)</button>
          <button class="secondary" onclick="goOutside('vip')">🍾 VIP Bottle Service (-$400, +50 Aura)</button>
          <button class="secondary" onclick="goOutside('drive')">🌃 Late-Night Drive (Requires Car • +25 Aura)</button>
          <button class="secondary" onclick="goOutside('shop')">🛍️ Outfit Haul (-$160, +25 Aura)</button>
        </div>
      </div>
    </div>

    <nav>
      <button class="nav-btn active" onclick="switchTab('life', this)"><span>✨</span>Life</button>
      <button class="nav-btn" onclick="switchTab('social', this)"><span>📱</span>Social</button>
      <button class="nav-btn" onclick="switchTab('circle', this)"><span>❤️</span>Circle</button>
      <button class="nav-btn" onclick="switchTab('hustle', this)"><span>👗</span>Style/Bank</button>
      <button class="nav-btn" onclick="switchTab('outside', this)"><span>🥂</span>Outside</button>
    </nav>
  </div>
</div>

<script>
  let player = {
    name: "Maya",
    skin: "#a86b43",
    hairStyle: "curls",
    hairColor: "#18181b",
    outfit: "Clean Girl",
    pronouns: "She/Her",
    orientation: "Women",
    wealth: "Rich",
    parentStyle: "Chill",
    major: "Nursing & Medicine",
    age: 17,
    money: 2500,
    energy: 90,
    gpa: 3.5,
    aura: 40,
    followers: 850,
    car: "None",
    housing: "Living w/ Parents",
    schoolStage: "High School",
    graduated: false,
    step: 0,
    circle: [],
    dms: []
  };

  function randomizeSetup() {
    const names = ["Maya", "Zuri", "Kai", "Chloe", "Jade", "Tomi", "Liam", "Aria"];
    const skins = ["#f3c6a5", "#d69e76", "#a86b43", "#5c3822"];
    const hairs = ["curls", "locs", "pixie", "sleek"];
    const colors = ["#18181b", "#7c2d12", "#d97706", "#9d174d"];
    const outfits = ["Clean Girl", "Streetwear", "Baddie Night", "Soft Luxury"];
    const wealthes = ["Rich", "Middle Class", "Struggling"];
    const styles = ["Chill", "Strict"];
    const orients = ["Women", "Men", "Everyone", "Single"];
    const majors = ["Nursing & Medicine", "Business & Finance", "Media & Fashion", "Tech & Software"];

    document.getElementById("char-name").value = names[Math.floor(Math.random() * names.length)];
    document.getElementById("skin-tone").value = skins[Math.floor(Math.random() * skins.length)];
    document.getElementById("hair-style").value = hairs[Math.floor(Math.random() * hairs.length)];
    document.getElementById("hair-color").value = colors[Math.floor(Math.random() * colors.length)];
    document.getElementById("outfit-style").value = outfits[Math.floor(Math.random() * outfits.length)];
    document.getElementById("family-wealth").value = wealthes[Math.floor(Math.random() * wealthes.length)];
    document.getElementById("parent-style").value = styles[Math.floor(Math.random() * styles.length)];
    document.getElementById("char-orientation").value = orients[Math.floor(Math.random() * orients.length)];
    document.getElementById("char-major").value = majors[Math.floor(Math.random() * majors.length)];
  }

  function startGame() {
    player.name = document.getElementById("char-name").value || "Maya";
    player.skin = document.getElementById("skin-tone").value;
    player.hairStyle = document.getElementById("hair-style").value;
    player.hairColor = document.getElementById("hair-color").value;
    player.outfit = document.getElementById("outfit-style").value;
    player.pronouns = document.getElementById("char-pronouns").value;
    player.orientation = document.getElementById("char-orientation").value;
    player.wealth = document.getElementById("family-wealth").value;
    player.parentStyle = document.getElementById("parent-style").value;
    player.major = document.getElementById("char-major").value;

    if (player.wealth === "Rich") { player.money = 2500; player.aura = 40; player.followers = 850; }
    if (player.wealth === "Middle Class") { player.money = 500; player.aura = 20; player.followers = 240; }
    if (player.wealth === "Struggling") { player.money = 90; player.aura = 15; player.followers = 110; }

    let crushName = "Elena";
    if (player.orientation === "Men") crushName = "Marcus";
    if (player.orientation === "Everyone") crushName = "Sasha";
    if (player.orientation === "Single") crushName = "Devon";

    player.circle = [
      { name: "Parents", role: `${player.wealth} & ${player.parentStyle}`, stat: player.parentStyle === "Chill" ? 80 : 50, type: "family" },
      { name: "Zoe", role: "Ride-or-Die Bestie 👯", stat: 85, type: "bestie" },
      { name: "Chloe", role: "Fake Friend 🐍", stat: 40, type: "fake" },
      { name: crushName, role: "Situationship 👀", stat: 55, type: "love" }
    ];

    player.dms = [
      { from: "Zoe (Bestie)", msg: "Are we going out this weekend or locking in for school? 👀", replyA: "We're going OUTSIDE 🪩", replyB: "Locking in on school 📚" },
      { from: `${crushName}`, msg: "Saw your latest post... you look good ngl 😮‍💨", replyA: "Flirt back 💬", replyB: "Leave on seen 😎" }
    ];

    document.getElementById("live-hair-style").value = player.hairStyle;
    document.getElementById("live-outfit-style").value = player.outfit;
    document.getElementById("setup-screen").classList.add("hidden");
    document.getElementById("game-screen").classList.remove("hidden");
    document.getElementById("social-handle").innerText = `@${player.name.toLowerCase()}.era`;
    document.getElementById("major-label").innerText = player.major;

    updateUI();
    renderCircle();
    renderDMs();
    showStoryCard("MAIN CHARACTER ERA", "tag-school", `Welcome, ${player.name}! Rocking ${player.hairStyle} in ${player.outfit} style with ${player.wealth.toLowerCase()} & ${player.parentStyle.toLowerCase()} parents.`);
  }

  function updateLookFromLive() {
    player.hairStyle = document.getElementById("live-hair-style").value;
    player.outfit = document.getElementById("live-outfit-style").value;
    player.aura += 5;
    updateUI();
  }

  function renderPortrait() {
    const portrait = document.getElementById("char-portrait");
    const crown = document.getElementById("hair-crown");
    const strip = document.getElementById("outfit-strip");
    const pill = document.getElementById("vibe-pill");
    const face = document.getElementById("face-emoji");

    portrait.style.background = player.skin;
    crown.className = `hair-crown ${player.hairStyle}`;
    crown.style.background = player.hairColor;

    if (player.energy < 25) face.innerText = "🫠";
    else if (player.aura >= 80) face.innerText = "😎";
    else face.innerText = "😌";

    const outfitMap = {
      "Clean Girl": { label: "CLEAN GIRL", bg: "#fbbf24", fg: "#0b0b0f", pill: "✨ Clean Girl & Gold" },
      "Streetwear": { label: "STREETWEAR", bg: "#38bdf8", fg: "#0b0b0f", pill: "🧢 Y2K & Streetwear" },
      "Baddie Night": { label: "CLUB FIT", bg: "#f472b6", fg: "#0b0b0f", pill: "🪩 Late-Night Club Fit" },
      "Soft Luxury": { label: "SOFT LUXURY", bg: "#c084fc", fg: "#0b0b0f", pill: "🥂 Soft Luxury Blazer" }
    };

    const info = outfitMap[player.outfit] || outfitMap["Clean Girl"];
    strip.innerText = info.label;
    strip.style.background = info.bg;
    strip.style.color = info.fg;
    pill.innerText = info.pill;
  }

  function formatFollowers(n) {
    return n >= 1000 ? (n / 1000).toFixed(1) + "K" : n;
  }

  function updateUI() {
    renderPortrait();
    document.getElementById("age-display").innerText = `Age ${Math.floor(player.age)} • ${player.schoolStage}`;
    document.getElementById("display-name").innerText = player.name;
    document.getElementById("display-meta").innerText = `${player.pronouns} • ${player.wealth} & ${player.parentStyle} • ${player.housing}`;
    document.getElementById("display-car").innerText = player.car === "None" ? "🚶🏽‍♀️ No Car" : `🚘 ${player.car}`;
    document.getElementById("stat-money").innerText = `$${player.money.toLocaleString()}`;
    document.getElementById("stat-energy").innerText = `${Math.min(100, Math.max(0, player.energy))}%`;
    document.getElementById("stat-followers").innerText = formatFollowers(player.followers);
    document.getElementById("stat-aura").innerText = player.aura;
    document.getElementById("career-status").innerText = `GPA: ${player.gpa.toFixed(1)} • ${player.graduated ? "Full-Time " + player.major : player.schoolStage}`;
  }

  function switchTab(tabName, btn) {
    ["life", "social", "circle", "hustle", "outside"].forEach(t => document.getElementById(`tab-${t}`).classList.add("hidden"));
    document.getElementById(`tab-${tabName}`).classList.remove("hidden");
    document.querySelectorAll(".nav-btn").forEach(b => b.classList.remove("active"));
    btn.classList.add("active");
    if (tabName === "circle") renderCircle();
    if (tabName === "social") renderDMs();
  }

  function postSocial(type) {
    const feedBox = document.getElementById("social-feed-box");
    let gain = Math.floor(Math.random() * 400) + 150;
    let html = "";

    if (type === "tiktok") {
      player.followers += gain;
      player.aura += 15;
      html = `
        <div class="post-box">
          <div style="font-weight: 700; color: var(--blue);">🎵 TikTok Posted (+${gain} followers)</div>
          <p style="margin-top: 4px;">"GRWM in my ${player.outfit.toLowerCase()} look ✨"</p>
          <div class="comment-bubble"><b>@zoe.bestie:</b> ATE AND LEFT NO CRUMBS 😍🔥</div>
          <div class="comment-bubble" style="border-color: var(--red);"><b>@chloe_xoxo:</b> Cute! Looks just like what I wore last week 👀</div>
        </div>`;
    } else if (type === "x_drama") {
      player.followers += gain * 2;
      player.aura += 20;
      html = `
        <div class="post-box">
          <div style="font-weight: 700; color: var(--pink);">🐦 Viral Tweet on X (+${gain * 2} followers)</div>
          <p style="margin-top: 4px;">"Some people act like besties in person and pray on downfall in group chats ☕️"</p>
          <div class="comment-bubble" style="border-color: var(--red);"><b>@chloe_xoxo:</b> Why are you always subtweeting??</div>
          <div class="comment-bubble"><b>@campus_tea:</b> Oop—who is this about?! 👀🍿</div>
        </div>`;
    } else if (type === "soft_launch") {
      player.followers += gain;
      player.aura += 18;
      html = `
        <div class="post-box">
          <div style="font-weight: 700; color: var(--accent);">📸 Soft Launch Posted (+${gain} followers)</div>
          <p style="margin-top: 4px;">Late dinner soft launch 🥂❤️</p>
          <div class="comment-bubble"><b>@zoe.bestie:</b> HARD LAUNCH WHEN?! 😭❤️</div>
        </div>`;
    }

    if (player.followers >= 2500) {
      player.money += 250;
      html += `<div class="post-box" style="border-color: var(--green); color: var(--green);">💰 Creator Payout: +$250 added to your Bank!</div>`;
    }

    feedBox.innerHTML = html;
    updateUI();
  }

  function renderDMs() {
    const list = document.getElementById("dm-list");
    if (player.dms.length === 0) {
      list.innerHTML = `<p style="font-size: 0.78rem; color: var(--muted);">No unread DMs right now.</p>`;
      return;
    }
    list.innerHTML = "";
    player.dms.forEach((dm, i) => {
      const div = document.createElement("div");
      div.className = "dm-card";
      div.innerHTML = `
        <div style="font-weight: 700; font-size: 0.82rem; color: var(--accent);">${dm.from}</div>
        <div style="font-size: 0.8rem; margin: 4px 0 8px 0;">"${dm.msg}"</div>
        <div style="display: flex; gap: 6px;">
          <button class="mini-btn secondary" onclick="replyDM(${i}, 'A')">${dm.replyA}</button>
          <button class="mini-btn secondary" onclick="replyDM(${i}, 'B')">${dm.replyB}</button>
        </div>
      `;
      list.appendChild(div);
    });
  }

  function replyDM(idx, choice) {
    const dm = player.dms[idx];
    if (choice === "A") {
      player.aura += 10;
      if (dm.from.includes("Bestie")) player.circle[1].stat = Math.min(100, player.circle[1].stat + 10);
      else player.circle[3].stat = Math.min(100, player.circle[3].stat + 15);
    } else {
      player.aura += 12;
      player.gpa = Math.min(4.0, player.gpa + 0.1);
    }
    player.dms.splice(idx, 1);
    updateUI();
    renderDMs();
  }

  function renderCircle() {
    const list = document.getElementById("circle-list");
    list.innerHTML = "";
    player.circle.forEach((p, idx) => {
      const div = document.createElement("div");
      div.className = "person-card";
      div.innerHTML = `
        <div>
          <div style="font-weight: 700; font-size: 0.88rem;">${p.name}</div>
          <div style="font-size: 0.73rem; color: var(--muted);">${p.role} • Bond: ${p.stat}%</div>
        </div>
        <div style="display: flex; gap: 5px;">
          <button class="mini-btn secondary" onclick="interactPerson(${idx}, 'hang')">Hang Out</button>
          ${p.type === "fake" ? `<button class="mini-btn" style="background: var(--red);" onclick="interactPerson(${idx}, 'cut')">Block</button>` : ""}
        </div>
      `;
      list.appendChild(div);
    });
  }

  function interactPerson(idx, action) {
    const person = player.circle[idx];
    switchTab("life", document.querySelectorAll(".nav-btn")[0]);

    if (action === "cut") {
      player.circle.splice(idx, 1);
      player.aura += 25;
      showStoryCard("BLOCKED & BLESSED", "tag-drama", `You cut off ${person.name}. Peace protected (+25 Aura)!`);
    } else if (person.type === "fake") {
      player.money = Math.max(0, player.money - 50);
      showStoryCard("FAKE FRIEND MOVE", "tag-drama", `${person.name} made you cover $50 at brunch and acted shady.`);
    } else if (person.type === "bestie") {
      person.stat = Math.min(100, person.stat + 10);
      player.energy = Math.min(100, player.energy + 15);
      showStoryCard("BESTIE BOND", "tag-school", `Good vibes with ${person.name} (+15 Energy).`);
    } else if (person.type === "love") {
      person.stat = Math.min(100, person.stat + 15);
      if (person.stat >= 75) person.role = "Official Partner ❤️";
      showStoryCard("ROMANCE", "tag-club", `Hanging out with ${person.name}. Status: ${person.role}!`);
    } else if (person.type === "family") {
      if (player.wealth === "Rich") {
        player.money += 400;
        showStoryCard("ALLOWANCE", "tag-school", `Your parents sent $400 to your bank!`);
      } else {
        person.stat = Math.min(100, person.stat + 10);
        showStoryCard("FAMILY TIME", "tag-school", `Quality time with your parents (+10 Bond).`);
      }
    }
    updateUI();
  }

  function doAction(type) {
    switchTab("life", document.querySelectorAll(".nav-btn")[0]);
    if (type === "study") {
      if (player.energy < 15) return showStoryCard("TOO TIRED", "tag-drama", "Get some sleep before studying!");
      player.gpa = Math.min(4.0, player.gpa + 0.2);
      player.energy -= 15;
      showStoryCard("SCHOOL GRIND", "tag-school", `GPA is now ${player.gpa.toFixed(1)} in ${player.major}.`);
    } else if (type === "work") {
      if (player.energy < 25) return showStoryCard("BURNOUT", "tag-drama", "Rest up before working another shift.");
      let pay = player.graduated ? 650 : 220;
      player.money += pay;
      player.energy -= 25;
      showStoryCard("PAID 🏦", "tag-school", `+$${pay} added to your bank!`);
    } else if (type === "rest") {
      player.energy = Math.min(100, player.energy + 45);
      showStoryCard("RECHARGED", "tag-school", "Energy restored!");
    }
    updateUI();
  }

  function buyCar(carName, price, auraBoost) {
    switchTab("life", document.querySelectorAll(".nav-btn")[0]);
    if (player.money < price) return showStoryCard("NOT ENOUGH CASH", "tag-drama", `Need $${price.toLocaleString()} for the ${carName}.`);
    player.money -= price;
    player.car = carName;
    player.aura += auraBoost;
    player.followers += 500;
    showStoryCard("NEW CAR 🚘", "tag-club", `You bought a ${carName}! (+${auraBoost} Aura, +500 Followers).`);
    updateUI();
  }

  function moveOut(tier) {
    switchTab("life", document.querySelectorAll(".nav-btn")[0]);
    if (player.age < 18) return showStoryCard("TOO YOUNG", "tag-drama", "Turn 18+ first to move out.");
    const cost = tier === "shared" ? 700 : 3000;
    if (player.money < cost) return showStoryCard("INSUFFICIENT FUNDS", "tag-drama", `Need $${cost.toLocaleString()}.`);
    player.money -= cost;
    player.housing = tier === "shared" ? "Shared Apt" : "Penthouse";
    player.aura += tier === "shared" ? 25 : 65;
    showStoryCard("MOVED OUT 🔑", "tag-club", `Welcome to your ${player.housing}!`);
    updateUI();
  }

  function goOutside(spot) {
    switchTab("life", document.querySelectorAll(".nav-btn")[0]);
    if (spot === "drive") {
      if (player.car === "None") return showStoryCard("NO CAR", "tag-drama", "Buy a car in Style/Bank first!");
      player.aura += 25;
      return showStoryCard("NIGHT DRIVE 🌃", "tag-club", `Cruising in your ${player.car} (+25 Aura).`);
    }
    if (spot === "club") {
      if (player.money < 90) return showStoryCard("BROKE ALERT", "tag-drama", "Need $90 for club entry.");
      player.money -= 90;
      player.energy -= 30;
      player.aura += 20;
      player.outfit = "Baddie Night";
      if (player.parentStyle === "Strict" && player.housing === "Living w/ Parents") {
        player.circle[0].stat -= 20;
        showStoryCard("CAUGHT OUT LATE!", "tag-drama", "Strict parents caught you coming home late from the club! (-20 Parent Bond).");
      } else {
        showStoryCard("CLUB NIGHT 🪩", "tag-club", "Switched into your club look and danced all night (+20 Aura)!");
      }
    } else if (spot === "vip") {
      if (player.money < 400) return showStoryCard("BROKE ALERT", "tag-drama", "VIP costs $400.");
      player.money -= 400;
      player.aura += 50;
      player.followers += 400;
      showStoryCard("VIP SECTION 🍾", "tag-club", "Bottle service & main character energy (+50 Aura)!");
    } else if (spot === "shop") {
      if (player.money < 160) return showStoryCard("BROKE ALERT", "tag-drama", "Need $160 to shop.");
      player.money -= 160;
      player.aura += 25;
      showStoryCard("SHOPPING HAUL 🛍️", "tag-club", "Fresh new pieces (+25 Aura).");
    }
    updateUI();
  }

  function showStoryCard(tag, tagClass, text, choices = null) {
    const feed = document.getElementById("event-feed");
    feed.innerHTML = "";
    const card = document.createElement("div");
    card.className = "event-card";
    card.innerHTML = `<span class="tag ${tagClass}">${tag}</span><div>${text}</div>`;

    if (choices) {
      document.getElementById("next-btn").classList.add("hidden");
      const stack = document.createElement("div");
      stack.className = "btn-stack";
      choices.forEach(c => {
        const b = document.createElement("button");
        b.className = "secondary";
        b.innerText = c.label;
        b.onclick = () => {
          c.effect();
          updateUI();
          document.getElementById("next-btn").classList.remove("hidden");
        };
        stack.appendChild(b);
      });
      card.appendChild(stack);
    }
    feed.appendChild(card);
  }

  function advanceLife() {
    player.age += 0.5;
    player.energy = Math.min(100, player.energy + 25);

    if (player.age === 18 && player.schoolStage === "High School") {
      player.schoolStage = "University";
      updateUI();
      return showStoryCard("UNIVERSITY ERA 🎓", "tag-school", `You turned 18 and started ${player.major}! Moving out and buying cars are now unlocked.`, [
        { label: "Join campus social scene (+25 Aura, +400 Followers)", effect: () => { player.aura += 25; player.followers += 400; showStoryCard("CAMPUS BUZZ", "tag-club", "Everyone knows your name already!"); } },
        { label: "Claim merit scholarship (+$800 Bank)", effect: () => { player.money += 800; showStoryCard("SCHOLARSHIP", "tag-school", "+$800 added to your bank!"); } }
      ]);
    }

    if (player.age >= 21 && !player.graduated) {
      player.graduated = true;
      player.schoolStage = "Graduated";
      player.money += 1500;
      updateUI();
      return showStoryCard("GRADUATION 🎓🎉", "tag-school", `Graduated in ${player.major}! Higher pay ($650/shift) + $1,500 bonus unlocked!`);
    }

    const events = [
      {
        tag: "SOCIAL DRAMA", tagClass: "tag-drama",
        text: "Group chat receipts leaked on X, and fake friend Chloe tries to twist the story.",
        choices: [
          { label: "Drop receipts on TikTok (+1,200 Followers, +30 Aura)", effect: () => { player.followers += 1200; player.aura += 30; showStoryCard("VIRAL RECEIPTS", "tag-social", "Everyone saw the truth!"); } },
          { label: "Stay unbothered (+15 Aura, +20 Energy)", effect: () => { player.aura += 15; player.energy += 20; showStoryCard("UNBOTHERED", "tag-school", "You kept your peace."); } }
        ]
      },
      {
        tag: "BRAND DEAL", tagClass: "tag-social",
        text: "A brand offers $600 for a TikTok post right before exams.",
        choices: [
          { label: "Take the $600 (-0.1 GPA)", effect: () => { player.money += 600; player.gpa = Math.max(2.0, player.gpa - 0.1); showStoryCard("SPONSORED", "tag-social", "+$600 in your bank!"); } },
          { label: "Focus on exams (+0.2 GPA)", effect: () => { player.gpa = Math.min(4.0, player.gpa + 0.2); showStoryCard("TOP GRADES", "tag-school", "GPA boosted!"); } }
        ]
      }
    ];

    const ev = events[player.step % events.length];
    player.step++;
    updateUI();
    showStoryCard(ev.tag, ev.tagClass, ev.text, ev.choices);
  }
</script>

</body>
</html>
