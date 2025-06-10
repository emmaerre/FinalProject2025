---
layout: default
title: Methodology  
---

<h1>Conclusion</h1>

This project aimed to explore and enrich the <a href="http://wit.istc.cnr.it/arco">ArCo Knowledge Graph</a> by identifying and addressing gaps in its representation of musical instruments, with a focus on the trombone. Using SPARQL queries, we discovered that certain culturally and historically relevant instruments—such as the trombone—were missing from specific classes like <a href="https://w3id.org/arco/ontology/arco/MusicHeritage">MusicHeritage</a> and <a href="https://w3id.org/arco/ontology/arco/MusicalInstrumentClassification">arco:MusicalInstrumentClassification</a>. 
This absence highlighted an opportunity to contribute to the semantic representation of Italian cultural heritage through Linked Open Data.
We selected two case-study instruments —the trombones of <a href="https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556890.html">Leopold Uhlmann</a> and <a href="https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556869.html">Ruggero Cesare</a>— and enriched their RDF descriptions by:

<ul>
  <li>Linking them to the class <a href="https://w3id.org/arco/ontology/arco/MusicalInstrumentClassification">MusicalInstrumentClassification</a>, which previously did not include them
</li>
  <li>Associating them with construction techniques such as <a href="https://dati.beniculturali.it/lodview-arco/resource/TechnicalCharacteristic/saldatura.html">saldatura</a> (welding) and <a href="https://dati.beniculturali.it/lodview-arco/resource/TechnicalCharacteristic/rivestimento.html">rivestimento</a> (coating) from the <a href="https://dati.beniculturali.it/lodview-arco/ontology/denotative-description/TechnicalCharacteristic.html">Technical Characteristics</a> class

</li>
  <li>Connecting them to the <a href="https://w3id.org/arco/ontology/arco/HornbostelSachsClassification">Hornbostel-Sachs classification</a> system and specifying three of its properties: number, definition, and edition
</li>
</ul>

To achieve these tasks, we combined structured <a href="https://dati.cultura.gov.it/sparql">SPARQL</a> querying with the use of <a href="https://en.wikipedia.org/wiki/Large_language_model">Large Language Models</a> (LLMs) to generate RDF triples and suggest semantic relationships. We applied three prompting strategies—zero-shot, few-shot, and chain-of-thought—and experimented with three different LLMs: <a href="https://chatgpt.com/g/g-8i7WASBxj-home">ChatGPT</a>, <a href="https://gemini.google.com/app?hl=it">Gemini</a>, and <a href="https://www.deepseek.com/en">DeepSeek</a>.
