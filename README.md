[honest-worship-advisor-readme.html](https://github.com/user-attachments/files/29616876/honest-worship-advisor-readme.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>READ ME — Honest Worship Advisor | Ask Marcus</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=Inter:wght@300;400;500;600&family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400&display=swap');

  :root {
    --navy: #0B1F3A;
    --navy-mid: #142849;
    --gold: #C9A84C;
    --gold-light: #E2C47A;
    --cream: #F5EDD8;
    --cream-light: #FAF6EE;
    --text-dark: #0B1F3A;
    --text-mid: #3D5475;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Inter', sans-serif;
    background: var(--cream-light);
    color: var(--text-dark);
    line-height: 1.8;
  }

  /* HEADER */
  .header {
    background: linear-gradient(160deg, #0B1F3A 0%, #142849 100%);
    padding: 70px 40px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }

  .header::before {
    content: '';
    position: absolute;
    top: -80px; left: 50%; transform: translateX(-50%);
    width: 600px; height: 600px;
    background: radial-gradient(circle, rgba(201,168,76,0.08) 0%, transparent 70%);
    pointer-events: none;
  }

  .brand-mark {
    font-family: 'Cormorant Garamond', serif;
    font-size: 11px;
    letter-spacing: 6px;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 20px;
    display: block;
  }

  .header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(36px, 6vw, 64px);
    font-weight: 900;
    color: var(--cream);
    line-height: 1.1;
    margin-bottom: 10px;
  }

  .header h1 span { color: var(--gold); }

  .header-sub {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: clamp(16px, 3vw, 22px);
    color: rgba(245,237,216,0.7);
    margin-bottom: 30px;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
  }

  .scripture-pill {
    display: inline-block;
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 14px;
    color: var(--gold-light);
    background: rgba(201,168,76,0.1);
    border: 1px solid rgba(201,168,76,0.3);
    padding: 10px 24px;
    border-radius: 2px;
  }

  /* CONTENT */
  .container {
    max-width: 820px;
    margin: 0 auto;
    padding: 60px 32px 80px;
  }

  /* SECTIONS */
  .section {
    margin-bottom: 56px;
  }

  .section-label {
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 4px;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 10px;
    display: block;
  }

  .section h2 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(24px, 4vw, 36px);
    font-weight: 700;
    color: var(--navy);
    line-height: 1.2;
    margin-bottom: 8px;
  }

  .gold-rule {
    width: 52px;
    height: 3px;
    background: var(--gold);
    margin: 14px 0 24px;
  }

  .section p {
    font-size: 16px;
    color: var(--text-mid);
    margin-bottom: 16px;
    line-height: 1.85;
  }

  /* PROBLEM CARDS */
  .problem-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
    margin-top: 24px;
  }

  @media (max-width: 560px) { .problem-grid { grid-template-columns: 1fr; } }

  .problem-card {
    background: white;
    border: 1px solid rgba(11,31,58,0.1);
    border-left: 4px solid var(--gold);
    padding: 20px 20px 20px 20px;
    border-radius: 3px;
  }

  .problem-card .icon {
    font-size: 24px;
    margin-bottom: 10px;
    display: block;
  }

  .problem-card h4 {
    font-family: 'Playfair Display', serif;
    font-size: 16px;
    color: var(--navy);
    margin-bottom: 6px;
  }

  .problem-card p {
    font-size: 13px;
    color: var(--text-mid);
    margin: 0;
    line-height: 1.65;
  }

  /* FORGE SECTION */
  .forge-wrap {
    background: var(--navy);
    border-radius: 4px;
    padding: 44px 40px;
    margin-top: 24px;
  }

  .forge-title {
    font-family: 'Playfair Display', serif;
    font-size: 28px;
    color: var(--gold);
    text-align: center;
    margin-bottom: 6px;
  }

  .forge-tagline {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 16px;
    color: rgba(245,237,216,0.65);
    text-align: center;
    margin-bottom: 36px;
  }

  .forge-steps {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }

  .forge-step {
    display: flex;
    gap: 20px;
    align-items: flex-start;
  }

  .forge-letter {
    width: 48px;
    height: 48px;
    background: linear-gradient(135deg, var(--gold), var(--gold-light));
    border-radius: 3px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Playfair Display', serif;
    font-size: 22px;
    font-weight: 900;
    color: var(--navy);
    flex-shrink: 0;
  }

  .forge-step-content h4 {
    font-family: 'Playfair Display', serif;
    font-size: 17px;
    color: var(--cream);
    margin-bottom: 4px;
  }

  .forge-step-content p {
    font-size: 13px;
    color: rgba(245,237,216,0.6);
    margin: 0;
    line-height: 1.6;
  }

  /* CREDIBILITY */
  .cred-box {
    background: white;
    border: 1px solid rgba(11,31,58,0.08);
    border-radius: 4px;
    padding: 36px 36px;
    margin-top: 24px;
    position: relative;
  }

  .cred-box::before {
    content: '"';
    font-family: 'Playfair Display', serif;
    font-size: 100px;
    color: rgba(201,168,76,0.15);
    position: absolute;
    top: -10px;
    left: 24px;
    line-height: 1;
  }

  .cred-box p {
    font-family: 'Cormorant Garamond', serif;
    font-size: 20px;
    font-style: italic;
    color: var(--navy);
    line-height: 1.7;
    margin-bottom: 16px;
    position: relative;
  }

  .cred-attr {
    font-size: 13px;
    font-weight: 600;
    color: var(--gold);
    letter-spacing: 0.5px;
  }

  /* STATS ROW */
  .stats-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin-top: 24px;
  }

  @media (max-width: 560px) { .stats-row { grid-template-columns: 1fr; } }

  .stat-box {
    background: white;
    border: 1px solid rgba(11,31,58,0.08);
    border-radius: 3px;
    padding: 28px 20px;
    text-align: center;
  }

  .stat-box .number {
    font-family: 'Playfair Display', serif;
    font-size: 40px;
    font-weight: 900;
    color: var(--navy);
    line-height: 1;
    margin-bottom: 6px;
  }

  .stat-box .number span { color: var(--gold); }

  .stat-box .label {
    font-size: 12px;
    color: var(--text-mid);
    letter-spacing: 0.3px;
    line-height: 1.5;
  }

  /* PRICING */
  .pricing-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin-top: 24px;
  }

  @media (max-width: 560px) { .pricing-row { grid-template-columns: 1fr; } }

  .price-box {
    border: 1.5px solid rgba(11,31,58,0.12);
    border-radius: 4px;
    padding: 28px 20px;
    text-align: center;
    background: white;
    position: relative;
  }

  .price-box.featured {
    border-color: var(--gold);
    background: rgba(201,168,76,0.04);
  }

  .price-box .badge {
    position: absolute;
    top: -11px; left: 50%; transform: translateX(-50%);
    background: var(--navy);
    color: var(--gold);
    font-size: 9px;
    font-weight: 700;
    letter-spacing: 1.5px;
    padding: 3px 12px;
    border-radius: 2px;
    white-space: nowrap;
  }

  .price-box .plan {
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 1px;
    text-transform: uppercase;
    color: var(--text-mid);
    margin-bottom: 10px;
  }

  .price-box .amount {
    font-family: 'Playfair Display', serif;
    font-size: 34px;
    font-weight: 900;
    color: var(--navy);
    line-height: 1;
    margin-bottom: 4px;
  }

  .price-box .period {
    font-size: 12px;
    color: var(--text-mid);
    margin-bottom: 16px;
  }

  .price-box .perks {
    font-size: 12px;
    color: var(--text-mid);
    line-height: 2;
    list-style: none;
  }

  .price-box .perks li::before {
    content: '✓ ';
    color: var(--gold);
    font-weight: 700;
  }

  /* WHO IT'S FOR */
  .for-list {
    list-style: none;
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }

  .for-list li {
    display: flex;
    align-items: flex-start;
    gap: 14px;
    background: white;
    border: 1px solid rgba(11,31,58,0.08);
    border-radius: 3px;
    padding: 16px 20px;
    font-size: 15px;
    color: var(--text-mid);
    line-height: 1.6;
  }

  .for-list li .check {
    width: 28px;
    height: 28px;
    background: rgba(201,168,76,0.12);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--gold);
    font-size: 13px;
    font-weight: 700;
    flex-shrink: 0;
    margin-top: 2px;
  }

  /* CTA */
  .cta-box {
    background: linear-gradient(135deg, var(--navy) 0%, #142849 100%);
    border-radius: 4px;
    padding: 56px 40px;
    text-align: center;
    margin-top: 24px;
    border: 1px solid rgba(201,168,76,0.2);
  }

  .cta-box h2 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(26px, 4vw, 38px);
    color: var(--cream);
    margin-bottom: 14px;
    line-height: 1.2;
  }

  .cta-box p {
    font-size: 15px;
    color: rgba(245,237,216,0.65);
    max-width: 480px;
    margin: 0 auto 32px;
    line-height: 1.7;
  }

  .cta-scripture {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 15px;
    color: var(--gold-light);
    margin-top: 24px;
  }

  /* FOOTER */
  .footer {
    background: var(--navy);
    text-align: center;
    padding: 32px 20px;
    font-size: 12px;
    color: rgba(245,237,216,0.3);
    border-top: 1px solid rgba(201,168,76,0.1);
  }

  .footer p { margin-bottom: 4px; }

  /* DIVIDER */
  .divider {
    width: 100%;
    height: 1px;
    background: rgba(11,31,58,0.08);
    margin: 56px 0;
  }
