<!-- README.md (LinkedIn_Testing) — HTML+CSS-in-Markdown | copy–paste this entire block into README.md -->

<!-- ====== Title Card ====== -->
<div align="center" style="font-family: ui-sans-serif, system-ui, 'Segoe UI', Roboto; line-height:1.55; color:#e5e7eb; background:#0b1220; padding:24px; border-radius:16px; border:1px solid #1f2a44;">
  <h1 style="margin:0 0 6px; font-size:34px;">🧪 LinkedIn Testing — Selenium IDE (.side) Suite</h1>
  <p style="margin:0; opacity:.9;">End-to-end scenarios for LinkedIn using Selenium IDE project files</p>
  <p style="margin:12px 0 0 0;">
    <img alt="Suite"  src="https://img.shields.io/badge/Format-.side%20(Selenium%20IDE)-38BDF8" />
    <img alt="Coverage" src="https://img.shields.io/badge/Scenarios-Login%20%7C%20Search%20%7C%20Connect%20%7C%20Group%20ops%20%7C%20Posts-8B5CF6" />
    <img alt="Artifacts" src="https://img.shields.io/badge/Report-PDF%20included-22C55E" />
    <img alt="License" src="https://img.shields.io/badge/License-MIT-10B981" />
  </p>
</div>

<!-- ====== Inline Color Legend ====== -->
<div align="center" style="margin-top:10px; font-size:13px;">
  <b style="color:#FB923C;">📊 Step</b> ·
  <b style="color:#38BDF8;">🎯 Result</b> ·
  <b style="color:#F472B6;">⚡ Decision</b> ·
  <b style="color:#22C55E;">🟩 Success</b> ·
  <b style="color:#F87171;">🟥 Risk</b>
</div>

---

## 📌 Overview

This repository contains **Selenium IDE test projects** for LinkedIn user flows. The suite ships as three `.side` files (Chrome-ready) plus a PDF report. You can **open and run** them directly in the **Selenium IDE browser extension**, or run from CLI using **selenium-side-runner**.

> <b style="color:#22C55E;">🟩 Quick start</b>: Install the Selenium IDE extension → Import `.side` → Play the suite. For headless/CI, see the CLI section below.

---

## 🧭 Table of Contents
- <a href="#-repository-structure">Repository Structure</a>
- <a href="#-scenarios-covered">Scenarios Covered</a>
- <a href="#-run-in-selenium-ide-gui">Run in Selenium IDE (GUI)</a>
- <a href="#-run-from-cli-selenium-side-runner">Run from CLI (selenium-side-runner)</a>
- <a href="#-artifacts--hashes">Artifacts & Hashes</a>
- <a href="#-notes--good-practices">Notes & Good Practices</a>
- <a href="#-license">License</a>

---

## 📂 Repository Structure

```text
|-- 📁 Selenium Automation
|   |-- 📄 Linkedin.side
|   |-- 📄 Linkedin - Sudipta.side
|   |-- 📄 Linkedin - Shuvro.side
|-- 📁 Report
|   |-- 📄 SQT Project LInkedin.pdf
|-- 📄 README.md
|-- 📄 LICENSE
|-- 📄 CITATION.cff
```

<!-- ====== Scenarios Covered (HTML+CSS inline; GitHub-compatible) ====== -->
<!-- Paste this whole block into README.md -->

