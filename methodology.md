---
layout: default
title: Methodology  
---

# Methodology 

<div class="step-menu">
  <button onclick="showStep('step1')">Step 1</button>
  <button onclick="showStep('step2')">Step 2</button>
  <button onclick="showStep('step3')">Step 3</button>
  <button onclick="showStep('step4')">Step 4</button>
</div>

<div id="step1" class="step-content">
  <h2>Step 1</h2>
  <p>Contenuto step 1.</p>
</div>

<div id="step2" class="step-content" style="display:none;">
  <h2>Step 2</h2>
  <p>Contenuto step 2.</p>
</div>

<div id="step3" class="step-content" style="display:none;">
  <h2>Step 3</h2>
  <p>Contenuto step 3.</p>
</div>

<div id="step4" class="step-content" style="display:none;">
  <h2>Step 4</h2>
  <p>Contenuto step 4.</p>
</div>

<script>
function showStep(id) {
  document.querySelectorAll('.step-content').forEach(el => el.style.display = 'none');
  document.getElementById(id).style.display = 'block';
}
</script>



