### Notes to be incorporated in to the thesis as and when they strike me.

# Intro:
 - Diagram of PVC 'ownership' by genome (host of hosts)
 - MERV model (poison arrow)
 - Strand exchange
 - Read the new Hurst manuscript from the 16th March '18


# Methods:

# Chapter 1: Structural Bioinformatics
 - Another quote from Silverman2012a: "For the most part, this homology is apparent at the structural level, not at the sequence level"
 - Introduce the chapter by drawing attention to the fact that homology modelling approaches are widely used when structures are absent.
 - Hurst2004 showed that PVC2 is required for formation of the toxic Afp. Yet more evidence that PVC3 is the one that's deleted. May also need to mention this in the Phylogenetics Chapter.
 - Make it plain that because there was so little functional information to go off in the original annotations, re-annotating and querying via HHPred was necessary and useful
 - HHpred results (supplementary table)
 - rmsd vs sequence ID xorrelation
 - DipTest binomial distribution
 - interior charge
   - The Ge et al paper has a similar figure where the electrostatics are very pronounced. Copy this.
   - Process for making inner tube donuts:
     - Open a reference structure (e.g. 3EAA -> NOT THE BIOUNIT)
     - Match structure to reference
     - Apply references sym to the structures (sym #subject group #ref)
       - May need to do this separately for each model, and re-save each donut as a single PDB in order to tile (-> do this by using `combine`, not group)


 - tail fibre (lumt? ligand docking? galactose?)
 - interior volume measurements
 - interior sheath high RMSDs but equivalent space occupation
 - speculation on sheath contractility/defunctness?
 - annotate the hypervariable tail fibre region on the MSA
 - Antigenicity?
 - SSCalc script of tail fibre simulations to see if they match with Dichroweb/PDB2CD predictions.
 - Positive surface charge for resistance to trypsinisation?
 - TopDraw/Pro-origami cartoons?
 - Create script to helically reconstruct the outer sheath
 - Render by conservation versus non-PVC inner and outer sheaths?
 - Check putative PAAR proteins for:
   - >"The cone contains nine short b-strands, three of which create its base and participate in binding to the VgrGb-helix and six others form three b-hairpins that point towards the vertex of the cone, but have different lengths" - from Schneider2013
   - Also look for these residues:
   > "The Zn binding site consists of three histidines and one cysteine—H14, H46, H54 and C81"
   - >"These residues are replaced with similar or complementary metal-binding residues (arginines, lysines and glutamines) in more distant homologues suggesting that they also carry a metal ion roughly at the same position. The metal ion, being a natural ligand for this site, stabilizes the pointed tip of the PAAR domain and is likely to be important for its integrity during penetra- tion of the target cell envelope."

 - Compare sheath proteins to fittings in EM densities for AFP/Pyocin/T4 (demonstrating that the sheath protrusions don't exist)
 - State hypothesis that the inner sheaths of all contractile structures appear well structurally conserved, but the outer sheaths can vary substantially. e.g. T6SS TssBC are not related to T4 gp18
 - Tape measure proteins typically have a high proportion of a-helix. Looks like the simulated structures exhibit this (even if not physilogically relevant structures). Maybe run through SScalc? use dssp to annotate the MSA?
 - Collapsed dataset to the best single models from each operon and locus by RMSD value.
 - Table of 'type 6'-iness, 'T4'-iness, Afp-iness etc.
  - Triangular ggtern-like graph?
 - Use of inner sheath proteins for phylogenetics may not be valid, if they transpire to be specialised basplate adapter proteins etc. They may not be fulfilling the role suspected.


# Chapter 2: Phylogenetics

 - i) Show that PVCs are actually very limited to photorhabdus from the MGB results.

    - Perhaps show a graph of the cumulative blast scores dropping off outside Photo?
    - Show an MGB output dominated by photorhabdus, with the variant forms of the operons in the more distant stuff

 - ii) Be more definitive on the ancient-ness of PVCs vs mobility. Find the paper that agreed they are less mobile (Sarris?)

 - iii) Identify all possible Photorhabdus operons.
 - Note that comparative studies across genera have been done before.
  - Demonstrate that PVCs not widespread on plasmids though.
  - No studies on the microevolution _within_ operons to date (as PVCs are quite unique in having many examples)
  - Little consideration to toxin bearing when others identify loci as 'AFP/PVC like'. Structure is important, but function is the defining characteristic.
  - Compare PVC MultiGeneBlast searches with and without toxins?
 - Hurst2004 paper also shows a characteristic GC trace for these types of structures.
 - Persson2009 -> afp2-4 and afp7 conserved across a number of marine bacteria. Appear essential
 - Sarris2016 -> sheath proteins are phylogenetically distinct, therefore should be considered separately.
 - Add a future study section
   - e.g. would like to fully automate the congruency process
   - would be interesting to create a consensus phylogeny based on more than just a single coat protein


