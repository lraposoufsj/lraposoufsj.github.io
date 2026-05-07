---
layout: page
title: "Molecular Spectroscopy Fundamentals"
permalink: /notes/spectroscopy/molecular-spectroscopy-fundamentals/
description: Energy levels, transitions, and spectroscopic selection rules with interactive visualizations
---

<!-- Include MathJax for LaTeX rendering -->
<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.0/es5/tex-mml-chtml.js">
</script>

<!-- Include Plotly for interactive plots -->
<script src="https://cdn.plot.ly/plotly-2.27.0.min.js"></script>

<style>
/* Import the note styling from previous template */
.note-container {
  display: flex;
  gap: 2rem;
  margin-top: 2rem;
  position: relative;
}

.note-toc {
  position: sticky;
  top: 2rem;
  width: 280px;
  height: fit-content;
  padding: 1.5rem;
  background: var(--global-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 6px;
  flex-shrink: 0;
}

.note-content {
  flex: 1;
  min-width: 0;
  max-width: 800px;
}

.note-body {
  line-height: 1.8;
  font-size: 1.05rem;
}

.note-body h2 {
  font-size: 1.8rem;
  margin-top: 2.5rem;
  margin-bottom: 1rem;
  color: var(--global-text-color);
  border-bottom: 1px solid var(--global-divider-color);
  padding-bottom: 0.5rem;
}

.note-body h3 {
  font-size: 1.4rem;
  margin-top: 2rem;
  margin-bottom: 0.75rem;
}

/* Scientific equation styling */
.equation-block {
  margin: 2rem 0;
  padding: 1.5rem;
  background: var(--global-code-bg-color);
  border-left: 4px solid var(--global-theme-color);
  border-radius: 6px;
  overflow-x: auto;
}

.equation-number {
  float: right;
  color: var(--global-text-color-light);
  font-size: 0.9rem;
}

.equation-label {
  display: block;
  font-weight: 600;
  color: var(--global-theme-color);
  margin-bottom: 0.75rem;
  font-size: 0.95rem;
}

/* Professional table styling (booktabs-inspired) */
.scientific-table {
  width: 100%;
  margin: 2rem 0;
  border-collapse: collapse;
  font-size: 0.95rem;
}

.scientific-table caption {
  caption-side: top;
  text-align: left;
  font-weight: 600;
  padding: 0.75rem 0;
  color: var(--global-text-color);
  font-size: 1rem;
}

.scientific-table thead {
  border-top: 2px solid var(--global-text-color);
  border-bottom: 1.5px solid var(--global-text-color);
}

.scientific-table thead th {
  padding: 0.75rem 1rem;
  text-align: left;
  font-weight: 600;
  color: var(--global-text-color);
}

.scientific-table tbody tr {
  border-bottom: 0.5px solid var(--global-divider-color);
}

.scientific-table tbody tr:last-child {
  border-bottom: 2px solid var(--global-text-color);
}

.scientific-table tbody td {
  padding: 0.75rem 1rem;
  color: var(--global-text-color);
}

.scientific-table tbody tr:hover {
  background: var(--global-code-bg-color);
}

.scientific-table .number {
  text-align: right;
  font-family: 'Monaco', 'Courier New', monospace;
}

.scientific-table .centered {
  text-align: center;
}

/* Interactive plot container */
.plot-container {
  margin: 2rem 0;
  padding: 1.5rem;
  background: var(--global-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 8px;
}

.plot-title {
  font-weight: 600;
  margin-bottom: 1rem;
  color: var(--global-text-color);
  font-size: 1.1rem;
}

.plot-caption {
  margin-top: 1rem;
  font-size: 0.9rem;
  color: var(--global-text-color-light);
  font-style: italic;
}

/* Figure styling */
figure {
  margin: 2rem 0;
  text-align: center;
}

figure img {
  max-width: 100%;
  height: auto;
  border-radius: 6px;
  border: 1px solid var(--global-divider-color);
}

figcaption {
  margin-top: 1rem;
  font-size: 0.9rem;
  color: var(--global-text-color-light);
  font-style: italic;
}

@media (max-width: 1024px) {
  .note-container {
    flex-direction: column;
  }
  
  .note-toc {
    position: relative;
    width: 100%;
    top: 0;
  }
}
</style>

<div class="note-container">
  <aside class="note-toc">
    <h3>📑 Contents</h3>
    <ul>
      <li><a href="#energy-levels">Energy Levels</a></li>
      <li><a href="#beer-lambert">Beer-Lambert Law</a></li>
      <li><a href="#electronegativity">Electronegativity Trends</a></li>
      <li><a href="#spectral-data">Spectral Data Tables</a></li>
      <li><a href="#molecular-vibrations">Molecular Vibrations</a></li>
    </ul>
  </aside>

  <main class="note-content">
    <article class="note-body">
      
      <h2 id="energy-levels">Energy Levels and Transitions</h2>
      
      <p>
        The energy of electromagnetic radiation is quantized and relates to frequency through Planck's equation:
      </p>

      <div class="equation-block">
        <span class="equation-label">Planck's Equation</span>
        <span class="equation-number">(1)</span>
        $$E = h\nu = \frac{hc}{\lambda}$$
      </div>

      <p>where:</p>
      <ul>
        <li>\(E\) is the energy of the photon (J)</li>
        <li>\(h\) is Planck's constant (\(6.626 \times 10^{-34}\) J·s)</li>
        <li>\(\nu\) is the frequency (Hz)</li>
        <li>\(c\) is the speed of light (\(2.998 \times 10^8\) m/s)</li>
        <li>\(\lambda\) is the wavelength (m)</li>
      </ul>

      <p>
        The energy difference between two quantum states determines the wavelength of absorbed or emitted radiation:
      </p>

      <div class="equation-block">
        <span class="equation-label">Energy Transition</span>
        <span class="equation-number">(2)</span>
        $$\Delta E = E_2 - E_1 = h\nu = \frac{hc}{\lambda}$$
      </div>

      <h2 id="beer-lambert">The Beer-Lambert Law</h2>

      <p>
        The Beer-Lambert law describes the attenuation of light passing through a solution. It's fundamental to quantitative spectroscopy:
      </p>

      <div class="equation-block">
        <span class="equation-label">Beer-Lambert Law</span>
        <span class="equation-number">(3)</span>
        $$A = \log_{10}\left(\frac{I_0}{I}\right) = \varepsilon \cdot c \cdot l$$
      </div>

      <p>where:</p>
      <ul>
        <li>\(A\) is the absorbance (dimensionless)</li>
        <li>\(I_0\) is the incident light intensity</li>
        <li>\(I\) is the transmitted light intensity</li>
        <li>\(\varepsilon\) is the molar absorptivity (L mol<sup>-1</sup> cm<sup>-1</sup>)</li>
        <li>\(c\) is the concentration (mol L<sup>-1</sup>)</li>
        <li>\(l\) is the path length (cm)</li>
      </ul>

      <p>
        Transmittance (\(T\)) is related to absorbance by:
      </p>

      <div class="equation-block">
        <span class="equation-number">(4)</span>
        $$T = \frac{I}{I_0} = 10^{-A}$$
        <br><br>
        $$A = -\log_{10}(T) = 2 - \log_{10}(\%T)$$
      </div>

      <h2 id="electronegativity">Electronegativity Trends</h2>

      <p>
        Pauling electronegativity values show periodic trends across the periodic table. Here's an interactive visualization showing how electronegativity varies with atomic number:
      </p>

      <div class="plot-container">
        <div class="plot-title">Figure 1: Pauling Electronegativity vs. Atomic Number</div>
        <div id="electronegativity-plot"></div>
        <div class="plot-caption">
          Hover over points to see element names and electronegativity values. Note the periodic trends and the gap for noble gases.
        </div>
      </div>

      <script>
        // Electronegativity data (selected elements)
        const elements = [
          {z: 1, symbol: 'H', name: 'Hydrogen', en: 2.20},
          {z: 3, symbol: 'Li', name: 'Lithium', en: 0.98},
          {z: 4, symbol: 'Be', name: 'Beryllium', en: 1.57},
          {z: 5, symbol: 'B', name: 'Boron', en: 2.04},
          {z: 6, symbol: 'C', name: 'Carbon', en: 2.55},
          {z: 7, symbol: 'N', name: 'Nitrogen', en: 3.04},
          {z: 8, symbol: 'O', name: 'Oxygen', en: 3.44},
          {z: 9, symbol: 'F', name: 'Fluorine', en: 3.98},
          {z: 11, symbol: 'Na', name: 'Sodium', en: 0.93},
          {z: 12, symbol: 'Mg', name: 'Magnesium', en: 1.31},
          {z: 13, symbol: 'Al', name: 'Aluminum', en: 1.61},
          {z: 14, symbol: 'Si', name: 'Silicon', en: 1.90},
          {z: 15, symbol: 'P', name: 'Phosphorus', en: 2.19},
          {z: 16, symbol: 'S', name: 'Sulfur', en: 2.58},
          {z: 17, symbol: 'Cl', name: 'Chlorine', en: 3.16},
          {z: 19, symbol: 'K', name: 'Potassium', en: 0.82},
          {z: 20, symbol: 'Ca', name: 'Calcium', en: 1.00},
          {z: 35, symbol: 'Br', name: 'Bromine', en: 2.96},
          {z: 53, symbol: 'I', name: 'Iodine', en: 2.66}
        ];

        const trace = {
          x: elements.map(e => e.z),
          y: elements.map(e => e.en),
          mode: 'markers+lines',
          type: 'scatter',
          name: 'Electronegativity',
          marker: {
            size: 10,
            color: elements.map(e => e.en),
            colorscale: 'Viridis',
            showscale: true,
            colorbar: {
              title: 'Pauling EN',
              thickness: 15
            }
          },
          text: elements.map(e => `${e.name} (${e.symbol})<br>Z = ${e.z}<br>EN = ${e.en}`),
          hovertemplate: '%{text}<extra></extra>',
          line: {
            color: 'rgba(100, 100, 100, 0.3)',
            width: 1
          }
        };

        const layout = {
          xaxis: {
            title: 'Atomic Number (Z)',
            gridcolor: 'rgba(200, 200, 200, 0.3)'
          },
          yaxis: {
            title: 'Pauling Electronegativity',
            gridcolor: 'rgba(200, 200, 200, 0.3)'
          },
          plot_bgcolor: 'rgba(0,0,0,0)',
          paper_bgcolor: 'rgba(0,0,0,0)',
          font: {
            family: 'inherit'
          },
          hovermode: 'closest',
          showlegend: false,
          margin: {l: 60, r: 30, t: 30, b: 60}
        };

        const config = {
          responsive: true,
          displayModeBar: true,
          displaylogo: false,
          modeBarButtonsToRemove: ['lasso2d', 'select2d']
        };

        Plotly.newPlot('electronegativity-plot', [trace], layout, config);
      </script>

      <h2 id="spectral-data">Spectral Data Tables</h2>

      <p>
        Characteristic IR absorption frequencies for common functional groups:
      </p>

      <table class="scientific-table">
        <caption>Table 1: Characteristic IR Absorption Frequencies</caption>
        <thead>
          <tr>
            <th>Functional Group</th>
            <th>Bond Type</th>
            <th class="number">Frequency (cm<sup>-1</sup>)</th>
            <th>Intensity</th>
            <th>Notes</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Alkane</td>
            <td>C–H stretch</td>
            <td class="number">2850–2960</td>
            <td class="centered">strong</td>
            <td>sp<sup>3</sup> hybridized C–H</td>
          </tr>
          <tr>
            <td>Alkene</td>
            <td>C=C stretch</td>
            <td class="number">1620–1680</td>
            <td class="centered">medium</td>
            <td>Variable intensity</td>
          </tr>
          <tr>
            <td>Alkene</td>
            <td>=C–H stretch</td>
            <td class="number">3020–3100</td>
            <td class="centered">medium</td>
            <td>sp<sup>2</sup> hybridized C–H</td>
          </tr>
          <tr>
            <td>Alkyne</td>
            <td>C≡C stretch</td>
            <td class="number">2100–2260</td>
            <td class="centered">weak</td>
            <td>Terminal alkynes stronger</td>
          </tr>
          <tr>
            <td>Alkyne</td>
            <td>≡C–H stretch</td>
            <td class="number">3260–3330</td>
            <td class="centered">strong</td>
            <td>Sharp, distinctive peak</td>
          </tr>
          <tr>
            <td>Alcohol</td>
            <td>O–H stretch</td>
            <td class="number">3200–3550</td>
            <td class="centered">strong</td>
            <td>Broad; H-bonded</td>
          </tr>
          <tr>
            <td>Carboxylic Acid</td>
            <td>O–H stretch</td>
            <td class="number">2500–3300</td>
            <td class="centered">strong</td>
            <td>Very broad; dimer</td>
          </tr>
          <tr>
            <td>Carbonyl</td>
            <td>C=O stretch</td>
            <td class="number">1670–1820</td>
            <td class="centered">strong</td>
            <td>Exact position varies</td>
          </tr>
          <tr>
            <td>Aldehyde</td>
            <td>C=O stretch</td>
            <td class="number">1720–1740</td>
            <td class="centered">strong</td>
            <td>—</td>
          </tr>
          <tr>
            <td>Ketone</td>
            <td>C=O stretch</td>
            <td class="number">1705–1725</td>
            <td class="centered">strong</td>
            <td>—</td>
          </tr>
          <tr>
            <td>Ester</td>
            <td>C=O stretch</td>
            <td class="number">1735–1750</td>
            <td class="centered">strong</td>
            <td>Higher than ketones</td>
          </tr>
          <tr>
            <td>Amine</td>
            <td>N–H stretch</td>
            <td class="number">3300–3500</td>
            <td class="centered">medium</td>
            <td>Primary: 2 peaks</td>
          </tr>
          <tr>
            <td>Nitrile</td>
            <td>C≡N stretch</td>
            <td class="number">2210–2260</td>
            <td class="centered">medium</td>
            <td>Sharp peak</td>
          </tr>
        </tbody>
      </table>

      <h2 id="molecular-vibrations">Molecular Vibrations</h2>

      <p>
        A non-linear molecule with \(N\) atoms has \(3N - 6\) normal modes of vibration (linear molecules have \(3N - 5\) modes). For example, water (H<sub>2</sub>O) has:
      </p>

      <div class="equation-block">
        <span class="equation-number">(5)</span>
        $$\text{Normal modes} = 3N - 6 = 3(3) - 6 = 3$$
      </div>

      <p>
        The three vibrational modes of water are: symmetric stretch (\(\nu_1\)), asymmetric stretch (\(\nu_3\)), and bending (\(\nu_2\)).
      </p>

      <p>
        Let's visualize a simulated IR spectrum showing these characteristic peaks:
      </p>

      <div class="plot-container">
        <div class="plot-title">Figure 2: Simulated IR Spectrum of a Carbonyl Compound</div>
        <div id="ir-spectrum-plot"></div>
        <div class="plot-caption">
          Simulated IR spectrum showing characteristic C=O stretch around 1720 cm<sup>-1</sup> and C–H stretches around 2900 cm<sup>-1</sup>.
        </div>
      </div>

      <script>
        // Generate simulated IR spectrum data
        function gaussian(x, center, height, width) {
          return height * Math.exp(-Math.pow(x - center, 2) / (2 * width * width));
        }

        const wavenumbers = [];
        const transmittance = [];
        
        for (let w = 500; w <= 4000; w += 5) {
          wavenumbers.push(w);
          let t = 100; // Start at 100% transmittance
          
          // C-H stretches (alkane)
          t -= gaussian(w, 2920, 35, 30);
          t -= gaussian(w, 2850, 30, 25);
          
          // C=O stretch (strong)
          t -= gaussian(w, 1720, 75, 25);
          
          // C-O stretch
          t -= gaussian(w, 1200, 45, 35);
          
          // Fingerprint region (complex)
          t -= gaussian(w, 1450, 25, 20);
          t -= gaussian(w, 1380, 20, 15);
          t -= gaussian(w, 900, 30, 25);
          
          transmittance.push(Math.max(0, t));
        }

        const irTrace = {
          x: wavenumbers,
          y: transmittance,
          type: 'scatter',
          mode: 'lines',
          fill: 'tozeroy',
          fillcolor: 'rgba(59, 130, 246, 0.2)',
          line: {
            color: 'rgb(59, 130, 246)',
            width: 2
          },
          hovertemplate: 'Wavenumber: %{x} cm⁻¹<br>Transmittance: %{y:.1f}%<extra></extra>'
        };

        const irLayout = {
          xaxis: {
            title: 'Wavenumber (cm⁻¹)',
            autorange: 'reversed',  // IR spectra are typically displayed reversed
            gridcolor: 'rgba(200, 200, 200, 0.3)'
          },
          yaxis: {
            title: 'Transmittance (%)',
            range: [0, 105],
            gridcolor: 'rgba(200, 200, 200, 0.3)'
          },
          plot_bgcolor: 'rgba(0,0,0,0)',
          paper_bgcolor: 'rgba(0,0,0,0)',
          font: {
            family: 'inherit'
          },
          showlegend: false,
          margin: {l: 60, r: 30, t: 30, b: 60},
          annotations: [
            {
              x: 1720,
              y: 20,
              xref: 'x',
              yref: 'y',
              text: 'C=O',
              showarrow: true,
              arrowhead: 2,
              ax: 0,
              ay: -40
            },
            {
              x: 2920,
              y: 60,
              xref: 'x',
              yref: 'y',
              text: 'C–H',
              showarrow: true,
              arrowhead: 2,
              ax: 0,
              ay: -40
            }
          ]
        };

        const irConfig = {
          responsive: true,
          displayModeBar: true,
          displaylogo: false,
          modeBarButtonsToRemove: ['lasso2d', 'select2d']
        };

        Plotly.newPlot('ir-spectrum-plot', [irTrace], irLayout, irConfig);
      </script>

      <h3>Comparison of Spectroscopic Techniques</h3>

      <table class="scientific-table">
        <caption>Table 2: Comparison of Common Spectroscopic Methods</caption>
        <thead>
          <tr>
            <th>Technique</th>
            <th>Energy Range</th>
            <th>Information Provided</th>
            <th>Transitions</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>UV-Visible</td>
            <td>200–800 nm</td>
            <td>Electronic structure, conjugation</td>
            <td>Electronic (π → π*, n → π*)</td>
          </tr>
          <tr>
            <td>Infrared (IR)</td>
            <td>2.5–25 μm</td>
            <td>Functional groups, bonding</td>
            <td>Vibrational</td>
          </tr>
          <tr>
            <td>Raman</td>
            <td>Visible laser</td>
            <td>Symmetric vibrations, complementary to IR</td>
            <td>Vibrational (different selection rules)</td>
          </tr>
          <tr>
            <td>NMR</td>
            <td>Radio frequency</td>
            <td>Molecular structure, connectivity</td>
            <td>Nuclear spin</td>
          </tr>
          <tr>
            <td>Mass Spec</td>
            <td>—</td>
            <td>Molecular weight, fragmentation</td>
            <td>Ionization</td>
          </tr>
        </tbody>
      </table>

      <p>
        Understanding these techniques and their complementary nature is essential for complete structural elucidation of organic compounds.
      </p>

    </article>
  </main>
</div>