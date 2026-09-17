---
layout: default
title: Sungbae Yoon
---

<!-- ==================== HERO ==================== -->
<div class="hero">
  <div class="term">
    <div class="term__bar">
      <span class="term__dot"></span><span class="term__dot"></span><span class="term__dot"></span>
      <span class="term__bar-title">sbyoon@siftlab — zsh</span>
    </div>
    <div class="term__body">

      <p class="term__line"><span class="term__prompt">$</span> whoami</p>

      <div class="hero__grid">
        <!-- 프로필 사진: assets/img/profile.png 이 있으면 그것을 쓰고,
             없으면 profile-chalice.svg(성배 아이콘)가 대신 보입니다. -->
        <img class="hero__avatar" src="{{ '/assets/img/profile.png' | prepend: site.baseurl }}" alt="Sungbae Yoon"
             onerror="this.onerror=null;this.src='{{ '/assets/img/profile-chalice.svg' | prepend: site.baseurl }}'">
        <div class="hero__main">
          <h1 class="hero__name">Sungbae Yoon <span class="hero__name-ko">윤성배</span></h1>
          <p class="hero__role" data-en="Security Researcher" data-ko="보안 연구자">Security Researcher</p>
          <p class="hero__affil" data-en="Kyung Hee University · SIFTLAB · Advisor: Prof. Jeman Park" data-ko="경희대학교 · SIFTLAB · 지도교수: Prof. Jeman Park">Kyung Hee University · SIFTLAB · Advisor: Prof. Jeman Park</p>
          <div class="hero__links">
            <a class="link-chip" href="https://github.com/Ygrail" target="_blank" rel="noopener"><i class="fa fa-github"></i> GitHub</a>
            <a class="link-chip" href="https://be-a-tist.tistory.com/" target="_blank" rel="noopener"><i class="fa fa-pencil-square-o"></i> Blog</a>
            <a class="link-chip" href="mailto:sbyoon0@naver.com"><i class="fa fa-envelope"></i> sbyoon0@naver.com</a>
          </div>
        </div>
      </div>

      <div class="hero__about">
        <p class="term__line"><span class="term__prompt">$</span> cat about.md</p>
        <p class="term__out"
           data-en="I'm a security researcher who likes understanding systems from the inside out — then validating that understanding through reverse engineering, vulnerability research, and real-world behavior analysis."
           data-ko="시스템을 안에서부터 이해하는 것을 좋아하고, 그렇게 얻은 이해를 리버스 엔지니어링·취약점 연구·실제 동작 분석으로 검증하는 보안 연구자입니다.">I'm a security researcher who likes understanding systems from the inside out — then validating that understanding through reverse engineering, vulnerability research, and real-world behavior analysis.</p>
        <p class="term__out"
           data-en="Recently, I've been focusing on <strong>Android application security</strong> and <strong>behavioral / runtime analysis</strong>, especially security issues that emerge at the intersection of <strong>mobile apps and AI agents</strong>."
           data-ko="최근에는 <strong>안드로이드 애플리케이션 보안</strong>과 <strong>행위·런타임 분석</strong>, 그중에서도 <strong>모바일 앱과 AI 에이전트</strong>가 만나는 지점에서 발생하는 보안 문제에 집중하고 있습니다.">Recently, I've been focusing on <strong>Android application security</strong> and <strong>behavioral / runtime analysis</strong>, especially security issues that emerge at the intersection of <strong>mobile apps and AI agents</strong>.</p>
        <p class="term__line"><span class="term__prompt">$</span><span class="term__cursor"></span></p>
      </div>

    </div>
  </div>
</div>

<!-- ==================== QUICK INFO ==================== -->
<section class="sec" id="quick-info">
  <h2 class="sec__title" data-label="Quick Info">quick_info</h2>

  <div class="kv">
    <div class="kv__row">
      <div class="kv__key" data-en="Affiliation" data-ko="소속">Affiliation</div>
      <div class="kv__val" data-en="Kyung Hee University <span class='dot'>·</span> SIFTLAB" data-ko="경희대학교 <span class='dot'>·</span> SIFTLAB">Kyung Hee University <span class="dot">·</span> SIFTLAB</div>
    </div>
    <div class="kv__row">
      <div class="kv__key" data-en="Interests" data-ko="관심 분야">Interests</div>
      <div class="kv__val" data-en="System Security <span class='dot'>·</span> Mobile Security <span class='dot'>·</span> Program Analysis <span class='dot'>·</span> AI Agent Security" data-ko="시스템 보안 <span class='dot'>·</span> 모바일 보안 <span class='dot'>·</span> 프로그램 분석 <span class='dot'>·</span> AI 에이전트 보안">System Security <span class="dot">·</span> Mobile Security <span class="dot">·</span> Program Analysis <span class="dot">·</span> AI Agent Security</div>
    </div>
    <div class="kv__row">
      <div class="kv__key" data-en="Tooling" data-ko="사용 도구">Tooling</div>
      <div class="kv__val">Linux <span class="dot">·</span> ELF <span class="dot">·</span> GDB <span class="dot">·</span> Frida <span class="dot">·</span> ADB</div>
    </div>
    <div class="kv__row">
      <div class="kv__key" data-en="Languages" data-ko="사용 언어">Languages</div>
      <div class="kv__val">C <span class="dot">·</span> C++ <span class="dot">·</span> Python</div>
    </div>
  </div>
