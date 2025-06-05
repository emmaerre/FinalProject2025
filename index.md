---
layout: default
title: Home
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs.  We recommend including a README, or a file with information about your project.

# Enriching ArCo: Knowledge Graph Enhancement through LLMs | Exploring musical instrument and semantic gaps in Cultural Heritage data.


This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## About the project

This project explores how SPARQL, RDF modeling, and Large Language Models (LLMs) can be combined to enrich the [ArCo Knowledge Graph](https://dati.beniculturali.it/arco/), focusing on musical instruments, particularly the trombone.

We applied a variety of prompting techniques—including zero-shot, few-shot, and chain-of-thought (CoT) prompting—to guide LLMs in producing useful, ontology-compliant triples and structured suggestions for data enrichment.

## Key objectives 

* Identify and investigate semantic **gaps** in ArCo’s [Music Heritage section](https://dati.beniculturali.it/arco/resource/MusicHeritage)   
* **Enrich** instrument entries (like the trombone) with missing classifications, construction techniques, and semantic metadata   
* Employ [LLMs](https://en.wikipedia.org/wiki/Large_language_model) to support and automate **RDF** generation    
*	Demonstrate the value of Chain-of-Thought (CoT) prompting in complex cultural data reasoning      
*	Evaluate limitations when suggested entities are not represented in the knowledge graph   

## Technologies and techniques 

*	[SPARQL](https://dati.cultura.gov.it/sparql) + [YASGUI](https://yasgui.org/)
*	RDF / OWL
*	Prompting with [ChatGPT](https://chatgpt.com/g/g-8i7WASBxj-home), [Gemini](https://gemini.google.com/app?hl=it), [DeepSeek](https://www.deepseek.com/en)
   -	Few-shot prompting for RDF triple generation
   -	Zero-shot prompting for idea discovery
   -	Chain-of-Thought (CoT) prompting for structured reasoning
*	[ArCo Ontology](https://dati.beniculturali.it/lode/extract?lang=it&url=https://raw.githubusercontent.com/ICCD-MiBACT/ArCo/master/ArCo-release/ontologie/arco/arco.owl)

## Case Studies

We enriched two trombones -one by Ruggero Cesare, the other by Leopold Uhlmann— both underrepresented in the original KG structure.

* [Ruggero Cesare’s Trombone](https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556869.html)
* [Leopold Uhlmann’s Trombone](https://dati.beniculturali.it/lodview-arco/resource/HistoricOrArtisticProperty/1500556890.html)

These instruments were enhanced with:
*	Explicit classification under musical instrument-related classes
*	Construction metadata (e.g., saldatura, rivestimento)
*	Additional semantic properties based on LLM-guided suggestions

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
