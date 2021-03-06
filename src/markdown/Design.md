
# Project Design

## Prions

Prions are self-perpetuating proteins that have a soluble, normally functional form and an additional insoluble form known as aggregates or amyloids (Tyedmers et.al, 2010). They are self-propagating conformations that have the ability to transmit phenotypes that are not caused by changes in nucleic acid formations (Tyedmers et.al, 2010). The first prions that were discovered were disease-prions, notably in mammalian diseases including sheep scrapie and human Creutzfeldt- Jacob (Liebman & Chernoff, 2012). These diseases were transmitted by infectious conformational isoforms of proteins, which in turn convert other proteins into the isoform (Liebman & Chernoff, 2012). To date, there are over thirty human diseases associated with the formation of prions (Liebman & Chernoff, 2012).

Currently, there are seven-known prions in Saccharomyces cerevisiae, each with a different function and phenotype (Tyedmers et.al, 2010). Although there are no general sequence similarity among all the seven prions, there is a heightened expressed level of asparagine and glutamine residues in all the prions (Tyedmers et.al, 2010).


<br>

## Modularity of Prions



New prion domains and functions and reporters found to make synthetic prions- leading to new natural prions (Wickner et.al, 2000). A hybrid prion protein can be formed by fusing different prion domains into the corresponding protein filaments (Wickner et.al, 2000). However, this hybridization is very selective - as it will not combine with all protein filaments (Wickner et.al, 2000).


<br>

## Reasoning for Usage



By using the self-perpetuating qualities of the prion domain as a tool, alternative forms of various proteins can be induced. This can occur through the enhancement of an existing function, or transferring a new one. Through this mechanism, in future research and applications, isoforms of proteins can be produced and manipulated for the desired effect or product. Applications of this project can be found here.

## The Prion Domain

The prion domain, derived from Sup35 of *S.cerevisiae*, was employed in the design of this project. The utility of Sup35 is based on its ability to manifest in either an infectious or non-infectious state (Dale et al., 2012). In [PSI-], the non-infectious state, the protein acts as a translational termination factor (Dale et al., 2012). In the [PSI+] state, however, the protein confers prion-like properties (Dale et al., 2012)). [PSI+] is often observed upon overexpression of Sup35, which results in protein aggregation (Bradley & Liebman, 2004). Based on the discovery that only the N-terminal and a small portion of the middle domain are essential to the propagation of the prion state, only the coding sequence of the first 137 amino acids was incorporated into the plasmid design (Bradley & Liebman, 2004). Decreasing the size of the plasmid was expected to aid in plasmid construction and transformation. This prion domain is referred to as “PrD”. As we wanted the prion domain to be a modular tool, we created a biobrick and placed it in the registry ([BBa_K2475000](http://parts.igem.org/Part:BBa_K2475000)).

## Bimolecular Fluorescence Complementation (BiFC)

BiFC is employed as a means to visualize protein interactions within live yeast cells. The method is based upon the principle that fragments of a fluorescent protein do not have the ability to fluoresce without interacting with one another in the form of a complex (Kerppola, 2008). In applying this principle to our project, the objective was to utilize the prion domain as a tool to give rise to functional proteins. The interaction of the N-terminal of YFP fused with PrD ([BBa_K2475003](http://parts.igem.org/Part:BBa_K2475003)) and the C-terminal of YFP fused with PrD ([BBa_K2475004](http://parts.igem.org/Part:BBa_K2475004) ) is expected to result in the emission of fluorescence when both split proteins come into close proximity in an aggregate.

<center>
![BiFC]({{image "bifc" "directlink" mode}})
</center>

## Fluorescence Resonance Energy Transfer (FRET)

FRET represents another method to visualize intracellular interactions. The premise underlying this technique is that the transfer of energy from excited fluorophores to non-excited fluorophores can occur when the two fluorophores are within a distance of 5 nm (Alberts et al., 2015). Labelling molecules of interest with different fluorophores enables the recognition of instances when they are at such close proximity, which typically only occurs when the molecules are interacting (Alberts et al., 2015). In order for the energy transfer to occur, the excitation spectrum of one fluorophore must overlap with the emission spectrum of another (Alberts et al., 2015). In this project, the excitation of cyan fluorescent protein (CFP) at approximately 430 nm will result in emission from yellow fluorescent protein (YFP) at approximately 535 nm if the associated prion domain is successful in increasing the interactive potential of the fluorophores (Alberts et al., 2015). FRET, as a part of this project design, is expected to demonstrate the ability of prion domains to bring together different proteins in an attempt to manipulate cellular processes. [PrD CFP](http://parts.igem.org/Part:BBa_K2475001) and [PrD YFP]( http://parts.igem.org/Part:BBa_K2475002 ) have been biobricked and placed in the registry.

<center>
![FRET]({{image "fret" "directlink" mode}})
</center>

## Experimental Plan


1. **Design** parts and primers for IDT synthesis

2. **PCR** amplify ordered parts

3. **Clone** into *E. coli*

4. **Isolate** cloned plasmid

5. **Transform** into Yeast

6. **Observe** engineered proteins in the aggregated form



## References

Alberts, B., Johnson, A., Lewis, J., Morgan, D., Raff, M., Roberts, K., & Walter, P. (2015). Ways of Working with Cells. In Molecular Biology of the Cell (6th ed., pp. 543-544). New York, NY: Garland Science.

2. Bradley, M. E., & Liebman, S. W. (2004). The Sup35 domains required for maintenance of weak, strong or undifferentiated yeast [PSI ] prions. Molecular Microbiology,51(6), 1649-1659. doi:10.1111/j.1365-
2958.2003.03955.x

3. Dale, J. W., Schantz, M. V., & Plant, N. (2012). Products from Native and Manipulated Cloned Genes. In From Genes to Genomes (3rd ed., p. 205). Hoboken, NJ: John Wiley & Sons, Inc.

4. Kerppola, T. K. (2008). Bimolecular Fluorescence Complementation (BiFC) Analysis as a Probe of Protein Interactions in Living Cells. Annual Review of Biophysics, (37), 465 - 487. doi:10.1146/annurev.biophys.37.032807.125842.

5. Liebman, S. W., & Chernoff, Y. O. (2012). Prions in Yeast. Genetics, 191(4), 1041-1072. doi:10.1534/genetics.111.137760

6. Tyedmers, J., Treusch, S., Dong, J., Mccaffery, J. M., Bevis, B., & Lindquist, S. (2010). Prion induction involves an ancient system for the sequestration of aggregated proteins and heritable changes in prion fragmentation. Proceedings of the National Academy of Sciences, 107(19), 8633-8638. doi:10.1073/pnas.1003895107.

7. Wickner, R., Taylor, K., Edskes, H., & Maddelein, M. (2000). Prions: Portable prion domains. Current Biology,10(9). doi:10.1016/s0960-9822(00)00460-7.
