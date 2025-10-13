---
layout: page
permalink: /teaching/
title: Teaching
description: Courses, materials, and teaching experience
nav: true
nav_order: 2
---

<style>
.teaching-container {
  display: flex;
  gap: 2rem;
  margin-top: 2rem;
}

.toc-sidebar {
  position: sticky;
  top: 2rem;
  width: 250px;
  height: fit-content;
  padding: 1.5rem;
  background: var(--global-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 6px;
}

.toc-sidebar h3 {
  margin-top: 0;
  font-size: 1.1rem;
  margin-bottom: 1rem;
  color: var(--global-text-color);
}

.toc-sidebar ul {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.toc-sidebar li {
  margin-bottom: 0.5rem;
}

.toc-sidebar a {
  color: var(--global-theme-color);
  text-decoration: none;
  font-size: 0.95rem;
  transition: all 0.2s;
}

.toc-sidebar a:hover {
  color: var(--global-hover-color);
  padding-left: 0.5rem;
}

.teaching-content {
  flex: 1;
  min-width: 0;
}

.institution-section {
  margin-bottom: 3rem;
}

.institution-header {
  font-size: 1.8rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: var(--global-text-color);
  border-bottom: 2px solid var(--global-divider-color);
  padding-bottom: 0.5rem;
}

.semester-group {
  margin-bottom: 2.5rem;
}

.semester-header {
  font-size: 1.3rem;
  font-weight: 500;
  color: var(--global-theme-color);
  margin-bottom: 1rem;
  margin-top: 1.5rem;
}

.course-card {
  padding: 1.25rem;
  margin-bottom: 1rem;
  background: var(--global-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 6px;
  transition: all 0.2s;
}

.course-card:hover {
  border-color: var(--global-theme-color);
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.course-title {
  font-size: 1.15rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: var(--global-text-color);
}

.course-code {
  color: var(--global-theme-color);
  font-family: monospace;
  font-size: 0.9rem;
}

.course-role {
  color: var(--global-text-color-light);
  font-style: italic;
  margin-bottom: 0.75rem;
}

.course-description {
  margin-bottom: 0.75rem;
  color: var(--global-text-color);
  line-height: 1.6;
}

.course-links {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.course-link {
  display: inline-block;
  padding: 0.4rem 0.8rem;
  background: var(--global-theme-color);
  color: white;
  text-decoration: none;
  border-radius: 4px;
  font-size: 0.9rem;
  transition: all 0.2s;
}

.course-link:hover {
  background: var(--global-hover-color);
  color: white;
  transform: translateY(-2px);
}

.materials-toggle {
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  background: var(--global-code-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 4px;
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  align-items: center;
  transition: all 0.2s;
}

.materials-toggle:hover {
  background: var(--global-divider-color);
}

.materials-toggle-icon {
  transition: transform 0.3s;
}

.materials-toggle-icon.open {
  transform: rotate(180deg);
}

.materials-content {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease-out;
}

.materials-content.open {
  max-height: 1000px;
  transition: max-height 0.5s ease-in;
}

.materials-section {
  margin-top: 1rem;
  padding: 1rem;
  background: var(--global-code-bg-color);
  border-radius: 4px;
}

.materials-section h4 {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 0.75rem;
  color: var(--global-theme-color);
}

.materials-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.materials-list li {
  margin-bottom: 0.5rem;
}

.materials-list a {
  color: var(--global-text-color);
  text-decoration: none;
  display: flex;
  align-items: center;
  padding: 0.4rem 0.6rem;
  border-radius: 3px;
  transition: all 0.2s;
}

.materials-list a:hover {
  background: var(--global-bg-color);
  color: var(--global-theme-color);
}

.materials-list a::before {
  content: "📄";
  margin-right: 0.5rem;
}

@media (max-width: 768px) {
  .teaching-container {
    flex-direction: column;
  }
  
  .toc-sidebar {
    position: relative;
    width: 100%;
    top: 0;
  }
}
</style>

<div class="teaching-container">
  <aside class="toc-sidebar">
    <h3>Quick Navigation</h3>
    <ul>
      <li><a href="#ufsj">Federal University of São João del Rei (UFSJ)</a></li>
      <li><a href="#unifei">Federal University of Itajubá (UNIFEI)</a></li>
    </ul>
  </aside>

  <div class="teaching-content">
    
    <!-- Current Position -->
    <section id="ufsj" class="institution-section">
      <h2 class="institution-header">Federal University of São João del Rei (UFSJ)</h2>
      <p><strong>Assistant Professor</strong> | 2025 - Present</p>
      
      <div class="semester-group">
        <h3 class="semester-header">2025/1</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QU03819740</span> - Experimental Biochemistry
          </div>
          <div class="course-role">Assistant Professor</div>
          <div class="course-description">
            Foundational course covering essential laboratory techniques in Biochemistry, such as the extraction and chemical analysis of starch, coconut oil, soybean protein, DNA, and SDS-PAGE techniques.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/ufsj/2025-2/BQE_20252_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/ufsj/2025-2/BQE_20252_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="#" class="course-link">💯 Test 1</a>
            <a href="#" class="course-link">💯 Test 2</a>
            <a href="#" class="course-link">💯 Substitute Test</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QU03419695</span> - Introduction to the Organic Chemistry Laboratory
          </div>
          <div class="course-role">Assistant Professor</div>
          <div class="course-description">
            Foundational course covering essential laboratory techniques in Organic Chemistry, such as liquid-liquid extraction, distillation, chromatography, recrystallization, aliphatic carbon and carbonyl substitutions, diazotization reactions, and functional group identification.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/ufsj/2025-2/ILQO_20252_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="#" class="course-link">💯 Test 1</a>
            <a href="#" class="course-link">💯 Test 2</a>
            <a href="#" class="course-link">💯 Substitute Test</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QU03319694</span> - Physical Methods in Organic Chemistry
          </div>
          <div class="course-role">Assistant Professor</div>
          <div class="course-description">
            Foundational course covering essential structure elucidation techniques for organic compounds, such as infrared (IR) and nuclear magnetic resonance (NMR) spectroscopies, and mass spectrometry (MS).
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
          </div>

          <!-- Expandable Materials Section -->
          <div class="materials-toggle" onclick="toggleMaterials(this)">
            <span><strong>📂 Course Materials</strong></span>
            <span class="materials-toggle-icon">▼</span>
          </div>
          <div class="materials-content">
            <div class="materials-section">
              <h4>📖 Lecture Notes and Slides</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Slides_Mod1.pdf' | relative_url }}" target="_blank">Part 01 - Mass Spectrometry (MS)</a></li>
                <li><a href="#" target="_blank">Part 02 - Infrared Spectroscopy (IR)</a></li>
                <li><a href="#" target="_blank">Part 03 - Nuclear Magnetic Resonance Spectroscopy (NMR)</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>📝 Exams and Tests</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/ufsj/2025-2/MFQO_20252_Test1.pdf' | relative_url }}" target="_blank">Test 1 - MS</a></li>
                <li><a href="#" target="_blank">Test 2 - MS and IR</a></li>
                <li><a href="#" target="_blank">Test 3 - MS, IR, and NMR</a></li>
                <li><a href="#" target="_blank">Substitute Test</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>💻 Exercises</h4>
              <ul class="materials-list">
                <li><a href="#" target="_blank">Assignment 1 - Implementing a Linked List</a></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">CNA0001</span> - General Chemistry for Engineering
          </div>
          <div class="course-role">Assistant Professor</div>
          <div class="course-description">
            Shared foundational course covering essential Chemistry-related topics. Topics include stoichiometry, thermochemistry, chemical equilibrium, chemical kinetics, and electrochemistry.
          </div>
          <div class="course-links">
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">💻 Materials</a>
            <a href="#" class="course-link">💯 Test 1</a>
            <a href="#" class="course-link">💯 Test 2</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Previous Position -->
    <section id="unifei" class="institution-section">
      <h2 class="institution-header">Federal University of Itajubá (UNIFEI)</h2>
      <p><strong>Substitute Professor</strong> | 2024/25</p>
      
      <div class="semester-group">
        <h3 class="semester-header">2025/1</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI016</span> - General Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course for Chemical and Bioprocesses Engineering, and Biology, covering atomic theory and electronic structure, chemical bonds, gases, liquids and solutions, thermodynamics, chemical kinetics, and electrochemistry.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
          </div>

          <!-- Expandable Materials Section -->
          <div class="materials-toggle" onclick="toggleMaterials(this)">
            <span><strong>📂 Course Materials</strong></span>
            <span class="materials-toggle-icon">▼</span>
          </div>
          <div class="materials-content">
            <div class="materials-section">
              <h4>📖 Lecture Notes and Slides</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Lecture_Notes_M1.pdf' | relative_url }}" target="_blank">Part 1 - UV-Vis Spectroscopy</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M2.pdf' | relative_url }}" target="_blank">Part 2 - Infrared Spectroscopy</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p1.pdf' | relative_url }}" target="_blank">Part 3A - NMR (Introduction and Concepts)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p2.pdf' | relative_url }}" target="_blank">Part 3B - NMR (Proton NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p3.pdf' | relative_url }}" target="_blank">Part 3C - NMR (Carbon-13 NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p4.pdf' | relative_url }}" target="_blank">Part 3D - NMR (J coupling and 2D NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M4.pdf' | relative_url }}" target="_blank">Part 4 - Mass Spectrometry</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>📝 Exams and Tests</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_ShortTest1.pdf' | relative_url }}" target="_blank">Short Test 1 - Part 2</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test1.pdf' | relative_url }}" target="_blank">Test 1 - Parts 1 to 4</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_ShortTest2.pdf' | relative_url }}" target="_blank">Short Test 2 - Part 5</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test2.pdf' | relative_url }}" target="_blank">Test 2 - Parts 6, 7, and 9</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI016_20251_Test_Sub.pdf' | relative_url }}" target="_blank">Substitute Test - Parts 1 to 4, 6, 7, and 9</a></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI017</span> - Experimental General Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course for Chemistry and Chemical Engineering, covering macroscopic evidence of chemical reactions, stoichiometry, standardization, the copper cycle, chemical kinetics, chemical equilibrium, precipitation reactions, and electrochemistry.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Test1.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1</a>
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI017_20251_Test2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI070</span> - Physical Methods for Analysis
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course for Chemistry covering essential spectroscopic and spectrometric tools for the analysis of Organic Compounds, such as UV-Vis, FTIR, MS, and NMR.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
          </div>

          <!-- Expandable Materials Section -->
          <div class="materials-toggle" onclick="toggleMaterials(this)">
            <span><strong>📂 Course Materials</strong></span>
            <span class="materials-toggle-icon">▼</span>
          </div>
          <div class="materials-content">
            <div class="materials-section">
              <h4>📖 Lecture Notes and Slides</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Lecture_Notes_M1.pdf' | relative_url }}" target="_blank">Part 1 - UV-Vis Spectroscopy</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M2.pdf' | relative_url }}" target="_blank">Part 2 - Infrared Spectroscopy</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p1.pdf' | relative_url }}" target="_blank">Part 3A - NMR (Introduction and Concepts)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p2.pdf' | relative_url }}" target="_blank">Part 3B - NMR (Proton NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p3.pdf' | relative_url }}" target="_blank">Part 3C - NMR (Carbon-13 NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M3_p4.pdf' | relative_url }}" target="_blank">Part 3D - NMR (J coupling and 2D NMR)</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Slides_M4.pdf' | relative_url }}" target="_blank">Part 4 - Mass Spectrometry</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>📝 Exams and Tests</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test1.pdf' | relative_url }}" target="_blank">Test 1 - Parts 1 and 2</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test2.pdf' | relative_url }}" target="_blank">Test 2 - Parts 1 to 3</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test3.pdf' | relative_url }}" target="_blank">Test 3 - Parts 1 to 4</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Test_Sub.pdf' | relative_url }}" target="_blank">Substitute Test - Parts 1 to 4</a></li>
              </ul>
            </div>

            <div class="materials-section">
              <h4>💻 Exercises</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2025-1/QUI070_20251_Solved_ex_M3.pdf' | relative_url }}" target="_blank">Solved Exercises - NMR Spectroscopy</a></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI212</span> - Experimental General Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course covering essential experimental aspects of Chemistry for Engineering courses, covering macroscopical evidence of chemical reactions, chemical equilibrium, chemical thermodynamics, and electrochemistry.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Test1.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1</a>
            <a href="{{ '/assets/pdf/unifei/2025-1/QUI212_20251_Test2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2</a>
          </div>
        </div>
      </div>

      <div class="semester-group">
        <h3 class="semester-header">2024/4 (Summer Course)</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI055</span> - Organic Chemistry II
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course taught during Jan/2025 covering substitution and elimination reactions, reactions of alkenes and alkynes, reactions of aromatic compounds, reactions of alcohols and ethers (including oxidation and reduction processes), organometallic chemistry, and carboxylic acid derivatives and their reactions.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
          </div>

          <!-- Expandable Materials Section -->
          <div class="materials-toggle" onclick="toggleMaterials(this)">
            <span><strong>📂 Course Materials</strong></span>
            <span class="materials-toggle-icon">▼</span>
          </div>
          <div class="materials-content">
            <div class="materials-section">
              <h4>📖 Lecture Notes and Slides</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M1.pdf' | relative_url }}" target="_blank">Part 1 - Alkenes and alkynes</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M2.pdf' | relative_url }}" target="_blank">Part 2 - Alkene addition reactions</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Slides_M3.pdf' | relative_url }}" target="_blank">Part 3 - Conjugated alkenes</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M4.pdf' | relative_url }}" target="_blank">Part 4 - Aromatic compounds</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M5.pdf' | relative_url }}" target="_blank">Part 5 - Alcohols and Ethers</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Lecture_Notes_M6.pdf' | relative_url }}" target="_blank">Part 6 - Oxidations, reductions, and RLi/RMgX</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>📝 Exams and Tests</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test1.pdf' | relative_url }}" target="_blank">Test 1 - Parts 1 and 2</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test2.pdf' | relative_url }}" target="_blank">Test 2 - Parts 1 to 4</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test3.pdf' | relative_url }}" target="_blank">Test 3 - Parts 1 to 5</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-summer/QUI055_20244_Test4.pdf' | relative_url }}" target="_blank">Test 4 - Parts 1 to 7</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <div class="semester-group">
        <h3 class="semester-header">2024/2</h3>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI022</span> - Organic Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course covering essential theoretical aspects of Organic Chemistry for Chemical and Materials Engineering, such as organic acids and bases, bond theory and conjugation, physical and chemical properties of organic compounds, radical reactions, electrophilic aromatic substitution reactions, and carboxyl condensation reactions.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
          </div>

          <!-- Expandable Materials Section -->
          <div class="materials-toggle" onclick="toggleMaterials(this)">
            <span><strong>📂 Course Materials</strong></span>
            <span class="materials-toggle-icon">▼</span>
          </div>
          <div class="materials-content">
            <div class="materials-section">
              <h4>📖 Lecture Notes</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M1.pdf' | relative_url }}" target="_blank">Part 1 - Representation and Bond Theory</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M2.pdf' | relative_url }}" target="_blank">Part 2 - Inductive and Mesomeric Effect</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M3.pdf' | relative_url }}" target="_blank">Part 3 - Functional Groups</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M4.pdf' | relative_url }}" target="_blank">Part 4 - Nomenclature</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M5.pdf' | relative_url }}" target="_blank">Part 5 - Physical and Chemical Properties</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M6.pdf' | relative_url }}" target="_blank">Part 6 - Acids and Bases</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M7.pdf' | relative_url }}" target="_blank">Part 7 - Stereochemistry</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M8.pdf' | relative_url }}" target="_blank">Part 8 - Radical Reactions</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M9.pdf' | relative_url }}" target="_blank">Part 9 - Alkene Addition Reactions</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M10.pdf' | relative_url }}" target="_blank">Part 10 - Electrophilic Aromatic Substitution Reactions</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Lecture_Notes_M11.pdf' | relative_url }}" target="_blank">Part 11 - Carbonyl Substitution and Addition Reactions</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>📝 Exams and Tests</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest1.pdf' | relative_url }}" target="_blank">Short Test 1 - Part 2</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test1.pdf' | relative_url }}" target="_blank">Test 1 - Parts 1 to 5</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest2.pdf' | relative_url }}" target="_blank">Short Test 2 - Part 8</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test2.pdf' | relative_url }}" target="_blank">Test 2 - Parts 1 to 9</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_ShortTest3.pdf' | relative_url }}" target="_blank">Short Test 3 - Part 10</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_Test3.pdf' | relative_url }}" target="_blank">Test 3 - Parts 1 to 11</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_TestSub.pdf' | relative_url }}" target="_blank">Replacement Test - Parts 1 to 11</a></li>
              </ul>
            </div>
            
            <div class="materials-section">
              <h4>💻 Exercises</h4>
              <ul class="materials-list">
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_List1.pdf' | relative_url }}" target="_blank">Exercise List 1 - Parts 1 to 5</a></li>
                <li><a href="{{ '/assets/pdf/unifei/2024-2/QUI022_20242_List2.pdf' | relative_url }}" target="_blank">Exercise List 2 - Parts 6 to 9</a></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI068</span> - Experimental Organic Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course covering essential experimental aspects of Organic Chemistry for Chemical and Materials Engineering, such as liquid-liquid extraction, chromatography (TLC and silica column), production of ASA, and recrystalization.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Test1.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI068_20242_Test2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI113</span> - Experimental Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course covering essential experimental aspects of Chemistry for Physics, Biology, and Bioprocess Engineering courses, covering macroscopical evidence of chemical reactions, stoichiometry, standardization, chemical kinetics, and chemical equilibrium.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Test1.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI113_20242_Test2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">QUI212</span> - Experimental General Chemistry
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Foundational course covering essential experimental aspects of Chemistry for Engineering courses, covering macroscopical evidence of chemical reactions, chemical equilibrium, chemical thermodynamics, and electrochemistry.
          </div>
          <div class="course-links">
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Syllabus.pdf' | relative_url }}" target="_blank" class="course-link">📝 Syllabus</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Exp_Prot.pdf' | relative_url }}" target="_blank" class="course-link">🧪 Experiments</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test1.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test1_2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 1 (2nd class)</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2</a>
            <a href="{{ '/assets/pdf/unifei/2024-2/QUI212_20242_Test2_2.pdf' | relative_url }}" target="_blank" class="course-link">💯 Test 2 (2nd class)</a>
          </div>
        </div>
      </div>
    </section>
    
  </div>
</div>

<script>
function toggleMaterials(element) {
  const content = element.nextElementSibling;
  const icon = element.querySelector('.materials-toggle-icon');
  
  content.classList.toggle('open');
  icon.classList.toggle('open');
}
</script>