<section id="-scenarios-covered" style="font-family: ui-sans-serif, system-ui, 'Segoe UI', Roboto; line-height:1.55;">
  <!-- Title -->
  <div style="display:flex; align-items:center; gap:10px; margin:0 0 10px;">
    <span style="display:inline-flex; width:22px; height:22px; border-radius:6px; background:#22C55E; box-shadow: inset 0 0 0 2px rgba(0,0,0,.12);"></span>
    <h2 style="margin:0; font-size:22px; color:#111827;">Scenarios Covered</h2>
  </div>

  <p style="margin:0 0 8px; color:#374151;">The test sets include (non-exhaustive):</p>

  <!-- Authentication -->
  <div class="row">
    <span class="cat">• Authentication:</span>
    <span class="pill">Login_Valid</span>
    <span class="pill">Login Loop</span>
  </div>

  <!-- People & Network -->
  <div class="row">
    <span class="cat">• People &amp; Network:</span>
    <span class="pill">Search People</span>
    <span class="pill">Connection Request Send</span>
    <span class="pill">Connection Request Ignore</span>
    <span class="pill">Follow People</span>
    <span class="pill">Unfollow People</span>
    <span class="pill">Message Send</span>
    <span class="pill">Report a Profile</span>
    <span class="pill">Show About this Profile Option</span>
  </div>

  <!-- Groups -->
  <div class="row">
    <span class="cat">• Groups:</span>
    <span class="pill">Groups Create</span>
    <span class="pill">Group Change Ownerships</span>
    <span class="pill">Group Turn on Automatically member approval</span>
    <span class="pill">Group Turn off Automatic member approval</span>
    <span class="pill">Groups Delete</span>
  </div>

  <!-- Posts & Interactions -->
  <div class="row">
    <span class="cat">• Posts &amp; Interactions:</span>
    <span class="pill">Post in Linkedin</span>
    <span class="pill">Post in Linkedin Loop</span>
    <span class="pill">Comment on a Post</span>
    <span class="pill">Comment Edit</span>
    <span class="pill">Comment Delete</span>
    <span class="pill">React on a Post</span>
    <span class="pill">React Remove</span>
    <span class="pill">Post Edit</span>
    <span class="pill">Post Delete</span>
  </div>

  <!-- Video UX -->
  <div class="row">
    <span class="cat">• Video UX:</span>
    <span class="pill">Video Volume on and off</span>
    <span class="pill">Video Full Screen and small screen</span>
    <span class="pill">Video Show Analytics</span>
  </div>

  <!-- Profile -->
  <div class="row">
    <span class="cat">• Profile:</span>
    <span class="pill">Add a Skill</span>
    <span class="pill">Show Business Options</span>
  </div>

  <!-- Notifications -->
  <div class="row">
    <span class="cat">• Notifications:</span>
    <span class="pill">Notification Delete</span>
  </div>

  #### 🎯 Result
  >  Coverage demonstrates end-to-end user behaviors recruiters care about (auth, engagement, moderation, and admin/group flows).
</section>

<!-- ====== Run in Selenium IDE (GUI) — HTML+CSS inline; GitHub-compatible ====== -->
<!-- Paste this whole block into README.md -->

<section id="-run-in-selenium-ide-gui" style="font-family: ui-sans-serif, system-ui, 'Segoe UI', Roboto; line-height:1.55;">

  <!-- Title Row -->
  <div style="display:flex; align-items:center; gap:10px; margin:0 0 10px;">
    <span style="display:inline-flex; width:18px; height:18px; border-radius:50%; background:#111827; box-shadow: inset 0 0 0 2px rgba(255,255,255,.6);"></span>
    <h2 style="margin:0; font-size:22px; color:#111827;">Run in Selenium IDE (GUI)</h2>
  </div>



  <div class="stepbox">
    1. Install the <b>Selenium IDE</b> browser extension
    <div>
      <span class="label">
      <div class="linkrow">• Chrome: <a href="https://chrome.google.com/webstore/detail/selenium-ide/mooikfkahbdckldjjndioackbalphokd">Web Store</a></div>
      <div class="linkrow">• Firefox: <a href="https://addons.mozilla.org/en-US/firefox/addon/selenium-ide/">Add-ons</a></div>
    </div>
  </div>

  <div class="stepbox">
    2. Open Selenium IDE</span> → <b>Open an existing project</b> → choose one of:<br/>
    <div>
      <span class="label">
      <code>Linkedin.side</code> · <code>Linkedin - Sudipta.side</code> · <code>Linkedin - Shuvro.side</code>
    </div>
  </div>

  <div class="stepbox">
    3. Configure Base URL</span> if prompted (each file already contains a default LinkedIn URL)
    <div>
      <span class="label">
    </div>
  </div>

  <div class="stepbox">
    4. Run</span> Click the <b>Play</b> button to run the whole suite or individual tests.
    <div>
      <span class="label">
    </div>
  </div>

  #### 🟥 Privacy
  >  These flows may require credentials. Use test accounts and avoid recording secrets.
</section>

<!-- Replace your section with this (renders a quote-style block on GitHub) -->
<section id="-run-from-cli-selenium-side-runner" style="font-family: ui-sans-serif, system-ui, 'Segoe UI', Roboto;">
  <h2 style="margin:0 0 8px; font-size:22px; color:#111827;">🧑‍💻 Run from CLI (selenium-side-runner)</h2>
  <blockquote style="
      margin:8px 0 0;
      padding:10px 12px;
      border-left:4px solid #9ca3af;
      background:#f9fafb;
      color:#111827;
      border-radius:6px;
    ">
    CLI is useful for repeatable runs and CI pipelines.
  </blockquote>
