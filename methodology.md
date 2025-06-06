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
  <h2>Step 1:Gap Identification and Knowledge Graph Exploration</h2>
  <p>
  We began our project by exploring the <a href="http://wit.istc.cnr.it/arco">ArCo</a> Knowledge Graph, focusing on the <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">Music Heritage</a> section. Our goal was to identify musical instruments documented within the dataset and to investigate whether certain instruments were missing or underrepresented.

<h3>Initial query - listing musical instrument</h3>

Our first <a href="https://dati.cultura.gov.it/sparql">SPARQL</a> query aimed to retrieve all distinct musical instruments classified under the <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">arco:MusicHeritage</a> class, along with their labels:

<img src="./assets/images/img1.png" alt="img1">

This query provided us with a general overview of the musical instruments currently categorized under the Music Heritage class.


<h3>Identifying a gap - missing instrument</h3>

We then formulated a second query to verify whether three specific instruments —trombone, trumpet (“tromba”), and violin (“violino”)— were present in the <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">arco:MusicHeritage</a> class. 
The query used FILTER, REGEX, UNION, and ORDER BY clauses to search for multiple terms simultaneously:

<img src="./assets/images/img2.png" alt="img2">

The results showed that "tromba" and "violino" were both present, but "trombone" returned no matches, indicating a potential gap in the knowledge graph.

To confirm this absence, we executed a focused query that searched only for the term trombone in the same class:

<img src="./assets/images/img3.png" alt="img3">

As expected, the result table was empty, further confirming that the trombone is not represented within the MusicHeritage class:

<img src="./assets/images/img4.png" alt="img4">


<h3>Further investigation - other classes</h3>

We expanded our search to see if the term trombone appeared in other relevant classes. A query on the class <a href="https://w3id.org/arco/ontology/arco/MusicalInstrumentClassification">arco:MusicalInstrumentClassification</a> also returned no results:

<img src="./assets/images/img5.png" alt="img5">

<img src="./assets/images/img6.png" alt="img6">


However, when we queried the more general class <a href="https://w3id.org/arco/ontology/arco/MovableCulturalProperty">arco:MovableCulturalProperty</a>, which is a superclass of <a href="https://w3id.org/arco/ontology/arco/HistoricOrArtisticProperty">arco:HistoricOrArtisticProperty</a>, we successfully found multiple records associated with trombones:

<img src="./assets/images/img7.png" alt="img7">

<img src="./assets/images/img8.png" alt="img8">

Among the results, we selected two specific trombones as case studies for enrichment:
•	<a href="https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556869.html">Ruggero Cesare’s trombone</a> (slide trombone / trombone a coulisse):

<img src="./assets/images/img9.png" alt="img9">

•	<a href="https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556890.html">Leopold Uhlmann’s trombone</a> (slide trombone / trombone a coulisse):

<img src="./assets/images/img10.png" alt="img10">



















  
  
  
  </p>
</div>


<div id="step2" class="step-content" style="display:none;">
  <h2>Step 2</h2>
  <p>Contenuto di Step 2...</p>
</div>


<div id="step3" class="step-content" style="display:none;">
  <h2>Step 3</h2>
  <p>Contenuto di Step 3...</p>
</div>


<div id="step4" class="step-content" style="display:none;">
  <h2>Step 4</h2>
  <p>Contenuto di Step 4...</p>
</div>






















<script>
function showStep(id) {
  document.querySelectorAll('.step-content').forEach(el => el.style.display = 'none');
  document.getElementById(id).style.display = 'block';
}
</script>



