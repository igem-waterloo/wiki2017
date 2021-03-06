# FRET

The team successfully transformed yeast cells with the plasmids required to perform the FRET experiments. Thus we had stocks of both [psi-] and [PSI+] W303 yeast containing our parts PrD-YFP, PrD-CFP, and both parts simultaneously.

Ideally, the FRET experiment would have been performed on a flow cytometer. We would have excited the CFP on PrD-CFP and looked for YFP fluorescence, which we hypothesized would be greater in [PSI+]. This would theoretically be due to the fluorescent proteins coming close together in the aggregate, and thus allowing non-emissive energy transfer from CFP to YFP that would not be possible if the proteins were further than 10 nm apart [1].

However, the Waterloo iGEM team did not have access to a flow cytometer with a laser with an appropriate wavelength; a ~430 nm light source is required to excite CFP. Subsequently, the team searched for a plate reader, which could also be used to perform the experiment. Unfortunately, no plate reader with an appropriate light source could be located on-campus. Therefore, the team decided to utilize a fluorometer with an adjustable light source to perform the excitation. Emission spectra were taken using a Horiba Fluorolog Spectrophotometer.

The drawback of this method of going about the experiments was that fluorometers are not typically used with live cells, as cells scatter light at ~500 nm and in a variable fashion depending on cell size. Nonetheless, so long as the presence of a fluorescent protein results in a distinct emission peak, the fluorometer is still useful as a tool.

We first confirmed, using yeast cells with a plasmid containing our Cup1-GFP part, that fluorometry can be used to confirm the presence of a fluorescent protein (see graph below); our samples containing GFP had a clear peak at 512 nm not present in any of our empty cell controls when excitation was performed at 488 nm. The sudden peak at the left side of the graph seen in all samples is from the light source, which bled over into the measured signal.

![ERROR]({{image "GFPcontgraph.png" "directlink" mode}})

The data above had the signal from the blank subtracted from it, but the data were not normalized for the precise number of cells. Samples were approximately normalized to 10^6 cells per mL, but this could not be done exactly, which resulted in visible variation in the signal. An additional study performed by the team found that the signal after subtraction of the blank signal was approximately proportional to cell concentration, both in the case of signal from GFP and the signal from cell scattering (data not shown).

The samples containing our constructs were not normalized as strictly due to the fact that we were simply checking for the existence of a peak, not the peak’s magnitude, but cell concentration still should have fallen between 10^5 and 10^6 cells per mL. The data for excitation at 488 nm are given below:

![ERROR]({{image "Excitationat488.png" "directlink" mode}})

Though this was not the precise desired excitation for YFP (which would be ~510 nm) [1], this allowed direct comparison to our flow cytometry work (elaborated on in our proof of functionality for our parts).

On the fluorometer, a distinct peak at 527 nm was observed in only the three [psi-] samples that contained YFP. This is in agreement with our flow cytometry data, which was only able to detect a high level of fluorescence in those same samples. Unsurprisingly, the fluorometer is less sensitive than the flow cytometer and thus even if other samples fluoresce at a low level, we would probably not be able to detect them here.

Upon excitation with of our samples at 430 nm on the fluorometer, we unfortunately were not able to tell whether or not our cells were fluorescing. This is because signal from cell scattering overlapped with the estimated emission spectrum for CFP. In one sample, however, we did see possible evidence that our system was functional:

![ERROR]({{image "Excitationat430.png" "directlink" mode}})

Given our knowledge that signal is approximately proportional to cell concentration, we scaled our [PSI+] CFP sample to have the same average signal as our [PSI+] CFP and YFP sample from 605 to 615 nm. At this wavelength, there should be no or next to no YFP signal, meaning the two samples should be identical. The excitation used to obtain the above data was performed at a higher source light intensity than previously used in the hope of seeing a fluorescence signal where previously the signal was too small compared to noise.

Since excitation at 430 nm should have no effect on YFP, and the presence of our constructs was confirmed in all cells, any difference in the signal of these two samples should be due to transfer of energy from CFP to YFP. Since the [PSI+] CFP and YFP sample is simultaneously lower at ~480 nm and higher at ~510 nm, the data seem to indicate that this energy transfer was happening. However, given that this experiment comes from a simple comparison of two samples, we cannot assign a high degree of certainty to this conclusion. Additionally, a the emission spectrum for [psi-] CFP and YFP was quite similar to that of [PSI+] CFP and YFP, which should not have been the case.

It is possible that had we included the M domain of Sup35 in our prion tag on the fluorescent proteins, we would have seen higher fluorescence in aggregate. This would allow us to make a more definitive conclusion. We had anticipated that the lack of the M domain may cause issues, and we had it synthesized in anticipation, with appropriate restriction sites to add it into our constructs.

We began work on adding the M domain, but as of the Wiki Freeze had not yet completed adding it to our construct PrD-YFP.

## References

[1] Piston, D. W., & Kremers, G.-J. (2007). Fluorescent protein FRET: the good, the bad and the ugly. Trends in Biochemical Sciences, 32(9), 407–414. https://doi.org/10.1016/j.tibs.2007.08.003



# Split YFP

The team created all necessary parts to perform these experiments. However, given the concern over the lack of the M-domain, we wanted to first confirm that fluorescence can be observed by making a translational fusion described in the FRET experiments. 
