---
layout: default
title: Methodology  
---

# Methodology 

Our methodological approach combines traditional SPARQL-based Knowledge Graph exploration with the generative capabilities of [Large Language Models](https://en.wikipedia.org/wiki/Large_language_model) (LLMs), aiming to identify and fill semantic and structural gaps in the [ArCo](http://wit.istc.cnr.it/arco) dataset. The process unfolds across four main phases, each targeting a specific aspect of enrichment. While each step is presented in detail in the dedicated sections, below is a brief overview of the main phases that structured our work:

1. **Gap Identification and Knowledge Graph Exploration**
We explored the ArCo Knowledge Graph to detect missing or underrepresented musical instruments, notably identifying the absence of the trombone within specific ontology classes.

2. **Triple Construction for Missing Classification**
Upon confirming the gap, we created RDF triples to formally link trombones to the appropriate classification within the knowledge graph.

3. **Triple Construction for Construction Techniques and Family Relations**
We further enriched the trombones’ descriptions by adding technical construction details and investigating the presence of related instrument makers.

4. **Triple Construction for Semantic Linking with Hornbostel-Sachs Classification**
Finally, we enhanced the semantic metadata by associating the trombones with the Hornbostel-Sachs classification system, aligning them with an internationally recognized taxonomy.

<div class="step-menu">
  <button onclick="showStep('step1')">Step 1</button>
  <button onclick="showStep('step2')">Step 2</button>
  <button onclick="showStep('step3')">Step 3</button>
  <button onclick="showStep('step4')">Step 4</button>
</div>

<div id="step1" class="step-content">
  
  <h2>Step 1</h2>
  <p>

<h3>Gap Identification and Knowledge Graph Exploration</h3>

We began our project by exploring the <a href="http://wit.istc.cnr.it/arco">ArCo</a> Knowledge Graph, focusing on the <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">Music Heritage</a> section. Our goal was to identify musical instruments documented within the dataset and to investigate whether certain instruments were missing or underrepresented.

<h4>Initial query - listing musical instrument</h4>

Our first <a href="https://dati.cultura.gov.it/sparql">SPARQL</a> query aimed to retrieve all distinct musical instruments classified under the <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">arco:MusicHeritage</a> class, along with their labels:

<img src="img1" alt="img1">


</p>
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



