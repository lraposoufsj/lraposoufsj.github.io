---
layout: page
permalink: /notes/
title: Lecture Notes
description: Comprehensive lecture notes on topics
nav: true
nav_order: 3
---

<style>
.notes-header {
  text-align: center;
  margin-bottom: 3rem;
}

.notes-header h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.notes-header p {
  font-size: 1.1rem;
  color: var(--global-text-color-light);
}

.search-filter-container {
  margin-bottom: 2rem;
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  align-items: center;
}

.search-box {
  flex: 1;
  min-width: 250px;
}

.search-box input {
  width: 100%;
  padding: 0.75rem 1rem;
  border: 1px solid var(--global-divider-color);
  border-radius: 6px;
  font-size: 1rem;
  background: var(--global-bg-color);
  color: var(--global-text-color);
}

.search-box input:focus {
  outline: none;
  border-color: var(--global-theme-color);
}

.filter-tags {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.filter-tag {
  padding: 0.5rem 1rem;
  border: 1px solid var(--global-divider-color);
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.2s;
  background: var(--global-bg-color);
  color: var(--global-text-color);
  font-size: 0.9rem;
}

.filter-tag:hover {
  border-color: var(--global-theme-color);
  background: var(--global-theme-color);
  color: white;
}

.filter-tag.active {
  background: var(--global-theme-color);
  color: white;
  border-color: var(--global-theme-color);
}

.category-section {
  margin-bottom: 3rem;
}

.category-header {
  font-size: 1.8rem;
  font-weight: 600;
  margin-bottom: 1.5rem;
  color: var(--global-text-color);
  border-bottom: 2px solid var(--global-divider-color);
  padding-bottom: 0.5rem;
  display: flex;
  align-items: center;
  gap: 0.75rem;
}

.category-icon {
  font-size: 1.5rem;
}

.notes-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.note-card {
  border: 1px solid var(--global-divider-color);
  border-radius: 8px;
  padding: 1.5rem;
  background: var(--global-bg-color);
  transition: all 0.2s;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.note-card:hover {
  border-color: var(--global-theme-color);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-2px);
}

.note-card-header {
  margin-bottom: 1rem;
}

.note-card-title {
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.note-card-title a {
  color: var(--global-text-color);
  text-decoration: none;
}

.note-card-title a:hover {
  color: var(--global-theme-color);
}

.note-card-meta {
  display: flex;
  gap: 1rem;
  font-size: 0.85rem;
  color: var(--global-text-color-light);
  margin-bottom: 0.75rem;
}

.note-card-description {
  color: var(--global-text-color);
  line-height: 1.6;
  margin-bottom: 1rem;
  flex-grow: 1;
}

.note-card-tags {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  margin-bottom: 1rem;
}

.note-tag {
  padding: 0.25rem 0.75rem;
  background: var(--global-code-bg-color);
  border-radius: 12px;
  font-size: 0.8rem;
  color: var(--global-theme-color);
}

.note-card-footer {
  display: flex;
  gap: 0.75rem;
  margin-top: auto;
}

.note-link {
  flex: 1;
  text-align: center;
  padding: 0.5rem 1rem;
  background: var(--global-theme-color);
  color: white;
  text-decoration: none;
  border-radius: 4px;
  font-size: 0.9rem;
  transition: all 0.2s;
}

.note-link:hover {
  background: var(--global-hover-color);
  color: white;
  transform: translateY(-1px);
}

.note-link.secondary {
  background: transparent;
  border: 1px solid var(--global-divider-color);
  color: var(--global-text-color);
}

.note-link.secondary:hover {
  border-color: var(--global-theme-color);
  color: var(--global-theme-color);
  background: transparent;
}

.no-results {
  text-align: center;
  padding: 3rem;
  color: var(--global-text-color-light);
  font-size: 1.1rem;
}

@media (max-width: 768px) {
  .notes-grid {
    grid-template-columns: 1fr;
  }
  
  .search-filter-container {
    flex-direction: column;
  }
  
  .search-box {
    width: 100%;
  }
}
</style>

<!-- Search and Filter -->
<div class="search-filter-container">
  <div class="search-box">
    <input type="text" id="search-input" placeholder="🔍 Procure notas por título, tópico ou palavra-chave...">
  </div>
  <div class="filter-tags">
    <span class="filter-tag active" data-filter="all">Todos os Tópicos</span>
    <span class="filter-tag" data-filter="organic-chemistry">Química Orgânica</span>
    <span class="filter-tag" data-filter="general-chemistry">Química Geral</span>
    <span class="filter-tag" data-filter="spectroscopy">Espectroscopia</span>
    <span class="filter-tag" data-filter="intellectual-property">Propriedade Intelectual</span>
    <span class="filter-tag" data-filter="mo-organic-chemistry">Orbitais Moleculares em Química Orgânica</span>
  </div>
</div>

<!-- Organic Chemistry Section -->
<section class="category-section" data-category="organic-chemistry">
  <h2 class="category-header">
    <span class="category-icon">🧪</span>
    Química Orgânica
  </h2>
  <div class="notes-grid">
    
    <div class="note-card" data-tags="organic-chemistry bonding">
      <div class="note-card-header">
        <div class="note-card-title">
          <a href="{{ '/notes/organic-chemistry/qob-20261-m1/' | relative_url }}">QOB-2026-1 - Módulo 1: Ligação Química</a>
        </div>
        <div class="note-card-meta">
          <span>📅 Atualizado em: Maio de 2026</span>
        </div>
      </div>
      <div class="note-card-description">
        Introdução ao estudo da Química Orgânica, revisão de teoria atômica, descrição de orbitais atômicos e de ligações σ e π, hibridação (sp³, sp³ e sp) e geometria molecular.
      </div>
      <div class="note-card-tags">
        <span class="note-tag">Modelo Atômico</span>
        <span class="note-tag">Ligação Química</span>
        <span class="note-tag">Hibridação</span>
        <span class="note-tag">Geometria Molecular</span>
      </div>
      <div class="note-card-footer">
        <a href="{{ '/notes/organic-chemistry/qob-20261-m1/' | relative_url }}" class="note-link">Ler Nota</a>
        <a href="{{ '/assets/pdf/notes/organic-chemistry-bond-theory.pdf' | relative_url }}" class="note-link secondary" download>📥 PDF</a>
      </div>
    </div>

  </div>
</section>

<!-- Spectroscopy Section -->
<section class="category-section" data-category="spectroscopy">
  <h2 class="category-header">
    <span class="category-icon">💻</span>
    Spectroscopy
  </h2>
  <div class="notes-grid">
    
    <div class="note-card" data-tags="programming python basics">
      <div class="note-card-header">
        <div class="note-card-title">
          <a href="{{ '/notes/spectroscopy/molecular-spectroscopy-fundamentals/' | relative_url }}">Molecular Spectroscopy Fundamentals</a>
        </div>
        <div class="note-card-meta">
          <span>📅 Updated: Feb 2025</span>
          <span>📖 25 min read</span>
        </div>
      </div>
      <div class="note-card-description">
        Complete guide to Python basics: variables, data types, control structures, functions, and essential built-in libraries.
      </div>
      <div class="note-card-tags">
        <span class="note-tag">Python</span>
        <span class="note-tag">Basics</span>
        <span class="note-tag">Syntax</span>
      </div>
      <div class="note-card-footer">
        <a href="{{ '/notes/spectroscopy/molecular-spectroscopy-fundamentals/' | relative_url }}" class="note-link">Read Note</a>
        <a href="{{ '/assets/pdf/notes/programming-python-fundamentals.pdf' | relative_url }}" class="note-link secondary" download>📥 PDF</a>
      </div>
    </div>

    <div class="note-card" data-tags="programming oop">
      <div class="note-card-header">
        <div class="note-card-title">
          <a href="{{ '/notes/programming/object-oriented/' | relative_url }}">Object-Oriented Programming</a>
        </div>
        <div class="note-card-meta">
          <span>📅 Updated: Jan 2025</span>
          <span>📖 30 min read</span>
        </div>
      </div>
      <div class="note-card-description">
        Deep dive into OOP concepts: classes, objects, inheritance, polymorphism, encapsulation, and design patterns.
      </div>
      <div class="note-card-tags">
        <span class="note-tag">OOP</span>
        <span class="note-tag">Design Patterns</span>
        <span class="note-tag">Java</span>
      </div>
      <div class="note-card-footer">
        <a href="{{ '/notes/programming/object-oriented/' | relative_url }}" class="note-link">Read Note</a>
        <a href="{{ '/assets/pdf/notes/programming-oop.pdf' | relative_url }}" class="note-link secondary" download>📥 PDF</a>
      </div>
    </div>

  </div>
</section>

<div class="no-results" id="no-results" style="display: none;">
  <p>No notes found matching your search. Try different keywords or select "All Topics".</p>
</div>

<script>
// Search functionality
const searchInput = document.getElementById('search-input');
const filterTags = document.querySelectorAll('.filter-tag');
const noteCards = document.querySelectorAll('.note-card');
const categorySections = document.querySelectorAll('.category-section');
const noResults = document.getElementById('no-results');

let currentFilter = 'all';

// Search function
searchInput.addEventListener('input', function() {
  const searchTerm = this.value.toLowerCase();
  filterNotes(searchTerm, currentFilter);
});

// Filter tags
filterTags.forEach(tag => {
  tag.addEventListener('click', function() {
    filterTags.forEach(t => t.classList.remove('active'));
    this.classList.add('active');
    currentFilter = this.getAttribute('data-filter');
    const searchTerm = searchInput.value.toLowerCase();
    filterNotes(searchTerm, currentFilter);
  });
});

function filterNotes(searchTerm, category) {
  let visibleCount = 0;
  
  // Hide all sections first
  categorySections.forEach(section => {
    section.style.display = 'none';
  });
  
  noteCards.forEach(card => {
    const title = card.querySelector('.note-card-title').textContent.toLowerCase();
    const description = card.querySelector('.note-card-description').textContent.toLowerCase();
    const tags = card.getAttribute('data-tags').toLowerCase();
    
    const matchesSearch = title.includes(searchTerm) || 
                         description.includes(searchTerm) || 
                         tags.includes(searchTerm);
    
    const matchesCategory = category === 'all' || tags.includes(category);
    
    if (matchesSearch && matchesCategory) {
      card.style.display = 'flex';
      // Show the parent section
      const parentSection = card.closest('.category-section');
      if (parentSection) {
        parentSection.style.display = 'block';
      }
      visibleCount++;
    } else {
      card.style.display = 'none';
    }
  });
  
  // Show/hide no results message
  if (visibleCount === 0) {
    noResults.style.display = 'block';
  } else {
    noResults.style.display = 'none';
  }
}
</script>