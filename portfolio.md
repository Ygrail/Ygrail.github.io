---
layout: page
title: portfolio
subtitle: Research · Projects
permalink: /portfolio/
---

<!--
  각 항목의 설명(pf-project__desc)은 노션 메모에 있던 제목/범위만으로 쓴 요약입니다.
  실제 연구 내용(분석 대상, 사용 기법, 결과)으로 자유롭게 늘려서 교체하세요.
  data-en / data-ko 두 속성 + 안쪽 기본 텍스트, 세 군데를 같이 고치면 됩니다.
-->

<div id="portfolio-content">

<!-- ==================== RESEARCH ==================== -->
<section class="sec" id="research">
  <h2 class="sec__title" data-label="Research">research</h2>

  <!-- ===== VeneerTrace ===== -->
  <div class="pf-project" id="veneertrace">
    <div class="pf-project__header">
      <h3 class="pf-project__name" data-en="VeneerTrace — On-Device Runtime Detection of Inconsistent Android Behavior" data-ko="VeneerTrace — 온디바이스 런타임 안드로이드 이상 행위 탐지">VeneerTrace — On-Device Runtime Detection of Inconsistent Android Behavior</h3>
      <span class="pf-project__period">2025 ~</span>
    </div>
    <p class="pf-project__desc"
       data-en="Runtime analysis work on Android applications whose observable behavior diverges from what they declare. The approach detects that inconsistency on the device itself at runtime, rather than from static artifacts alone. Manuscript <strong>in progress</strong> for IEEE Transactions on Mobile Computing: <em>“Actions Speak Louder Than Words: On-Device Runtime Detection of Inconsistent Android Behavior with VeneerTrace.”</em>"
       data-ko="선언된 동작과 실제로 관측되는 동작이 어긋나는 안드로이드 애플리케이션을 대상으로 한 런타임 분석 연구입니다. 정적 정보에만 의존하지 않고, 기기 위에서 런타임에 그 불일치를 탐지하는 방식을 다룹니다. <strong>IEEE Transactions on Mobile Computing</strong>에 <em>“Actions Speak Louder Than Words: On-Device Runtime Detection of Inconsistent Android Behavior with VeneerTrace”</em> 제목으로 논문 작성 중입니다.">
    Runtime analysis work on Android applications whose observable behavior diverges from what they declare. The approach detects that inconsistency on the device itself at runtime, rather than from static artifacts alone. Manuscript <strong>in progress</strong> for IEEE Transactions on Mobile Computing: <em>“Actions Speak Louder Than Words: On-Device Runtime Detection of Inconsistent Android Behavior with VeneerTrace.”</em>
    </p>
    <div class="pf-project__tags">
      <span class="tag tag--accent">IEEE TMC (in progress)</span>
      <span class="tag">Android</span>
      <span class="tag">Runtime Analysis</span>
      <span class="tag">Behavioral Analysis</span>
      <span class="tag">On-Device</span>
    </div>
  </div>

  <!-- ===== AI Agent manipulation ===== -->
  <div class="pf-project" id="ai-agent">
    <div class="pf-project__header">
      <h3 class="pf-project__name" data-en="Inducing Malfunction in Android AI Agents" data-ko="안드로이드 AI 에이전트 오작동 유도 기법">Inducing Malfunction in Android AI Agents</h3>
      <span class="pf-project__period">2025 ~ 2026</span>
    </div>
    <p class="pf-project__desc"
       data-en="Mobile AI agents drive applications through the same accessibility labels and on-screen visuals that the UI exposes to users. This work looks at what happens when that channel is manipulated — accessibility labels and visual information are altered to steer an agent into acting against the user's intent. Submitted to <strong>CISC-W'26</strong>."
       data-ko="모바일 AI 에이전트는 사용자가 보는 화면과 동일한 접근성 라벨·시각 정보를 근거로 앱을 조작합니다. 이 연구는 그 입력 채널이 조작되었을 때 어떤 일이 벌어지는지를 다룹니다. 접근성 라벨과 시각 정보를 변조해 에이전트가 사용자의 의도와 다르게 동작하도록 유도하는 기법을 정리했으며, <strong>CISC-W'26</strong>에 투고했습니다.">
    Mobile AI agents drive applications through the same accessibility labels and on-screen visuals that the UI exposes to users. This work looks at what happens when that channel is manipulated — accessibility labels and visual information are altered to steer an agent into acting against the user's intent. Submitted to <strong>CISC-W'26</strong>.
    </p>
    <div class="pf-project__tags">
      <span class="tag tag--accent">CISC-W'26 (submitted)</span>
      <span class="tag">AI Agent Security</span>
      <span class="tag">Accessibility Label</span>
      <span class="tag">Mobile AI Agents</span>
      <span class="tag">Agent–Application Interaction</span>
    </div>
  </div>

  <!-- ===== Stacktrace tracing ===== -->
  <div class="pf-project" id="stacktrace">
    <div class="pf-project__header">
      <h3 class="pf-project__name" data-en="Stacktrace Tracing for Multi-threaded Android Applications" data-ko="멀티 스레드 환경 안드로이드 앱 Stacktrace 추적 기법">Stacktrace Tracing for Multi-threaded Android Applications</h3>
      <span class="pf-project__period">2025</span>
    </div>
    <p class="pf-project__desc"
       data-en="Analyzing an Android application gets considerably harder once execution is spread across threads: a call path observed in one thread no longer explains where a behavior actually originated. This work studies stacktrace tracing techniques that keep the call context intact in multi-threaded applications. Published at <strong>CISC-W'25</strong>."
       data-ko="안드로이드 애플리케이션 분석은 실행 흐름이 여러 스레드로 흩어지는 순간 난이도가 크게 올라갑니다. 한 스레드에서 관측한 호출 경로만으로는 그 동작이 실제로 어디에서 비롯됐는지 설명되지 않기 때문입니다. 멀티 스레드 환경에서 호출 컨텍스트를 유지한 채 Stacktrace를 추적하는 기법을 다뤘고, <strong>CISC-W'25</strong>에 게재했습니다.">
    Analyzing an Android application gets considerably harder once execution is spread across threads: a call path observed in one thread no longer explains where a behavior actually originated. This work studies stacktrace tracing techniques that keep the call context intact in multi-threaded applications. Published at <strong>CISC-W'25</strong>.
    </p>
    <div class="pf-project__tags">
      <span class="tag tag--accent">CISC-W'25</span>
      <span class="tag">Android</span>
      <span class="tag">Multi-threading</span>
      <span class="tag">Stacktrace</span>
      <span class="tag">Dynamic Analysis</span>
    </div>
  </div>