</section>

<!-- ==================== RESEARCH INTERESTS ==================== -->
<section class="sec" id="research-interests">
  <h2 class="sec__title" data-label="Research Interests">research_interests</h2>

  <div class="cards">
    <div class="card">
      <h3 class="card__title" data-en="<i class='fa fa-terminal'></i>System Security" data-ko="<i class='fa fa-terminal'></i>시스템 보안"><i class="fa fa-terminal"></i>System Security</h3>
      <div class="card__tags">
        <span class="tag">Linux</span>
        <span class="tag">Reverse Engineering</span>
        <span class="tag">Vulnerability Analysis</span>
      </div>
    </div>

    <div class="card">
      <h3 class="card__title" data-en="<i class='fa fa-sitemap'></i>Program Analysis" data-ko="<i class='fa fa-sitemap'></i>프로그램 분석"><i class="fa fa-sitemap"></i>Program Analysis</h3>
      <div class="card__tags">
        <span class="tag">Static Analysis</span>
        <span class="tag">Dynamic Analysis</span>
        <span class="tag">Behavioral Analysis</span>
      </div>
    </div>

    <div class="card">
      <h3 class="card__title" data-en="<i class='fa fa-android'></i>Mobile Security" data-ko="<i class='fa fa-android'></i>모바일 보안"><i class="fa fa-android"></i>Mobile Security</h3>
      <div class="card__tags">
        <span class="tag">Android</span>
        <span class="tag">ADB</span>
        <span class="tag">Dynamic Analysis</span>
      </div>
    </div>

    <div class="card">
      <h3 class="card__title" data-en="<i class='fa fa-magic'></i>AI Agent Security" data-ko="<i class='fa fa-magic'></i>AI 에이전트 보안"><i class="fa fa-magic"></i>AI Agent Security</h3>
      <div class="card__tags">
        <span class="tag">Mobile AI Agents</span>
        <span class="tag">AppFunctions</span>
        <span class="tag">Agent–Application Interaction</span>
      </div>
    </div>
  </div>
</section>

<!-- ==================== EDUCATION ==================== -->
<section class="sec" id="education">
  <h2 class="sec__title" data-label="Education">education</h2>

  <div class="tl">
    <div class="tl__item">
      <div class="tl__date">2025 ─ Present</div>
      <div class="tl__body">
        <strong data-en="Kyung Hee University" data-ko="경희대학교">Kyung Hee University</strong>
        <p data-en="M.S. in Convergence Security" data-ko="융합보안학과 석사과정">M.S. in Convergence Security</p>
        <p class="tl__sub" data-en="SIFTLAB · Advisor: Prof. Jeman Park" data-ko="SIFTLAB · 지도교수: Prof. Jeman Park">SIFTLAB · Advisor: Prof. Jeman Park</p>
      </div>
    </div>
    <div class="tl__item">
      <div class="tl__date">2019 ─ 2024</div>
      <div class="tl__body">
        <strong data-en="Kyung Hee University" data-ko="경희대학교">Kyung Hee University</strong>
        <p data-en="B.S. in Computer Engineering" data-ko="컴퓨터공학과 학사">B.S. in Computer Engineering</p>
      </div>
    </div>
  </div>
</section>

<!-- ==================== PUBLICATIONS ==================== -->
<section class="sec" id="publications">
  <h2 class="sec__title" data-label="Publications">publications</h2>

  <h3 class="sub" data-en="In progress / Submitted" data-ko="진행 중 / 투고">In progress / Submitted</h3>

  <div class="entry">
    <div class="entry__text">
      <strong>Actions Speak Louder Than Words: On-Device Runtime Detection of Inconsistent Android Behavior with VeneerTrace</strong>
      <span class="entry__venue">IEEE Transactions on Mobile Computing</span>
    </div>
    <div class="entry__meta"><span class="badge badge--amber" data-en="In Progress" data-ko="진행 중">In Progress</span></div>
  </div>

  <div class="entry">
    <div class="entry__text">
      <strong data-en="Inducing Malfunction in Android AI Agents via Accessibility Label and Visual Information Manipulation" data-ko="접근성 라벨·시각 정보 조작을 통한 안드로이드 AI 에이전트 오작동 유도 기법">Inducing Malfunction in Android AI Agents via Accessibility Label and Visual Information Manipulation</strong>
      <span class="entry__venue">CISC-W'26</span>
    </div>
    <div class="entry__meta"><span class="badge" data-en="Submitted" data-ko="투고">Submitted</span></div>
  </div>

  <h3 class="sub" data-en="Published" data-ko="게재">Published</h3>

  <div class="entry">
    <div class="entry__text">
      <strong data-en="A Study on Stacktrace Tracing Techniques for Analyzing Multi-threaded Android Applications" data-ko="멀티 스레드 환경 안드로이드 어플리케이션 분석을 위한 Stacktrace 추적 기법 연구">A Study on Stacktrace Tracing Techniques for Analyzing Multi-threaded Android Applications</strong>
      <span class="entry__venue">CISC-W'25</span>
    </div>
    <div class="entry__meta"><span class="badge badge--muted">2025</span></div>
  </div>
