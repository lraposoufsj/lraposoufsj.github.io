---
layout: page
permalink: /Teaching/
title: Teaching
description: Course materials for current and previous students
nav: true
nav_order: 2
---

<style>
.teaching-wrap { padding: 0.5rem 0 3rem; }

/* ── search & filters ── */
.search-row {
  display: flex;
  gap: 8px;
  margin-bottom: 2rem;
  flex-wrap: wrap;
}
.search-row input {
  flex: 1;
  min-width: 200px;
  padding: 8px 14px;
  font-size: 14px;
  border: 0.5px solid var(--global-divider-color);
  border-radius: 8px;
  background: var(--global-bg-color);
  color: var(--global-text-color);
  outline: none;
  font-family: inherit;
}
.search-row input:focus {
  border-color: var(--global-theme-color);
}
.filter-btn {
  padding: 7px 14px;
  font-size: 13px;
  border: 0.5px solid var(--global-divider-color);
  border-radius: 8px;
  background: var(--global-bg-color);
  color: var(--global-text-color-light);
  cursor: pointer;
  font-family: inherit;
  transition: all 0.15s;
}
.filter-btn:hover { border-color: var(--global-theme-color); color: var(--global-theme-color); }
.filter-btn.active {
  background: var(--global-theme-color);
  border-color: var(--global-theme-color);
  color: #fff;
  font-weight: 500;
}

/* ── section labels ── */
.section-label {
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.09em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  margin-bottom: 1rem;
}

/* ── grid ── */
.course-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(290px, 1fr));
  gap: 12px;
  margin-bottom: 2rem;
}

/* ── cards ── */
.course-card {
  background: var(--global-bg-color);
  border: 0.5px solid var(--global-divider-color);
  border-radius: 12px;
  padding: 1.1rem 1.25rem;
  transition: border-color 0.15s;
}
.course-card:hover { border-color: var(--global-theme-color); }
.course-card.current { border-color: var(--global-theme-color); border-width: 1px; }
.course-card.hidden { display: none; }

.card-top {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 0.5rem;
  gap: 8px;
}
.course-code {
  font-size: 11px;
  font-weight: 600;
  color: var(--global-theme-color);
  background: color-mix(in srgb, var(--global-theme-color) 12%, transparent);
  padding: 2px 8px;
  border-radius: 6px;
  white-space: nowrap;
}
.sem-badge {
  font-size: 11px;
  color: var(--global-text-color-light);
  white-space: nowrap;
  padding-top: 2px;
}
.course-title {
  font-size: 14px;
  font-weight: 600;
  color: var(--global-text-color);
  line-height: 1.4;
  margin-bottom: 2px;
}
.course-meta {
  font-size: 12px;
  color: var(--global-text-color-light);
  margin-bottom: 1rem;
}

/* ── material chips ── */
.mat-group { margin-bottom: 0.6rem; }
.mat-group-label {
  font-size: 10px;
  text-transform: uppercase;
  letter-spacing: 0.07em;
  color: var(--global-text-color-light);
  margin-bottom: 4px;
}
.mat-chips { display: flex; flex-wrap: wrap; gap: 5px; }
.mat-chip {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-size: 12px;
  padding: 3px 10px;
  border: 0.5px solid var(--global-divider-color);
  border-radius: 6px;
  color: var(--global-text-color);
  background: var(--global-card-bg-color, var(--global-bg-color));
  text-decoration: none;
  transition: all 0.15s;
}
.mat-chip:hover {
  border-color: var(--global-theme-color);
  color: var(--global-theme-color);
  text-decoration: none;
}
.mat-chip.soon {
  opacity: 0.38;
  pointer-events: none;
}
.chip-icon { font-size: 11px; }

.section-divider {
  border: none;
  border-top: 0.5px solid var(--global-divider-color);
  margin: 0.5rem 0 1.75rem;
}

.no-results {
  display: none;
  color: var(--global-text-color-light);
  font-size: 14px;
  padding: 2rem 0;
}
</style>

