---
layout: default
title: Methodology  
---

<h1>Comparison of LLMs</h1>
We observed the following differences in behavior among the LLMs used:

<ul>
  <li><a href="https://chatgpt.com/g/g-8i7WASBxj-home">ChatGPT</a> consistently delivered the most context-aware and ontology-compliant results. When using chain-of-thought prompting, it was especially useful in proposing structured and detailed triples, backed by reasoning. It also provided relevant enrichment suggestions grounded in the vocabulary of ArCo.</li>
  <li><a href="https://gemini.google.com/app?hl=it">Gemini</a> (by Google) performed reliably when given clear examples (few-shot prompting), but its outputs were often syntactically correct but semantically shallow, lacking explanation or deeper contextual understanding.</li>
  <li><a href="https://www.deepseek.com/en">DeepSeek</a> produced results comparable to Gemini but occasionally struggled with ontology-specific terms and sometimes returned incomplete triples or vague responses.</li>
</ul>

Ultimately, <a href="https://chatgpt.com/g/g-8i7WASBxj-home">ChatGPT</a> emerged as the most effective LLM for generating RDF triples and identifying valuable enrichment paths in the ArCo KG, particularly when using chain-of-thought and few-shot prompting. However, using multiple models provided a useful comparative perspective and reinforced the importance of prompt engineering and critical evaluation of LLM-generated content.

This project demonstrated how the combined use of SPARQL querying, knowledge graph ontology exploration, and LLM-driven knowledge generation can identify and address semantic gaps in cultural heritage datasets. It also highlighted some of the current limitations in both KGs and LLMs—especially in cases where certain real-world entities (like other members of the Uhlmann family) were not represented and could not be automatically integrated.
Our experience reinforces the potential of integrating KGs and LLMs in digital humanities, while also underlining the importance of human validation and domain expertise in curating and extending cultural knowledge representations.
