Human TCR alpha and beta RNA-based 5’-RACE protocol with unique molecular identifiers (UMI)
==========================================================================================

## PROCEDURE
**CRITICAL STEP:** Perform cell isolation, RNA purification, cDNA synthesis and 1st PCR preparation steps in the 
separate clean work places. General recommendation to lower the risk of RNA degradation and contamination should be carried
out: (labcoats, gloves, tips with aerosol filters, certified RNAse/DNAse free reagents, performing of non-template control
reaction).

### Contents:
1. [Preparing starting material – cell purification.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#preparing-starting-material--cell-purification-timing-25-hours) **Timing** ~2.5 h
2. [Preparing starting material – total RNA. ](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#preparing-starting-material--total-rna-timing-05-hour) **Timing** ~0.5 h
3. [cDNA synthesis with template switch.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#cdna-synthesis-with-template-switch-timing-2-hours) **Timing** ~2 h
4. [First PCR amplification.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#first-pcr-amplification-timing-2-hours) **Timing** ~2 h
5. [Second PCR amplification.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#second-pcr-amplification-timing-2-hours) **Timing** ~1 h
6. [Anticipated result.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#anticipated-result) 
7. [Sequencing library preparation.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#sequencing-library-preparation) **Timing** ~2 h
8. [Sequencing.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#sequencing) **Timing** variable
9. [Oligonucleotides table.](https://github.com/repseqio/protocols/blob/4b3762321e00bc18e8479719c6b98f87f38a145f/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#table-1-oligonucleotides)


#### Preparing starting material – cell purification. Timing ~2.5 hours.
**1|** Perform isolation of mononuclear cells from whole blood using [Ficoll Paque density gradient centrifugation](https://github.com/repseqio/protocols/blob/master/MNCs%20extraction%20using%20SepMate%E2%84%A2%20(Stemcell)%20tubes.md#extraction-of-mononuclear-cells-mncs-from-periferal-blood) or 
lymphocyte extraction from tissue specimen.

**2|** Purify T cells subset of interest using magnetic separation or fluorescence-activated cell sorting.

**CRITICAL STEP:** TCR cDNA libraries can be generated starting from RNA isolated from total leukocytes, PBMCs or any tissue containing T cells. 

**CRITICAL STEP:** Control for the counts of purified T cells of interest is desirable in order to manage the amount
of input cells and RNA material.  

**CRITICAL STEP:** If using fluorescence-activated cell sorting for purifying limited number of cells, direct sorting
into lysis buffer from RNA isolation kit is recommended (RLT buffer, Qiagen). The cells are lysed immediately
in the collection tube and the mRNA is protected from degradation.

**CRITICAL STEP:** It is preferable to use freshly isolated cell sample for RNA purification. In the case of frozen 
samples, culture thawed cells overnight in RPMI-1640 supplemented with 10% human serum.


#### Preparing starting material – total RNA. Timing ~0.5 hour.
**3|** Use column-based RNA isolation method, for example, [RNeasy Micro kit (QIAGEN)](https://www.qiagen.com/ru/shop/sample-technologies/rna/rna-preparation/rneasy-micro-kit#orderinginformation).
Verified minimal number of cells for the protocol is *500 T cells sorted directly in RLT buffer of RNeasy Micro kit*.

**CRITICAL STEP:** Large amounts of gDNA significantly affect cDNA synthesis. For large numbers of cells (>200,000 cells), when using column-based RNA extraction method, DNAse treatment is strongly recommended for large numbers of cells.

**PAUSE POINT:** Cellular lysate in RLT buffer (QIAGEN) can be stored at -70ºC for at least a month. Works even for low cell counts.

**4|** Optionally: verify RNA quantity and quality, e.g. using Agilent Bioanalyzer or gel electrophoresis. RNA Integrity 
Number > 7, or correct 28S rRNA:18S rRNA ratio (around 1.5-2.5:1) and a low number of shadow bands above and below 18S
band are indicative of high quality RNA. 

**CRITICAL STEP:** High RNA quality is critical for the efficient library preparation.

**PAUSE POINT:** RNA can be stored in 75% ethanol at least 1 year at -20°C, or at least 1 week at 4°C. For small RNA
amounts, it is better to start cDNA synthesis immediately after RNA extraction.

#### cDNA synthesis with template switch. Timing ~2 hours.

In case of QIAGEN column RNAeasy MinElute isolation - recommended for less than 100 000 cells - which is a more common case, the minimal final RNA volume is ~10 µl (using 12 μl elution buffer). Hence, two cDNA synthesis can be used to proceed the whole sample (5 µl of RNA in one reaction). 

**5|** In a sterile thin-walled 0.2 ml reaction tube, mix the following reagents in a final volume of 20 μl.

| Component | Amount, μl | Final concentration* |
| --------- | ----------- | ------------------- |
| First Strand Buffer (5x, Clontech) | 4 | 1x |
| DTT (20 mM) | 2 | 2 mM |
|dNTP solution (10 mM each) | 2 | 1 mM each |
| cDNA synthesis primer mix**: ACR_st4 (10 μM), BCR4short (10 μM) | 2 | 1 μM for each primer |
| 5’-template switch adapter (10 μM) | 2 | 1 μM |
| SMARTScribe Reverse Transcriptase (10x, Clontech) | 2 | 10 U/µl |
| rRNasin | 1 | 0,4 U/µl |
| RNA | 1-5 | Up to 500 ng per reaction |
| mQ | 0-4  | |

\* Final concentration refers to concentration in 20 μl following addition of mix.

\** see [**Table 1**](https://github.com/repseqio/protocols/blob/master/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#table-1-oligonucleotides) for primers mixes. 

**CRITICAL STEP:** Preferably, *use most or all RNA extracted from sample of interest.* At a later stage (step 9), 
a portion of obtained cDNA may be used in order to achieve desirable coverage in terms of sequencing reads per UMI (cDNA). High coverage (>5 reads per UMI) allows to correct errors using UMI logic only, without following frequency-based correction of PCR errors. 

**6|** Place the reaction tube(s) into a thermal cycler and incubate 60 minutes at 42ºC.

**7|** Add 1 μl of Uracyl DNA glycosylase (5U/μl, New England Biolabs) and incubate 40 min at 37ºC. 

**CRITICAL STEP:** Uracyl DNA glycosylase treatment removes residual template switch adapter which is critical for
the accurate labeling of starting cDNA molecules.  

**8|** Purify cDNA using MinElute PCR Purification Kit (Qiagen). During purification, wash twice with PE buffer. 
Elute with 14 μl EB buffer.

**CRITICAL STEP:** Residual quantity of oligonucleotides and enzymes used in the reverse transcription negatively affect
subsequent PCR. Removing of these components provides obtaining of pure final bands and allows to carry out 1st PCR 
in a smaller reaction volume.

**PAUSE POINT:** At this time, purified cDNA can be stored at 4°C overnight. For extended storage (<=1 month), it is 
recommended that the cDNA product be stored at −20°C in the freezer. However, it is safer to proceed with the 1st PCR 
the same or next day without freezing, not to lose the material. With minimal cell counts, safer to proceed the same day.

#### First PCR amplification. Timing ~2 hours.
During optimization of PCR amplification step we have tested several polymerases from different suppliers. The best
result was obtained with Q5 polymerase (NEB, M0491L, 500 units). Alternatively, other polymerase with high fidelity 
and processivity may be used.

Both alpha and beta TCR chains can be amplified in the same first round PCR reaction when sample availability is limited. 
Carry out 21 cycles.

Use proportional number of reaction tubes to amplify required amount of cDNA:
For up to 300 000 cells in initial sample: cDNA synthesis of the sample can be pooled on the single MinElute 
Qiagen column for purification and eluted with 12 μl elution buffer. Take all into the 50 μl of the first round 
PCR reaction.

**9|** In a sterile thin-walled 0.2 ml reaction tube, mix the following reagents in a final volume of 50 μl

| Component | Amount, ul | Final concentration |
| --------- | ---------- | ------------------- |
| 1st strand cDNA | 1-10 μl | |
| Q5 polymerase buffer (5x, NEB) | 10 | 1x |
| dNTP mix (10 mM each) | 1 | 0.2 mM each |
| Forward: M1ss primer | 1 | 0.2 μM |
| Reverse primers mix*: ACR_st1 (10 μM), BC2uniR (10 μM) | 1 | 0.2 μM each |
| Q5 polymerase (NEB) | 0.5 | 0.02 U/µl |
| Nuclease free water | 26.5-35.5 | |

\* see [**Table 1**](https://github.com/repseqio/protocols/blob/master/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#table-1-oligonucleotides) for primers mixes. 

**CRITICAL STEP:** Use proportional number of reaction tubes to amplify required amount of cDNA.

 **10|**  Perform PCR using the following parameters:
 
| Cycle | Denature | Anneal | Extend |
| ----- | -------- | ------ | ------ |
| 1 | 98ºC for 30 s | - | - |
| 21 | 98ºC for 10 s | 55ºC for 10 s | 72ºC for 50 s |
| 1 | - | - | 72ºC for 2 min |

**11|** Combine PCR products that were obtained starting from the same RNA sample and purify using the QIAquick PCR 
purification Kit. During purification, wash twice. Elute purified PCR product in 30 µl of elution buffer.

**PAUSE POINT:** At this time, purified product of the 1st PCR can be stored at 4°C overnight. For extended storage 
(1-2 months), it is recommended that the PCR product be stored at −20°C freezer.
 
#### Second PCR amplification. Timing ~2 hours.
This part of the protocol uses slightly nested reverse constant region primers coupled with added sample barcodes.
The numbers of barcoded sample primers used will need to be adjusted according to the number of samples and each barcode
must be assigned to only one sample amplification. See the end of the protocol for a complete list of synthesized barcoded 
sample primers.

At this point, the samples must be split and processed separately for alpha and beta if 2 primers were combined in cDNA 
synthesis and 1st PCR). Therefore each first round reaction will generate 2 second round PCRs, one for alpha and one for
beta.

**12|** In a sterile thin-walled 0.2 ml reaction tube, mix the following reagents in a final volume of 50 μl

| Component | Amount, ul | Final concentration |
| --------- | ---------- | ------------------- |
| Purified 1st PCR product | 1-2* | |
| Q5 polymerase buffer (5x, NEB) | 10 | 1x |
| dNTP mix (10 mM each) | 1 | 0.2 mM each |
| M1s primer with sample barcode (10 µM) | 1 | 0.2 µM |
| hum bcj_i /hum acj_i primer with sample barcode (10 µM) | 1 | 0.2 µM |
| Q5 polymerase (NEB) | 0.5 | 0.02 U/µl |
| Nuclease free water | 34.5-35.5 | |
 
\*in some cases, dilution of the 1st PCR product may enhance efficiency of the 2nd PCR 

**CRITICAL STEP:** On a single MiSeq/HiSeq run, combine M1s primers with different numbers of random nucleotides at 
the 5’-end for different samples (2, 3, or 4 nt, see [**Table 1**](https://github.com/repseqio/protocols/blob/master/Human%20TCR%20alpha%20and%20beta%20RNA-based%20RACE%20protocol.md#table-1-oligonucleotides)). This provides better diversity generation which is
critical for clusters differentiation by Illumina sequencer.

**13|** Perform PCR using the following parameters:

| Cycle | Denature | Anneal | Extend |
| ----- | -------- | ------ | ------ |
| 1 | 98ºC for 30 s | - | - |
| 9-15 | 98ºC for 10 s | 58ºC for 10 s | 72ºC for 50 s |
| 1 | - | - | 72ºC for 2 min |

**14|** Verify quality and concentration of obtained PCR product by analyzing aliquot of the sample alongside DNA ladder
on agarose gel or Agilent Bioanalyzer.

**CRITICAL STEP:** Visible band (~2 ng/ul) should be normally obtained within 10-16 cycles of second PCR. Absence of visible
band by 18 cycle of 2nd PCR may indicate that less than 1,000 cDNA molecules have entered 1st PCR.

**15|** Purify PCR product using QIAquick PCR purification Kit (or other column based purification system). During 
purification, wash twice.

**CRITICAL STEP:** It is important to purify products of the second PCR within an hour after amplification. Otherwise 
residual enzyme activities may damage the ends of the library that carry sample barcodes required for the data
demultiplexing in further software analysis. Preferably store at +4ºC in the meanwhile.  

**PAUSE POINT:** At this time, purified libraries can be stored at 4°C overnight. For extended storage (up to 1 month),
it is recommended that the PCR product be stored at −20°C freezer before adapter ligation.

#### Anticipated result
Using the protocol provided will typically produce pure PCR band after 21 cycles of first PCR and 10-16 cycles of
second PCR amplification, depending on the cell count, cell integrity, RNA quality, mRNA content in cells, and amounts 
of starting mRNA.

#### Sequencing library preparation 

**16|** For each of the obtained libraries, determine concentration using the QuBit Fluorometer.

**17|** Process libraries for sequencing by pooling before adapter ligation (option A) or after ligation of adapters (option B):

##### A. Pooled adapter ligation
**I.** For a MiSeq run or HiSeq lane, prepare pool of your libraries by combining equal molar or equal volume portion of each individual sample. The resulting amount of pooled PCR products should be at least 300 ng.

**CRITICAL STEP:** We recommend to generate parallel libraries of similar content (e.g., ten samples of 100,000 T cells each) using the same protocol and number of PCR cycles, and further mix the obtained libraries in equal volume proportions. This allows to obtain homogeneous over-sequencing (reads per UMI), which is optimal for further comparative bioinformatic analysis. For example, the library which started from 30,000 T cells may produce more PCR product than one which started from 10,000 T cells after the same number of PCR cycles. However, the former library would also carry proportionally more TCR cDNA molecules, and thus requires more sequencing reads to achieve the comparable UMI coverage.

**II.** Use pooled PCR products from previous step to prepare a sequencing library. Use the NEBNext Ultra DNA library prep kit for Illumina and apply a standard protocol according to the [manufacturer recommendations.](https://www.neb.com/protocols/2014/05/22/protocol-for-use-with-nebnext-ultra-dna-library-prep-kit-for-illumina-e7370)

##### B. Separate adapter ligation 

**I.** Alternatively, prepare separate libraries for each sample. Use the NEBNext Ultra DNA library prep kit for Illumina and apply a standard protocol according to the [manufacturer recommendations.](https://www.neb.com/protocols/2014/05/22/protocol-for-use-with-nebnext-ultra-dna-library-prep-kit-for-illumina-e7370) Use at least 300 ng of each PCR product.

**CRITICAL STEP:** Double-end sample barcoding in the second PCR amplification protects from cross-sample contaminations
during co-amplification of joined PCR-products after adapters ligation. Nevertheless, some minimal cross-sample 
contamination may still occur. In order to provide 100% protection from the cross-sample contaminations, ligation of
Illumina adapters separately to each library is recommended.

**II.** For a MiSeq/HiSeq run, pool libraries of interest with ligated Illumina adapters in equal volumes.

**18|** Purify target library using AMPure XP beads or agarose gel purification. Prepare 2% agarose gel with 1x TBE buffer.
Run the agarose gel electrophoresis at 120V for ~60 minutes. Then excise the gel with amplified libraries in the range
of ~600-750nt (size of amplicons with Illumina adapters is sample dependent).

**CRITICAL STEP:** Even minor amounts of short non-specific products may essentially reduce counts of target sequencing 
reads, since short fragments are much more efficient in solid-phase bridge amplification.

**CRITICAL STEP:** Cut from gel widely, not to lose shortest and longest variants, since the invisible dispersion of TCR 
fragments lengths may be significant.

**CRITICAL STEP:** Cut from gel fast, and use soft UV light, or preferably use Safe Imager and Sybr Green staining, not
to damage the library.

#### Sequencing
**19|**  Spike the library with 20% of PhiX library.

**20|** Analyze the resulting library using paired end Illumina MiSeq or HiSeq2500 sequencing, standard Illumina sequencing 
primers, 150+150 or 200+200 paired end sequencing. 

**CRITICAL STEP:** 150+150 length is sufficient to cover CDR3. However, the longer are the reads, the more accurate is
V gene segment identification afterwards.  

#### Table 1. Oligonucleotides

| Primer | Application | Sequence |
| ------ | ----------- | -------- |
| 1st strand cDNA synthesis |||
| SmartNNNa | 5’ – template switch adapter* | AAGCAGUGGTAUCAACGCAGAGUNNNNUNNNNUNNNNUCTT(rG)4 |
| ACR_st4 | Primer for cDNA synthesis, human TCR alpha chain mRNA, C-region | GTCTAGCACAGTTTTGTC |
| BCR4short | Primer for cDNA synthesis, human TCR beta chain mRNA, C-region | GTATCTGGAGTCATTGA |
| 1st PCR amplification |||
| M1ss | primer, anneals on the switch adapter | AAGCAGTGGTATCAACGCA |
| ACR_st1 | Nested primer, TCR alpha cDNA, C-region | GTCACTGGATTTAGAGTC | 
| BC2uniR | Nested primer, TCR beta cDNA, C-region | TGCTTCTGATGGCTCAAACAC |
| 2nd PCR amplification** |||
| M1s_i | Slightly nested primer, anneals on the switch adapter | (N)2–4(XXXXX)CAGTGGTATCAACGCAGAG |
| Hum acj i | Nested primer, TCR alpha cDNA, C-region | (N)2–4(XXXXX)GGGTCAGGGTTCTGGATAT |
| Hum bcj i | Nested primer, TCR beta cDNA, C-region | (N)2–4(XXXXX)ACACSTTKTTCAGGTCCTC |

\* U=dU. Adapter quality is critical. 

\**(N)2-4  – random nucleotides which introduced at 5’-ends of the final library for better diversity generation and cluster differentiation by Illumina sequencer. XXXXX – sample barcode (numbered as “i” in the primer name), generation of sample barcodes on both sides of the library minimizes cross-sample contamination. 

#### Troubleshooting


| Problem | Possible reason | Possible solution |
| ------- | --------------- | ----------------- |
| gDNA contamination (when using phenol-chloroform extraction method) | Interphase pipetted up with aqueous phase | Do not draw off the entire aqueous phase after phase separation. Perform DNAse treatment. |
| Low RNA yield | Final RNA pellet was incompletely  dissolved | Do not allow the RNA to dry completely after last washing, the pellet can lose solubility. |
| RNA is degraded | Samples were stored too long before processing | Try to process sample immediately after collection |
|  | Isolated RNA were stored at incorrect temperature | Store RNA samples at -20°C and in 75% ethanol |
|  | RNAse contamination | Prepare new solutions of reagents and treat equipment with RNAse decontamination solution (e.g. RNAseZap, Ambion) |
| Agarose gel electrophoresis reveals low concentration of the PCR product or no product | The RNA may contain impurities that inhibit cDNA synthesis | In some cases, ethanol precipitation of RNA can remove impurities. If this does not help, re-isolate the RNA |
|  | PCR undercycling | Subject the samples to two or three additional PCR cycles (plus one extra final extension cycle) and recheck the products |
|  | cDNA synthesis or PCR kit related problems | Use control high-quality RNA extracted from large amounts of T cells or white blood cells to verify kits performance |
| Bands and background smear are very intense | PCR overcycling | Repeat the PCR amplification, using two or three fewer PCR cycles |
| Background smear is intense or short length fragments are visible |  | Purify target library using AMPure XP beads or agarose gel purification |