<div class="teaching-wrap">

  <!-- Search & filter bar -->
  <div class="search-row">
    <input type="text" id="course-search" placeholder="Search by course name, code, or topic…" oninput="filterCourses()" />
    <button class="filter-btn active" onclick="setFilter('all', this)">All</button>
    <button class="filter-btn" onclick="setFilter('ufsj', this)">UFSJ</button>
    <button class="filter-btn" onclick="setFilter('unifei', this)">UNIFEI</button>
  </div>

  <!-- Current semester -->
  <p class="section-label" id="label-current">Current semester — UFSJ 2026/1</p>
  <div class="course-grid" id="grid-current">

    <!-- O Chem for Bio -->
    <div class="course-card current" data-inst="ufsj" data-keywords="organic chemistry biology bonding stereochemistry conjugation conformation intermolecular qob CB00615546 2026 2026/1">
      <div class="card-top">
        <span class="course-code">CB00615546</span>
        <span class="sem-badge">UFSJ 2026/1</span>
      </div>
      <div class="course-title">Organic Chemistry for Biological Sciences</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/QOB_20261_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture notes</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_m1_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Chemical Bonding</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_m2_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Intermolecular Forces</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_m3_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — Conjugation</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_m4_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Nomenclature and Organic Functions</a>
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 5 — Conformational Analysis and Projections</a>
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 6 — Stereochemistry</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 — Parts 1 and 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qob_20261_test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2 — Parts 3 and 4</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Test 3 — Parts 5 and 6</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- Gen Chem for Bio -->
    <div class="course-card current" data-inst="ufsj" data-keywords="general chemistry biology bonding inorganic nomenclature solution equilibrium acids bases pH qgb CB00515545 2026 2026/1">
      <div class="card-top">
        <span class="course-code">CB00515545</span>
        <span class="sem-badge">UFSJ 2026/1</span>
      </div>
      <div class="course-title">General Chemistry for Biological Sciences</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/QGB_20261_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture notes</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_m1_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Chemical Bonding</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_m2_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Inorganic Functions</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_m3_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — Solution Chemistry</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_m4_notes.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Chemical Equilibrium</a>
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 5 — Acids, bases, and pH</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 — Parts 1 and 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qgb_20261_test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2 — Part 3</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Test 3 — Parts 4 and 5</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- OChem 3 -->
    <div class="course-card current" data-inst="ufsj" data-keywords="physical methods organic chemistry spectroscopy nmr ir ms qo3 QU02419742 2026 2026/1">
      <div class="card-top">
        <span class="course-code">QU02419742</span>
        <span class="sem-badge">UFSJ 2026/1</span>
      </div>
      <div class="course-title">Organic Chemistry III</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/ORG3_20261_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture notes</div>
        <div class="mat-chips">
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 1 — UV Spectroscopy</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/QO3_20261_Slides_M2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Infrared Spectroscopy</a>
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 3 — NMR Spectroscopy</a>
          <a class="mat-chip soon"><span class="chip-icon">📊</span> Part 4 — Mass Spectrometry</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qo3_20261_test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 — Parts 1 and 2</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Test 2 — Parts 1 to 3</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Test 3 — Parts 1 to 4</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- Gen Chem Exp 1 -->
    <div class="course-card current" data-inst="ufsj" data-keywords="general chemistry laboratory experimental glassware report scientific density calibration flame evidence reaction chemical melting point napththalene alcohol gasoline mixture separation salt synthesis formula hydrated determination qexp1 QU00519628 2026 2026/1">
      <div class="card-top">
        <span class="course-code">QU00519628 </span>
        <span class="sem-badge">UFSJ 2026/1</span>
      </div>
      <div class="course-title">Experimental General Chemistry I</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/QGE1_20261_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/QGE1_2026_1_Exp.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2026-1/qe1_20261_test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip soon"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

  </div>

  <hr class="section-divider" />

  <!-- Previous courses -->
  <p class="section-label" id="label-previous">Previous courses</p>
  <div class="course-grid" id="grid-previous">

    <!-- Physical Methods -->
    <div class="course-card" data-inst="ufsj" data-keywords="physical methods organic chemistry spectroscopy nmr ir ms mfqo qu03319694 2025 2025/2">
      <div class="card-top">
        <span class="course-code">QU03319694</span>
        <span class="sem-badge">UFSJ 2025/2</span>
      </div>
      <div class="course-title">Physical Methods in Organic Chemistry</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture slides</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Slides_Mod1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Mass Spectrometry</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Slides_Mod2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Infrared Spectroscopy</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Slides_Mod3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — NMR Spectroscopy</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 — MS</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2 — MS and IR</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_TestSub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- Intro Organic Lab -->
    <div class="course-card" data-inst="ufsj" data-keywords="introduction organic chemistry laboratory experimental ilqo qu03419695 2025 2025/2">
      <div class="card-top">
        <span class="course-code">QU03419695</span>
        <span class="sem-badge">UFSJ 2025/2</span>
      </div>
      <div class="course-title">Introduction to the Organic Chemistry Laboratory</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Exps.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_TestSub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- Experimental Biochemistry -->
    <div class="course-card" data-inst="ufsj" data-keywords="experimental biochemistry bqe qu03819740 starch dna sds-page 2025 2025/2">
      <div class="card-top">
        <span class="course-code">QU03819740</span>
        <span class="sem-badge">UFSJ 2025/2</span>
      </div>
      <div class="course-title">Experimental Biochemistry</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/BQE_8P_20252_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/BQE_Apostila_v2024.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/BQE_20252_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/BQE_20252_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1a</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/BQE_20252_Test3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
        </div>
      </div>
    </div>

    <!-- General Chemistry for Engineering -->
    <div class="course-card" data-inst="ufsj" data-keywords="general chemistry engineering cna0001 stoichiometry thermochemistry equilibrium kinetics electrochemistry 2025 2025/2">
      <div class="card-top">
        <span class="course-code">CNA0001</span>
        <span class="sem-badge">UFSJ 2025/2</span>
      </div>
      <div class="course-title">General Chemistry for Engineering</div>
      <div class="course-meta">Assistant Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture slides</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Slides_Mod5.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Chemical Reactions and Stoichiometry</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Slides_Mod6.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Thermochemistry</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Slides_Mod7.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — Chemical Kinetics</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Slides_Mod8.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Chemical Equilibrium</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Slides_Mod9.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 5 — Electrochemistry</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Test3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 (3)</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_Test4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2 (4)</a>
          <a class="mat-chip" href="{{ '/assets/pdf/ufsj/2025-2/QG_20252_TestSub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- QUI070 Physical Methods UNIFEI 2025/1 -->
    <div class="course-card" data-inst="unifei" data-keywords="physical methods analysis spectroscopy uv-vis ir nmr ms qui070 unifei 2025 2025/1">
      <div class="card-top">
        <span class="course-code">QUI070</span>
        <span class="sem-badge">UNIFEI 2025/1</span>
      </div>
      <div class="course-title">Physical Methods for Analysis</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture slides</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Lecture_Notes_M1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — UV-Vis</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — IR</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3A — NMR intro</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3B — ¹H NMR</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3C — ¹³C NMR</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3D — J coupling & 2D NMR</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Mass Spectrometry</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 3</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test_Sub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Exercises</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Solved_ex_M3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">✏️</span> Solved NMR exercises</a>
        </div>
      </div>
    </div>

    <!-- QUI016 General Chemistry UNIFEI 2025/1 -->
    <div class="course-card" data-inst="unifei" data-keywords="general chemistry qui016 unifei 2025 atomic bonds gases solutions thermodynamics kinetics electrochemistry 2025/1">
      <div class="card-top">
        <span class="course-code">QUI016</span>
        <span class="sem-badge">UNIFEI 2025/1</span>
      </div>
      <div class="course-title">General Chemistry</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_ShortTest1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Short Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_ShortTest2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Short Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test_Sub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
    </div>

    <!-- QUI017 Experimental General Chemistry UNIFEI 2025/1 -->
    <div class="course-card" data-inst="unifei" data-keywords="experimental general chemistry qui017 unifei 2025 stoichiometry kinetics equilibrium electrochemistry 2025/1">
      <div class="card-top">
        <span class="course-code">QUI017</span>
        <span class="sem-badge">UNIFEI 2025/1</span>
      </div>
      <div class="course-title">Experimental General Chemistry</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Exp_prot.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
        </div>
      </div>
    </div>

    <!-- QUI212 Experimental General Chemistry UNIFEI 2025/1 -->
    <div class="course-card" data-inst="unifei" data-keywords="experimental general chemistry engineering qui212 unifei 2025 equilibrium thermodynamics electrochemistry 2025/1">
      <div class="card-top">
        <span class="course-code">QUI212</span>
        <span class="sem-badge">UNIFEI 2025/1</span>
      </div>
      <div class="course-title">Experimental General Chemistry (Engineering)</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
        </div>
      </div>
    </div>

    <!-- QUI055 Organic Chemistry II UNIFEI 2024/4 summer -->
    <div class="course-card" data-inst="unifei" data-keywords="organic chemistry ii qui055 unifei 2024 summer alkenes alkynes aromatic alcohols ethers organometallic 2024/4">
      <div class="card-top">
        <span class="course-code">QUI055</span>
        <span class="sem-badge">UNIFEI 2024/4 (Summer)</span>
      </div>
      <div class="course-title">Organic Chemistry II</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture slides</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Alkenes & alkynes</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Alkene additions</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — Conjugated alkenes</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Aromatic compounds</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M5.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 5 — Alcohols & ethers</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M6.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 6 — Oxidations, reductions & RLi/RMgX</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 3</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 4</a>
        </div>
      </div>
    </div>

    <!-- QUI022 Organic Chemistry UNIFEI 2024/2 -->
    <div class="course-card" data-inst="unifei" data-keywords="organic chemistry qui022 unifei 2024 acids bases conjugation aromatic substitution carbonyl 2024/4">
      <div class="card-top">
        <span class="course-code">QUI022</span>
        <span class="sem-badge">UNIFEI 2024/2</span>
      </div>
      <div class="course-title">Organic Chemistry</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Lecture notes</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 1 — Representation & bond theory</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 2 — Inductive & mesomeric effects</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 3 — Functional groups</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M4.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 4 — Nomenclature</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M5.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 5 — Physical & chemical properties</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M6.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 6 — Acids & bases</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M7.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 7 — Stereochemistry</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M8.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 8 — Radical reactions</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M9.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 9 — Alkene addition reactions</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M10.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 10 — Electrophilic aromatic substitution</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M11.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📊</span> Part 11 — Carbonyl substitution & addition</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Short Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Short Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Short Test 3</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test3.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 3</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_TestSub.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Substitute Test</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Exercises</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_List1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">✏️</span> Exercise List 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_List2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">✏️</span> Exercise List 2</a>
        </div>
      </div>
    </div>

    <!-- QUI068 Experimental Organic Chemistry UNIFEI 2024/2 -->
    <div class="course-card" data-inst="unifei" data-keywords="experimental organic chemistry qui068 unifei 2024 extraction chromatography tlc asa recrystallization">
      <div class="card-top 2024/2">
        <span class="course-code">QUI068</span>
        <span class="sem-badge">UNIFEI 2024/2</span>
      </div>
      <div class="course-title">Experimental Organic Chemistry</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Exp_Prot.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
        </div>
      </div>
    </div>

    <!-- QUI113 Experimental Chemistry UNIFEI 2024/2 -->
    <div class="course-card" data-inst="unifei" data-keywords="experimental chemistry qui113 unifei 2024 stoichiometry standardization kinetics equilibrium biology physics bioprocess 2024/2">
      <div class="card-top">
        <span class="course-code">QUI113</span>
        <span class="sem-badge">UNIFEI 2024/2</span>
      </div>
      <div class="course-title">Experimental Chemistry</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Exp_Prot.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
        </div>
      </div>
    </div>

    <!-- QUI212 Experimental General Chemistry UNIFEI 2024/2 -->
    <div class="course-card" data-inst="unifei" data-keywords="experimental general chemistry engineering qui212 unifei 2024 equilibrium thermodynamics electrochemistry 2024/2">
      <div class="card-top">
        <span class="course-code">QUI212</span>
        <span class="sem-badge">UNIFEI 2024/2</span>
      </div>
      <div class="course-title">Experimental General Chemistry (Engineering)</div>
      <div class="course-meta">Substitute Professor</div>
      <div class="mat-group">
        <div class="mat-group-label">Documents</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Syllabus.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📄</span> Syllabus</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Exp_Prot.pdf' | relative_url }}" target="_blank"><span class="chip-icon">🧪</span> Experiments</a>
        </div>
      </div>
      <div class="mat-group">
        <div class="mat-group-label">Tests</div>
        <div class="mat-chips">
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test1.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test1_2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 1 (2nd class)</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2</a>
          <a class="mat-chip" href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test2_2.pdf' | relative_url }}" target="_blank"><span class="chip-icon">📝</span> Test 2 (2nd class)</a>
        </div>
      </div>
    </div>

  </div>

  <p class="no-results" id="no-results">No courses match your search.</p>

