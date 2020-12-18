---
draft: true
slides: ""
url_pdf: ""
title: Do evolutionary rates of antibiotic targets shift as a consequence of
  antibiotic evolution?
subtitle: "Hypothesis: The selective pressures on antibiotic targets change in
  response to the evolution of natural antibiotics. Here I propose that we can
  measure these shifts on phylogenies of antibiotic targets by measuring the
  relative change in substitution rates before and after the origin of genes
  responsible for the biosynthesis of antibiotics present in biosynthetic gene
  clusters (BGC)."
date: 2020-12-18T04:54:17.283Z
summary: This project aims to determine the direction of the changes in
  substitution rates of antibiotic targets as a response to the evolution of
  naturally occurring antibiotics.
url_video: ""
featured: true
external_link: Molecular Evolution
url_slides: ""
tags:
  - Molecular Evolution
  - Antibiotic Resistance
  - Antibiotic Targets
  - Selection Tests
links: null
image:
  caption: A drug bound to the binding site of its molecular target.
  focal_point: Smart
  filename: featured.jpg
  preview_only: true
url_code: ""
---
## Rationale, and significance.

Questions: Does the introduction of naturally occurring antibiotics in the environment change the substitution rate of the antibiotics' targets? What are the forces affecting the evolution of antibiotic targets in bacteria?

Multidisciplinary efforts in the biological sciences have led to the identification of many antibiotic targets, many of which are enzymes involved in cell wall biosynthesis, cell membrane biosynthesis, translation, DNA duplication, among other cellular processes. The evolution of these protein targets is shaped by factors such as drift, positive and purifying selection, factors that have imprinted their action during billions of years in these sequences, and whose relative strength can be quantified (Mortimer et al., 2018). Understanding the evolutionary dynamics of these protein targets can elucidate the evolutionary forces that have shaped target evolution as a result of the use of antibiotics during long evolutionary periods.

Antibiotics are a subset of physiologically active compounds loosely referred to as drugs. The number of drug targets among all classes of approved therapeutic drugs was around 900 in 2017, 190 of them being pathogen targets (Santos et al., 2017). Typically, many antibiotic targets are essential proteins in the cell, and their inhibition can cause important deleterious effects (de Lima et al., 2012). Essential proteins are evolutionarily constrained by purifying selection, this means that mutations in these loci can have big fitness effects, a characteristic that has been quantified using dN/dS ratios. Antibiotic targets are even more constrained than non-target essential genes, and the genome average constraint level (Gladki et al., 2013). This level of constraint in antibacterial targets is ancient, since both dN/dS and pN/pS ratios, which measure purifying selection respectively at the interspecies and intraspecific levels are small (Gladki et al., 2013). In both cases, lower substitution rates with respect to essential genes, suggests strong purifying selection acting over a long evolutionary time. Gladki et al. summarize the pN/pS ratios for known drug targets in bacteria, such as the aminoglycosides that inhibit protein synthesis by binding the ribosomal subunits, or the quinolones that are a group of compounds that inhibit bacteria topoisomerases such as gyrase B. Please notice that gyrB is the target of the aminocoumarins, which is the other antibiotic class studied in chapter 1.

Previously, rates haven't been measured for target proteins separately for different types of cells. However, the set of possible explanations for the low rate of target evolution may differ depending on whether that cell produces the antibiotic, is targeted by the antibiotic and is non-resistant, or is targeted by the antibiotic and is resistant. We expect:

1- a low rate in all cells if target proteins are under strong purifying selection for their native function. This strong purifying selection is what makes them good antibiotic targets, because there are few escape routes (i.e. resistance mutations which also maintain function) (Searls, 2003). This is in contrast to less constrained proteins that are potential targets, but they are able to quickly develop resistance, and any antibiotic becomes ineffective, and therefore there is no long-term fitness advantage to the antibiotic producing organism.

2- a low rate in antibiotic-producing cells and resistant target cells if the removal of target protein variants that are susceptible to the drug results in strong purifying selection.

in contrast we expect:

3- a high rate in all cells, if an arms race exists between the evolution of resistance and the evolution of new antibiotic variants; this would result in positive Darwinian selection (Farhat et al., 2013).

Expectations #2 and #3 invoke co-evolution between antibiotics and their targets via specific modifications that respectively improve or impede the action of the compound.

There is a general assumption in the literature that antibiotic targets with lower substitution rates are more constrained in their relative evolvability for antibiotic resistance via amino acid substitutions, which makes them attractive for the development of drugs (Gladki et al., 2013; Searls, 2003). This constraint  is assumed to be due to purifying selection on the native function of the target (#1, above). However, a significant limitation of these studies is that they conflate substitution rates of antibiotic targets before and after the evolution of the antibiotic, and thus no study has distinguished between expectations #1-3. As others have, I also hypothesize that super-constrained proteins do make the best antibiotic targets; but to test this I propose to examine whether these proteins were among the slowest evolving before the evolution of the targeting antibiotic.

If expectations 2 and 3 are valid, then target protein evolutionary rate is influenced by the advent of the antibiotic system. Although the question on how antibiotic evolution affects target evolution is of central importance, it has not been addressed yet.

I hypothesize that the evolutionary novelty of an antibiotic compound may result in changes in substitution rates of targets over evolutionary time in two different ways. (A) Purifying selection causes the removal of variants that are not able to face the chemical challenge and would result in a reduction in dN/dS (expectation 2). (B) Positive selection would act on drug targets with substitutions that confer resistance; this would result in an increase in the dN/dS (expectation 3). These two processes would result in a shift in the substitution rate of the targets after the origin of the antibiotic, suggesting that the evolutionary forces acting on these targets changed as a result of antibiotic evolution. In this chapter, I propose to test the hypothesis that antibiotic targets have different substitution rates before and after the evolution of antibiotics. To do so, I will use the dating estimates generated in chapter 1, and test for shifts in substitution rates along branches in target phylogenies with respect to these events.

To test whether these differences in rates are significant I will compare them with different null models that assume a single substitution ratio, or a free ratio model, using likelihood ratio tests. Additionally, I will compare these genes to other essential genes that are not known to be targeted by antibiotics as my control group. I hypothesize also that the shifts in evolutionary rates may depend on factors such as subcellular location and protein structure, and although I won’t test these hypotheses here I have discussed their implications in the expected challenges section.