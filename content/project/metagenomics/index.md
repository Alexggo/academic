---
draft: true
slides: ""
url_pdf: ""
title: What is the natural reservoir of Candida auris and history of multidrug
  resistance? Exploring the natural history of C. auris using a bioinformatics
  approach.
subtitle: "Hypothesis: Candida auris, a pathogenic fungus that was first
  identified in 1996, has an avian host that is its natural reservoir in the
  wild. I will evaluate this hypothesis by using a computational approach
  searching for contaminant DNA sequences in published RNA-seq studies on SRA
  and using a metagenomics pipeline."
date: 2020-12-18T05:05:25.940Z
summary: ""
url_video: ""
featured: true
external_link: Metagenomics
url_slides: ""
tags:
  - Pathogen Evolution
  - Zoonotic Disease
  - Bioinformatics
links: null
image:
  caption: "Hypothesis of the origin and spread of Candida auris from rural to
    urban environments. source: Casadevall, 2019."
  focal_point: Smart
  filename: featured.jpg
  preview_only: true
url_code: ""
---
## Background, and rationale.

Question: What is the natural reservoir of Candida auris?

Candida auris is one of the few species of fungi that cause candidiasis in humans. This pathogen commonly affects patients with weakened immune systems that get infected during hospital stays. The treatment of this infection is complicated, mainly because many isolates of C. auris are multidrug resistant, meaning that they can survive to the main classes of antifungals such as azoles, amphotericin B and echinocandins. In addition to this, C. auris is capable of surviving on surfaces for long periods of time. Although C. auris is a very serious risk for human health, little is known about the ecology of this organism. Some questions that remain elusive include: (1) where does it come from? (2) when did it originate? and (3) does it have a secondary host? I will address these questions in this chapter by collecting DNA data available in public repositories.

Human infections caused by C. auris have only been reported recently. For example, the first clinical isolate was detected in Japan in 2009, and other cases were consequently identified in South Korea (2011), India (2011), Europe (2016), and other regions. However, resequencing studies of previous cultures have shown that a sample from 1996 in Korea may be the first known case of C. auris ever isolated. The reasons for the recent detection of this organism remain unknown.

The genus Candida is a polyphyletic clade with more than 500 species, such as C. albicans or C. parasitosis, which are part of the Debaryomycetacae family. C. auris is in the Clavispora clade of the Metschnikowiaceae family, being a close relative of C. haemulonii, C. pseudohaemulonii, C. duobushaemulonii and C. lusitaniae (Fig. 7A). These species are predominantly isolated from non-human samples, which might be the reason why C. auris was not identified until 1996, when the first cases appeared in hospitals. These fungal species have been isolated from plant and marine samples, and some from human infections (Jackson et al., 2019). However, C. auris isolates are only found in humans or in clinical environments such as hospitals. It is likely that C. auris was a non-pathogenic fungus present in the environment that recently became pathogenic. If so, finding isolates of C. auris in non-clinical settings may be of great epidemiological interest, since this can inform us on the life history of the species, and on when and how this pathogen expanded, became a pathogen, or developed drug resistance.

Phylogenetic analysis of C. auris isolates shows that there are four genetically different clades of C. auris (Lockhart, 2017), whose origin correspond to different global regions: clade I (South Asia), clade II (East Asia), clade III (South Africa) and clade IV (South America).  Similarly, molecular dating (Fig. 7B) suggests that clade IV originated more recently (TMRCA 1984; 95% HPD 1982-1988), followed by clade I (TMRCA 1878; 95% HPD 1870-1887), clade III (TMRCA 1844; 95% HPD 1832-1855), and clade II (TMRCA 1679; 95% HPD 1663-1698). However, the dates for clades I and III were impacted by the inclusion of divergent strains that don’t have ERG11 resistance mutations. Excluding these outliers, the dating for clades I (1984) and III (1985) are more like clade IV (1984). This suggests a recent expansion and diversification within each of the clades and a much older separation event of the four clades around 22000 (Chow et al., 2020). Although, the cause for this recent expansion of Candida auris is currently unknown.

 The simultaneous origin of C. auris in different regions of the world has led to some speculation about its origin. It has been suggested that its tolerance to high temperatures, which is much higher than other fungi in the same family, is an indicator of a possible secondary host. For example, the optimum growth temperatures of fungi like Saccharomyces cerevisiae is 21-27C, a temperature like other fungi of Metschnikowiaceae family. In contrast, C. auris can grow at temperatures as high as 42C, and it's capable of surviving the basal temperature of the human body. Additionally, C. auris can survive conditions several fold saltier than the ocean and it is well adapted to survive dry environmental conditions during weeks, a unique trait that differs from its relatives. This could make it more suitable for saline environments like desert lakes, tidal pools or very salty regions of the human skin, such as axilla and groin (Jackson, 2019). These unique properties as well as the simultaneous origin of C. auris has been suggested to be the result of adaptations to warmer global temperatures (Casadevall, 2019), followed by changes in C. auris ecological niches that resulted in the fungi being into greater contact with susceptible humans, and consequently changing its distribution from remote rural areas into urban centers, where cases started to be identified. In addition to this, its high thermotolerance gives C. auris the advantage to survive the high basal temperatures of mammals and birds, which act as a barrier to fungal infection in these animal groups, suggesting that C. auris may have an avian reservoir (Casadevall, 2019), since bird body temperatures range between 40-42C and other Candida sp. are commonly found in avian hosts (Al-Yasiri et al., 2016).

The avian hypothesis has not been directly tested and it remains speculative. Here, I propose to test this hypothesis by  searching for contaminant DNA of C. auris that might have been amplified and stored on NGS databases, many of which have been produced by different initiatives such as the Earth Microbiome Project or the Global Ocean Sampling Expedition. I also propose to investigate the source of C. auris in samples whose origin might be agricultural, zoonotic, aquatic, terrestrial, clinical, etc. Thus, this could be an important first step to show hints of its origin that could be further confirmed by sequencing in future research.

Metagenomics and metatranscriptomics identification methods capable of detecting DNA in bulk can bypass the limitations of amplicon-based sequencing and can detect residual eukaryotic DNA from organisms like C. auris. Some of these methods such as Kraken, MEGAN or more recently CCMetagen, have been released to explore microbial diversity from DNA samples. These classifiers assign a taxonomic label to short reads by calculating the lowest common ancestor of the sequences. In particular, CCMetagen appears to be the most appropriate to find C. auris, since it outperforms Kraken in detecting eukaryotic samples at the species level (Marcelino et al., 2020).

Results 'hidden' in published analyses suggest C. auris is indeed in birds, and that more samples ready for analysis remain to be identified. Interestingly, the dataset to evaluate CCMetagen has reported the presence of C. auris in birds (Fig. 8), this was done reanalyzing an SRA samples from four Anseriformes (waterfowl) and Charadriiformes (shorebird) sampled in temperate and arid Australia, being this the first instance where C. auris has been reported in a bird sample. Although preliminary, this finding is also consistent with C. auris’s high tolerance for warm and salty conditions.

This analysis was performed on a small subset of birds and it was not the author’s intention to determine the origin of C. auris, and the significance of this serendipitous discovery might have been overlooked. My intention for this chapter is to expand this analysis to birds and other vertebrates in order to explore the geographic, phylogenetic and ecological diversity of Candida auris in the wild.