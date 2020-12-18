---
title: "Network Evolution: Is network structure a result of phylogenetics"
summary: This project aims to show evidence that network evolution using drug interaction scores correlates linearly with phylogenetic distance. 
tags:
- Network Biology
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: "A small subset of the Protein-Protein Interaction Network in Saccharomyces cerevisiae. source: Wodak Lab"
  focal_point: Smart

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: 
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Hypothesis: cellular networks diverge with time, and so do drug-drug interaction networks, since these are a proxy to measure network structure. This hypothesis, although apparent, has not been directly tested due to complexities in the measuring procedures of networks. 

### Evolutionary rate is correlated to protein connectivity, where proteins with a larger number of protein-protein contacts evolve at a faster rate than proteins with less. 
Evolutionary rates are correlated with protein connectivity, this link has been shown in yeast protein interaction networks. Proteins involved in a large number of protein connections evolve at a slower rate than proteins that have fewer interactions (Fraser et al. 2002; Fraser and Hirsh 2004). However, this hypothesis has been contested by others (Bloom and Adami 2003; Jordan et al. 2003). 
More recent work done in yeast, worm and fly interactomes supports this hypothesis, by suggesting that proteins that are more central in the network are more essential for survival and have a slower evolutionary rate (Hahn and Kern 2005).

### Molecular networks like Protein-Protein Interaction Networks are being modified by evolutionary forces, through processes like rewiring, loss and gene duplication. 
Molecular networks like cell metabolism, cell signaling or transcription networks are being remodeled and modified by evolutionary forces, in a way new connections are formed and others are being removed. Species more closely related have a more similar network structure than species that are more evolutionarily distant. This has been shown by correlating network topology alignments with phylogenetic alignments.


### Protein-Protein Interaction Networks are not known for many species, but Drug-Drug Interaction Networks might be used as a proxy of network structure. 
Only a few species’ interactomes have been mapped, and the ones that have might not describe fully the network structures of the organisms. Lehar et al, showed that drug-drug interaction scores can be used to predict metabolic structure in Candida albicans. By using a metabolic flux model of ergosterol the biosynthesis pathway, they showed that Bliss score measurements reflect the network or the relation between the targets, such as whether the targets occur in parallel pathways, serially or in other types of assortments. 

### Unsolved question. What metrics of drug-drug interaction high-througput experiments correlate well with phylogenetic distance?
