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
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">💻 Materials</a>
            <a href="#" class="course-link">💯 Tests</a>
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
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">💻 Materials</a>
            <a href="#" class="course-link">💯 Tests</a>
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
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">💻 Materials</a>
            <a href="#" class="course-link">💯 Tests</a>
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
            <a href="#" class="course-link">💯 Tests</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Previous Position -->
    <section id="unifei" class="institution-section">
      <h2 class="institution-header">Federal University of Itajubá (UNIFEI)</h2>
      <p><strong>Substitute Professor</strong> | 2024</p>
      
      <div class="semester-group">
        <h3 class="semester-header">2025/1</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">ENG201</span> - Calculus II
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Multivariable calculus including partial derivatives, multiple integrals, and vector calculus for engineering students.
          </div>
          <div class="course-links">
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">📊 Lecture Notes</a>
          </div>
        </div>
      </div>

      <div class="semester-group">
        <h3 class="semester-header">2024/4 (Summer Course)</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">CS100</span> - Intensive Programming Workshop
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Two-week intensive workshop introducing programming concepts for incoming students. Hands-on approach with daily coding exercises.
          </div>
          <div class="course-links">
            <a href="#" class="course-link">💻 Workshop Materials</a>
            <a href="#" class="course-link">🎯 Exercises</a>
          </div>
        </div>
      </div>

      <div class="semester-group">
        <h3 class="semester-header">2024/2</h3>
        
        <div class="course-card">
          <div class="course-title">
            <span class="course-code">MATH150</span> - Linear Algebra
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Introduction to vector spaces, linear transformations, matrices, eigenvalues, and eigenvectors with applications to engineering problems.
          </div>
          <div class="course-links">
            <a href="#" class="course-link">📝 Syllabus</a>
            <a href="#" class="course-link">📚 Resources</a>
          </div>
        </div>

        <div class="course-card">
          <div class="course-title">
            <span class="course-code">CS205</span> - Object-Oriented Programming
          </div>
          <div class="course-role">Substitute Professor</div>
          <div class="course-description">
            Core OOP concepts using Java including inheritance, polymorphism, interfaces, and design patterns. Project-based learning approach.
          </div>
          <div class="course-links">
            <a href="#" class="course-link">📚 Course Page</a>
            <a href="#" class="course-link">💻 Code Examples</a>
            <a href="#" class="course-link">📊 Projects</a>
          </div>
        </div>
      </div>
    </section>

  </div>
</div>