</div>

<script>
var activeFilter = 'all';

function setFilter(inst, btn) {
  activeFilter = inst;
  document.querySelectorAll('.filter-btn').forEach(function(b) { b.classList.remove('active'); });
  btn.classList.add('active');
  filterCourses();
}

function filterCourses() {
  var query = document.getElementById('course-search').value.toLowerCase().trim();
  var cards = document.querySelectorAll('.course-card');
  var visible = 0;

  cards.forEach(function(card) {
    var instMatch = activeFilter === 'all' || card.dataset.inst === activeFilter;
    var keywords = (card.dataset.keywords + ' ' + card.querySelector('.course-title').textContent).toLowerCase();
    var queryMatch = query === '' || keywords.indexOf(query) !== -1;
    var show = instMatch && queryMatch;
    card.classList.toggle('hidden', !show);
    if (show) visible++;
  });

  var currentCards = document.querySelectorAll('#grid-current .course-card:not(.hidden)');
  var previousCards = document.querySelectorAll('#grid-previous .course-card:not(.hidden)');
  document.getElementById('label-current').style.display = currentCards.length ? '' : 'none';
  document.getElementById('grid-current').style.display = currentCards.length ? '' : 'none';
  document.querySelector('.section-divider').style.display = (currentCards.length && previousCards.length) ? '' : 'none';
  document.getElementById('label-previous').style.display = previousCards.length ? '' : 'none';
  document.getElementById('grid-previous').style.display = previousCards.length ? '' : 'none';
  document.getElementById('no-results').style.display = visible === 0 ? 'block' : 'none';
}
</script>