</style>
</head>
<body>

<!-- HEADER -->
<div class="header">
  <span class="brand-mark">Honest Worship · Ministry Advisory · RAW Consulting</span>
  <h1>Ask <span>Marcus</span></h1>
  <p class="header-sub">Your 24/7 worship and production ministry advisor — built on faith, experience, and a genuine call to see your ministry thrive</p>
  <div class="scripture-pill">"Iron sharpens iron, as one person sharpens another." — Proverbs 27:17</div>
</div>

<div class="container">

  <!-- WHAT IS THIS -->
  <div class="section">
    <span class="section-label">What Is This</span>
    <h2>Real Answers for Real Ministry Challenges</h2>
    <div class="gold-rule"></div>
    <p>Ask Marcus is a 24/7 worship and production ministry advisor built on over 35 years of combined real-world ministry experience. Whether you are a worship pastor navigating a difficult team, a music director trying to build a culture of excellence, or a production leader who feels unseen and undervalued — this tool was built specifically for you.</p>
    <p>This is not a generic chatbot. Every answer is rooted in Marcus Ford's decades of hands-on ministry experience across multiple states, shaped by the Word of God, and delivered with the pastoral heart of someone who has walked every road you are walking right now. You get honest, Scripture-grounded, no-fluff answers to the questions you are afraid to ask anyone else.</p>
    <p>Available any time of day or night. No appointment needed. No judgment. Just wisdom when you need it most.</p>
  </div>

  <!-- PROBLEMS WE SOLVE -->
  <div class="section">
    <span class="section-label">The Problems We Solve</span>
    <h2>If You Are Facing Any of These, You Are in the Right Place</h2>
    <div class="gold-rule"></div>
    <p>Ministry leadership is one of the most rewarding and most challenging callings on the planet. These are the real issues worship and production leaders bring to Marcus every day.</p>

    <div class="problem-grid">
      <div class="problem-card">
        <span class="icon">🎵</span>
        <h4>Team Conflict and Culture Problems</h4>
        <p>Musicians who won't submit to leadership. Tension between the worship team and production team. Cliques, attitudes, and power struggles that drain the life out of your ministry.</p>
      </div>
      <div class="problem-card">
        <span class="icon">🎚️</span>
        <h4>Production and Technical Challenges</h4>
        <p>Audio issues that never get resolved. Production teams that feel disconnected from the worship team's vision. Leaders who don't know how to bridge the gap between sound and spirit.</p>
      </div>
      <div class="problem-card">
        <span class="icon">🙏</span>
        <h4>Spiritual Drift in Your Ministry</h4>
        <p>Musicians who are talented but not discipled. A team that performs on Sunday but has no spiritual depth Monday through Saturday. Worship that looks good but lacks the presence of God.</p>
      </div>
      <div class="problem-card">
        <span class="icon">👑</span>
        <h4>Leadership That Doesn't Value You</h4>
        <p>Pastors who treat worship ministry as a support act rather than a Kingdom priority. Being overlooked in leadership meetings. Fighting for budget, respect, and a seat at the table.</p>
      </div>
      <div class="problem-card">
        <span class="icon">🔥</span>
        <h4>Burnout and Ministry Exhaustion</h4>
        <p>Giving everything you have on Sunday while running on empty the rest of the week. No boundaries, no rest, and no one around who truly understands what you carry.</p>
      </div>
      <div class="problem-card">
        <span class="icon">📋</span>
        <h4>No Training or Development System</h4>
        <p>New team members with no clear path to grow. No rehearsal culture. No way to develop leaders from within. Everything depending on you and falling apart when you are not there.</p>
      </div>
      <div class="problem-card">
        <span class="icon">⏰</span>
        <h4>Accountability and Consistency Issues</h4>
        <p>Team members who show up late, unprepared, or not at all. No culture of excellence or commitment. Standards that exist on paper but never in practice.</p>
      </div>
      <div class="problem-card">
        <span class="icon">🏛️</span>
        <h4>Building Ministry From the Ground Up</h4>
        <p>Starting a worship department with no blueprint. Trying to build structure, culture, and excellence simultaneously with limited resources and even less support.</p>
      </div>
    </div>
  </div>

  <!-- FORGE FRAMEWORK -->
  <div class="section">
    <span class="section-label">Our Framework</span>
    <h2>Built on the F.O.R.G.E. Framework</h2>
    <div class="gold-rule"></div>
    <p>Every answer Marcus gives is shaped by the F.O.R.G.E. framework — a proven leadership development system designed to forge worship and production leaders who lead like Jesus. This is not theory. This is the same framework Marcus has used to develop leaders across the country for decades.</p>

    <div class="forge-wrap">
      <div class="forge-title">F.O.R.G.E.</div>
      <div class="forge-tagline">Forging leaders who lead like Jesus</div>
      <div class="forge-steps">
        <div class="forge-step">
          <div class="forge-letter">F</div>
          <div class="forge-step-content">
            <h4>Form — Develop Christlike Character</h4>
            <p>True ministry leadership starts from the inside out. Before you can lead others, God must shape you. We help leaders identify and address the character gaps that are limiting their ministry effectiveness.</p>
          </div>
        </div>
        <div class="forge-step">
          <div class="forge-letter">O</div>
          <div class="forge-step-content">
            <h4>Observe — Learn Through Example and Modeling</h4>
            <p>Great leaders are first great learners. We connect you to the models, examples, and principles that show you what healthy worship and production ministry actually looks like in practice.</p>
          </div>
        </div>
        <div class="forge-step">
          <div class="forge-letter">R</div>
          <div class="forge-step-content">
            <h4>Refine — Strengthen Skills and Discipline</h4>
            <p>Excellence in ministry requires both spiritual depth and practical skill. We help you sharpen the specific leadership, relational, and technical skills your role demands.</p>
          </div>
        </div>
        <div class="forge-step">
          <div class="forge-letter">G</div>
          <div class="forge-step-content">
            <h4>Grow — Expand Leadership Influence</h4>
            <p>Your impact should grow beyond your immediate team. We help you develop the influence, vision, and strategy to build a ministry that outlasts any single Sunday service.</p>
          </div>
        </div>
        <div class="forge-step">
          <div class="forge-letter">E</div>
          <div class="forge-step-content">
            <h4>Empower — Release Others Into Ministry</h4>
            <p>The ultimate goal of leadership is to make yourself unnecessary. We help you build a culture where others are developed, released, and trusted to carry the ministry forward.</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- WHO IS MARCUS -->
  <div class="section">
    <span class="section-label">Who Is Marcus</span>
    <h2>Experience You Can Trust. Faith You Can Feel.</h2>
    <div class="gold-rule"></div>
    <p>Marcus Ford is the co-founder of Honest Worship and RAW Consulting, a ministry consulting and training organization built to serve worship and production leaders at every level. With over 35 years of combined ministry experience across multiple states, Marcus has served as a worship leader, music director, production director, ministry consultant, church audio system designer, and leadership trainer.</p>
    <p>Marcus and his partner Sharon Ford have walked alongside hundreds of worship and production ministry leaders — helping them navigate conflict, build culture, develop teams, and rediscover the joy of their calling. His approach is always pastoral, always Scripture-grounded, and always rooted in the belief that God has more for your ministry than you have experienced so far.</p>
    <p>This is not someone who read about ministry from the outside. Marcus has been in the room. He has sat with the frustrated worship pastor, the overlooked production director, the burned-out musician, and the first-time ministry leader who had no idea where to start. He has seen what breaks ministries down and what builds them back up — and he has built this tool to bring that wisdom directly to you.</p>

    <div class="cred-box">
      <p>Marcus brings a level of wisdom, clarity, and pastoral care to worship ministry leadership that I have rarely seen. His guidance helped our team move from constant conflict to genuine unity. He does not just give you answers — he helps you become the leader your ministry needs.</p>
      <span class="cred-attr">— Tye Maner, Executive Pastor · Love First Christian Center</span>
    </div>

    <div class="stats-row" style="margin-top:20px;">
      <div class="stat-box">
        <div class="number">35<span>+</span></div>
        <div class="label">Years of Combined Ministry Experience</div>
      </div>
      <div class="stat-box">
        <div class="number">24<span>/7</span></div>
        <div class="label">Available Any Time You Need Answers</div>
      </div>
      <div class="stat-box">
        <div class="number">100<span>%</span></div>
        <div class="label">Rooted in Scripture and Real Ministry Practice</div>
      </div>
    </div>
  </div>

  <!-- WHO IT'S FOR -->
  <div class="section">
    <span class="section-label">Who This Is For</span>
    <h2>This Was Built for You If You Are...</h2>
    <div class="gold-rule"></div>

    <ul class="for-list">
      <li>
        <span class="check">✓</span>
        A worship pastor or director carrying the weight of your ministry alone and needing someone who truly understands what you face
      </li>
      <li>
        <span class="check">✓</span>
        A music director trying to build a culture of excellence and discipleship on a team that has never been trained to think that way
      </li>
      <li>
        <span class="check">✓</span>
        A production or audio director who feels invisible, undervalued, and unsure how to bridge the gap between technical excellence and spiritual purpose
      </li>
      <li>
        <span class="check">✓</span>
        A worship team member who senses a call to lead but has no one to show you how
      </li>
      <li>
        <span class="check">✓</span>
        A senior pastor or church leader who wants to understand how to support, develop, and properly resource your worship and production ministry
      </li>
      <li>
        <span class="check">✓</span>
        A church planter or new ministry leader trying to build a worship department from scratch with limited experience and limited resources
      </li>
      <li>
        <span class="check">✓</span>
        Anyone in worship or production ministry who is tired of searching the internet for answers that were never written for someone in your specific situation
      </li>
    </ul>
  </div>

  <!-- PRICING -->
  <div class="section">
    <span class="section-label">Access Options</span>
    <h2>Start Free. Upgrade When You Are Ready.</h2>
    <div class="gold-rule"></div>
    <p>Your first 3 questions are completely free. No credit card required. No strings attached. Experience the wisdom for yourself, then choose the plan that fits where you are.</p>

    <div class="pricing-row" style="grid-template-columns: repeat(2, 1fr);">
      <div class="price-box">
        <div class="plan">Free Trial</div>
        <div class="amount">$0</div>
        <div class="period">3 questions</div>
        <ul class="perks">
          <li>3 ministry questions</li>
          <li>Honest answers</li>
          <li>Scripture references</li>
        </ul>
      </div>
      <div class="price-box featured">
        <div class="badge">MOST POPULAR</div>
        <div class="plan">Monthly Access</div>
        <div class="amount">$29</div>
        <div class="period">per month</div>
        <ul class="perks">
          <li>Unlimited questions</li>
          <li>Priority responses</li>
          <li>F.O.R.G.E. framework</li>
          <li>Ministry resource library</li>
        </ul>
      </div>
      <div class="price-box">
        <div class="badge">SAVE 40%</div>
        <div class="plan">Annual Access</div>
        <div class="amount">$197</div>
        <div class="period">per year</div>
        <ul class="perks">
          <li>Everything in Monthly</li>
          <li>Coaching calls via Zoom</li>
          <li>Master Class Intensive discount</li>
        </ul>
      </div>
      <div class="price-box">
        <div class="plan">Church Team</div>
        <div class="amount">$97</div>
        <div class="period">per month</div>
        <ul class="perks">
          <li>Up to 10 team members</li>
          <li>Ministry assessment included</li>
          <li>Bulk learning resources</li>
        </ul>
      </div>
    </div>
  </div>

  <!-- CTA -->
  <div class="cta-box">
    <h2>Your Ministry Deserves More Than Guesswork</h2>
    <p>God did not call you to figure this out alone. He placed people in your path to sharpen you, strengthen you, and help you lead with greater clarity, confidence, and Kingdom impact.</p>
    <p style="color:rgba(245,237,216,0.65); font-size:15px; margin-top:12px;">Start with 3 free questions. No credit card. No pressure. Just honest answers from someone who has walked the road you are on.</p>
    <div class="cta-scripture">"Iron sharpens iron, as one person sharpens another." — Proverbs 27:17</div>
  </div>

</div>

<!-- FOOTER -->
<div class="footer">
  <p>© 2024 Honest Worship · RAW Consulting · info@rawconsulting.co</p>
  <p>Built on the F.O.R.G.E. Framework · Forging leaders who lead like Jesus</p>
</div>

</body>
</html>