</section>

<!-- ==================== PROJECTS ==================== -->
<section class="sec" id="projects">
  <h2 class="sec__title" data-label="Projects">projects</h2>

  <div class="pf-project" id="ms-exchange">
    <div class="pf-project__header">
      <h3 class="pf-project__name" data-en="Microsoft Exchange Server Vulnerability Analysis" data-ko="Microsoft Exchange Server 취약점 분석">Microsoft Exchange Server Vulnerability Analysis</h3>
      <span class="pf-project__period">2026</span>
    </div>
    <p class="pf-project__desc"
       data-en="Vulnerability analysis targeting Microsoft Exchange Server, a mail and collaboration backbone still widely operated on-premise in enterprise environments."
       data-ko="엔터프라이즈 환경에서 여전히 온프레미스로 널리 운영되는 메일·협업 기반 서비스인 Microsoft Exchange Server를 대상으로 한 취약점 분석 프로젝트입니다.">
    Vulnerability analysis targeting Microsoft Exchange Server, a mail and collaboration backbone still widely operated on-premise in enterprise environments.
    </p>
    <div class="pf-project__tags">
      <span class="tag">MS Exchange</span>
      <span class="tag">Enterprise</span>
      <span class="tag">Vulnerability Analysis</span>
    </div>
  </div>
</section>

</div><!-- /portfolio-content -->

<footer class="foot">
  <span>© {{ site.time | date: '%Y' }} Sungbae Yoon</span>
  <span>
    <a href="{{ '/' | prepend: site.baseurl }}">← back to whoami</a>
  </span>
</footer>