</section>


  
  
  ##### Install Node & Runner

  ```bash
  # Node.js 18+ recommended
  node -v
  npm -v

  # Install Selenium IDE runner (requires Chrome/Firefox + drivers on PATH)
  npm install -g selenium-side-runner
  ```

  ##### Run a suite
  ```bash
  # Run the master suite in Chrome
  selenium-side-runner "Linkedin.side" --browser chrome

  # Or a focused suite
  selenium-side-runner "Linkedin - Sudipta.side" --browser chrome
  selenium-side-runner "Linkedin - Shuvro.side"  --browser chrome
  ```   
  ##### Tips for reliability
  ```bash
  # Headless runs (CI)
  selenium-side-runner "Linkedin.side" --browser chrome --headless

  # Slow down for flaky UIs
  selenium-side-runner "Linkedin.side" --browser chrome --output-directory reports --timeout 60000 --delay 200  
  ``` 
  #### 🟩 Success
  > Generated reports (JSON/JUnit) in <code>./reports/</code> can be published in CI.

<!-- ====== Artifacts & Hashes + Notes & Good Practices + License ====== -->
<!-- Paste this whole block into README.md (GitHub-compatible HTML+CSS-in-Markdown) -->

<section id="-artifacts--hashes" style="font-family: ui-sans-serif, system-ui, 'Segoe UI', Roboto; line-height:1.55;">
  <!-- Title -->
  <div style="display:flex; align-items:center; gap:10px; margin:0 0 10px;">
    <span style="display:inline-flex; width:18px; height:18px; border-radius:50%; background:#111827; box-shadow: inset 0 0 0 2px rgba(255,255,255,.6);"></span>
    <h2 style="margin:0; font-size:22px; color:#111827;">Artifacts &amp; Hashes</h2>
  </div>

  <p style="margin:0 0 10px; color:#374151;">For provenance and large-file verification:</p>

  <table align="center" class="tbl">
    <thead>
      <tr>
        <th style="width:48%;">File</th>
        <th style="width:18%; text-align:right;">Size</th>
        <th style="width:34%;">SHA-256 (first 16)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><span class="pill-gray">Linkedin.side</span></td>
        <td style="text-align:right;">114,791 bytes</td>
        <td class="hash">aaf9af40a34693a2</td>
      </tr>
      <tr>
        <td><span class="pill-gray">Linkedin - Sudipta.side</span></td>
        <td style="text-align:right;">74,595 bytes</td>
        <td class="hash">5a1d8589d1e941c</td>
      </tr>
      <tr>
        <td><span class="pill-gray">Linkedin - Shuvro.side</span></td>
        <td style="text-align:right;">40,354 bytes</td>
        <td class="hash">aead257a9daa48e2</td>
      </tr>
      <tr>
        <td><span class="pill-gray">SQT Project LInkedin.pdf</span></td>
        <td style="text-align:right;">13,732,553 bytes</td>
        <td class="hash">09cf7055aae44e30</td>
      </tr>
    </tbody>
  </table>

  #### 🎯 Result
  > Use these hashes to confirm integrity after download or CI artifact moves.
  <hr style="border:none; border-top:1px solid #e5e7eb; margin:18px 0 12px;" />

  <!-- Notes & Good Practices -->
  <div id="-notes--good-practices" style="display:flex; align-items:center; gap:10px; margin:0 0 10px;">
    <span style="display:inline-flex; width:18px; height:18px; border-radius:4px; background:#fde68a; box-shadow: inset 0 0 0 2px rgba(0,0,0,.1);"></span>
    <h2 style="margin:0; font-size:22px; color:#111827;">Notes &amp; Good Practices</h2>
  </div>

  <ul style="margin:0 0 14px 18px; padding:0; color:#111827;">
    <li style="margin:6px 0;">
      <b>Credentials</b>: Store via browser password manager during local GUI runs; for CLI/CI, inject via environment variables and <b>never</b> commit secrets.
    </li>
    <li style="margin:6px 0;">
      <b>Selector stability</b>: Prefer data-test attributes if available; avoid brittle absolute XPaths.
    </li>
    <li style="margin:6px 0;">
      <b>Waits</b>: Replace fixed delays with <code>waitForElementVisible</code>/<code>assert</code> where possible.
    </li>
    <li style="margin:6px 0;">
      <b>Scaling</b>: Consider exporting to Playwright or WebDriver for advanced assertions and parallelization.
    </li>
  </ul>

  <hr style="border:none; border-top:1px solid #e5e7eb; margin:18px 0 12px;" />

  <!-- License -->
  <h2 id="-license" style="margin:0 0 8px; font-size:22px; color:#111827;">📄 License</h2>
  <p style="margin:0;">
    This project is licensed under the <b>MIT License</b> — see <code><a href = "LICENSE">LICENSE</a></code>.
  </p>
</section>