# Chapter 3: Tail
 - Could the dramatic change in secondary structure seen in temperature shifts be a clue to a conformational rearrangement in the tail fibres when transducing a signal?

# Chapter 4: Synthetic and Natural Operon Regulation
 - Construct maps
 - nusG??? Role with High GC content?
 - Shikuma et al speculate on whether an altruistic event, or neutrally lytic, depending on population proportions.
 - Reporter microscopy:
   - Display the 4x4 grids as before
   - Also have some 'blown up' panels which highlight the heterogeneity (e.g. ultra bright cells)
 - Stress response?
   - Elongation of the cells?
   - Crystals forming (phase bright)?

# Misc:
 - MGB parser: check if 2 seqs overlap, if so, take the longest or the intersection of the 2?
 - MGB parser: test for identical sequences, and remove redundancy.
 - MGB parser: compare with Yang's database?
 - MGB parser: Sanity check for hits to yersinia/vibrio seqs etc?


# Discussion:
 - Evidence for convergent evolution rather than direct descension?
   - PVCs functionally resemble Afp, but structurally resemble Pyocins.
   - More ancestral/less mobile than initially suspected.
 - Have shown here that though many things that look like PVCs exist, the 'true' PVCs are very restricted to the 'rhabduses. Serratia has the closest relative, but the 'MRCA' of PVCs and Afps etc must exist somewhere within the split from serratia and photorhabdus
 - Speculate on the role of the ATPase
   - Recycling more efficient than de novo synthesis Kube2015 (and references 12, 61, 76)

---------

## Thesis submission notes from the Graduate School

Thesis Presentation Guidelines:

- A4
- 4cm Left margin + Adequate margins elsewhere for trimming/binding
- Page numbers at least 1.5cm from left hand margin
- 1.5 spacing
- Single sided. 2 sided is permitted for the final library copy.
- Include library declaration
- Not to exceed 70,000 words (excluding appendices, footnotes, tables, bibliography

Title Page:
- Full thesis title (+ subtitle if appropriate)
- Volume number if needed (include current vol number and total vol number)
- Author fullname (qualifications/distinctions optional)
- Full qualification name
- Uni Name/Dept Name/Center name
- Month + Year of Submission

ToC:
- Immediately after Title Page.
- Followed by list of figures/list of tables

Acknowledgements:
- Immediately after list of figs/tables

Declaration:
‘This thesis is submitted to the University of Warwick in support of my application for the degree of Doctor of Philosophy. It has been composed by myself and has not been submitted in any previous application for any degree [(if parts previously used add:) apart from the background material in sections XXX which was previously submitted for YYY degree.]
‘The work presented (including data generated and data analysis) was carried out by the author except in the cases outlined below:
‘List of data provided and/or analysis carried out by collaborators.
‘Parts of this thesis have been published by the author:
‘List of publications including submitted papers.’

Abstract:
 - Max 300 words. No longer than a single A4 side.

Abbreviations:
 - Front or rear of the thesis, but must be indicated in the ToC

Tables and Illustrations:
 - Ideally printed on high quality paper. Copy paper not appropriate.

Research Training:
 - Permitted if deemed appropriate by student + supervisor


Submission guidelines:
 - 2 softbound copies to Graduate School
 - Electronic copies on CD-ROM as a single PDF.
