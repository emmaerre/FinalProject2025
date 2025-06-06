---
layout: default
title: Methodology  
---

# Methodology 

<div class="step-menu">
  <button onclick="showStep('step1')">Step 1</button>
  <button onclick="showStep('step2')">Step 2</button>
</div>

<div id="step1" class="step-content">
  <h2>Step 1</h2>
  <p>Contenuto step 1.</p>
</div>

<div id="step2" class="step-content" style="display:none;">
  <h2>Step 2</h2>
  <p>Contenuto step 2.</p>
</div>

<script>
function showStep(id) {
  document.querySelectorAll('.step-content').forEach(el => el.style.display = 'none');
  document.getElementById(id).style.display = 'block';
}
</script>








Questo è il contenuto della pagina Methodology. Puoi scrivere qui usando Markdown:

- **Elenchi**
- [Link](https://esempio.com)
- ![Immagine](image.png)
![image](https://github.com/user-attachments/assets/52f00910-ca72-47e0-b3d3-9014d5833ccd)