</section>

<!-- ==================== PROJECTS ==================== -->
<section class="sec" id="projects">
  <h2 class="sec__title" data-label="Projects">projects</h2>

  <div class="tl">
    <div class="tl__item">
      <div class="tl__date">2026</div>
      <div class="tl__body">
        <strong data-en="Microsoft Exchange Server Vulnerability Analysis" data-ko="Microsoft Exchange Server 취약점 분석">Microsoft Exchange Server Vulnerability Analysis</strong>
        <p class="tl__sub"><a href="{{ '/portfolio/#ms-exchange' | prepend: site.baseurl }}" data-en="Details →" data-ko="자세히 →">Details →</a></p>
      </div>
    </div>
  </div>
</section>

<!-- ==================== CTF / ACTIVITIES ==================== -->
<section class="sec" id="activities">
  <h2 class="sec__title" data-label="CTF &amp; Activities">ctf_and_activities</h2>

  <div class="tl">
    <div class="tl__item">
      <div class="tl__date">2025</div>
      <div class="tl__body">
        <strong>HACKHU <span class="badge badge--muted" data-en="KHU Hacking Club" data-ko="경희대학교 해킹동아리">KHU Hacking Club</span></strong>
        <p data-en="System Hacking Education" data-ko="시스템 해킹 교육">System Hacking Education</p>
      </div>
    </div>
    <div class="tl__item">
      <div class="tl__date">2024</div>
      <div class="tl__body">
        <strong data-en="Hacktheon (Beginner)" data-ko="Hacktheon (초급)">Hacktheon (Beginner)</strong>
        <span class="badge" data-en="Finalist" data-ko="본선 진출">Finalist</span>
        <p class="tl__sub" data-en="Team: Neophytes" data-ko="팀: Neophytes">Team: Neophytes</p>
      </div>
    </div>
  </div>
</section>

<!-- ==================== SKILLS ==================== -->
<section class="sec" id="skills">
  <h2 class="sec__title" data-label="Skills">skills</h2>

  <div class="skills__group">
    <div class="skills__label" data-en="Security" data-ko="보안">Security</div>
    <div class="skills__row">
      <span class="skill skill--accent">Linux</span>
      <span class="skill skill--accent">ELF</span>
      <span class="skill skill--accent">GDB</span>
      <span class="skill skill--accent">Frida</span>
      <span class="skill skill--accent">ADB</span>
    </div>
  </div>

  <div class="skills__group">
    <div class="skills__label" data-en="Programming" data-ko="프로그래밍">Programming</div>
    <div class="skills__row">
      <span class="skill">C</span>
      <span class="skill">C++</span>
      <span class="skill">Python</span>
    </div>
  </div>
</section>

<!-- ==================== PERSONAL ==================== -->
<section class="sec" id="personal">
  <h2 class="sec__title" data-label="Personal">personal</h2>

  <div class="note">
    <div class="note__mark">✝</div>
    <div class="note__body">
      <strong data-en="Christian." data-ko="크리스천입니다.">Christian.</strong>
      <p data-en="As a Christian, I want to use what I learn to serve others and contribute to a better world. Through security research, I hope to protect people and the technologies they depend on, and ultimately use my knowledge to help others and make a positive impact on society."
         data-ko="크리스천으로서, 제가 배운 것을 다른 사람을 섬기고 더 나은 세상을 만드는 데 쓰고 싶습니다. 보안 연구를 통해 사람들과 그들이 의지하는 기술을 지키고, 나아가 제 지식으로 다른 사람을 돕고 사회에 긍정적인 영향을 주고 싶습니다.">As a Christian, I want to use what I learn to serve others and contribute to a better world. Through security research, I hope to protect people and the technologies they depend on, and ultimately use my knowledge to help others and make a positive impact on society.</p>
    </div>
  </div>
</section>

<footer class="foot">
  <span>© {{ site.time | date: '%Y' }} Sungbae Yoon</span>
  <span>
    <a href="mailto:sbyoon0@naver.com">sbyoon0@naver.com</a> ·
    <a href="https://github.com/Ygrail" target="_blank" rel="noopener">github.com/Ygrail</a>
  </span>
</footer>
