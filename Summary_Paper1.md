## "Measurement of the Ionization Produced by Sub-keV Silicon Nuclear Recoils in a CCD Dark Matter Detector." A brief summary. 

### Intro

One common method used to detect low mass WIMP-like dark matter is through the ionization produced by a recoiling nucleus. In this paper, the authors used a Silicon CCD detector. Silicon is an ideal detector material due to its low noise and relatively low mass. Interactions yielding high recoil energies produce ionization signals that are the same as an electron of the same energy. The detectors are most sensitive to a WIMP mass below $10GeV/C^2$.  The paper aims to quantify the nuclear recoil ionization which is important in characterizing the sensitivity of a WIMP detector. 

### Experimental Setup 

The authors use a $^{124}$Sb$^9$Be photoneutron source to produce low energy neutrons with energy of 24keV with production rate of $10^4s^{-1}$. The neutrons elastically scatter off silicon nuclei in the detector yielding nuclear recoils that deposit an energy of $<3.2keV_{nr}$ within the bulk of the detector. 
The detector was an 8Mpixel CCD with an area of $18.8cm^2$. A Bias voltage of 128V was applied to prevent any diffusion of charge carriers. This insures that there are no regions of partial charge collection that might hinder the energy response of the CCD. on average, $3.8eV_{ee}$ is required to free a charge carrier in silicon.
The detector was placed in a vacuum sealed aluminum container. Between the source and the detector, there was a 20cm block of lead to help prevent outside sources of noise and to mimic the conditions that are available only in underground experiments. Due to the large mass of Pb, the neutron flux was minimally effected by the shielding. The flux was measured by a $^3$He counter placed outside of the vacuum chamber. 

### Analysis Methods 

This Authors used two methods to determine nuclear recoil ionization efficiency: 
The first method used a cubic spline function with 3 free parameters to parameterize $E_e$ as a function of nuclear recoil energy $E_r$. The relationship between ionization energy and nuclear recoil energy is defined as:
$$
E_e = \Gamma E_r
$$
Where 
 $$
 \Gamma = \frac{1+\frac{eV_b}{\epsilon_\gamma}Y(E_{nr})}{(1+\frac{eV_b}{\epsilon_\gamma})}
 $$
 With $Y(E_{nr})$ being the nuclear recoil ionization efficiency or "yield function." 
 The method fitted a $E_e$ spectrum to the data was derived by applying the spline to the simulated $E_r$ spectrum. (See figure 4 in the paper to visualize the results.) The fitting function was obtained by applying the spline model of the nuclear recoil efficiency to the simulated recoil spectrum and convolving with the detector resolution. 
 The second method used was the "Integral Method" **Look more into this.** The integral method is a way to determine a desired quantity that is directly coupled to a known or measured PDF. For example, the authors are using the simulated PDF of the number of electron-hole pairs created by a nuclear recoil to determine the exact energy that created them. This method works by equating two integrals, one for the PDF if the simulated recoil energy and one for the PDF of the measured number of e-h pairs produced. The lower integration bound, $ Y(E_r)$, for the second integral is then varied so that the two integrals are equivalent. 

 ### Results and Conclusions 

 The integral method was applied to configurations with several different sources and 2 target configurations, BeO and alumina-BeO. Both resulted in results consistent within statistical uncertainty. There were many sources of statistical uncertainty, but both target configurations mostly agreed with each other. The maximum energy deviation was 16% at an energy of $E_e=60eV_{ee}$ - but the differences were far beyond statistical uncertainty at low energies. The total systematic uncertainty was 8.5% 
 They authors reported nuclear recoil ionization efficiency for energies between $0.7$ and $3.2keV_{nr}$. The measured efficiency was found to deviate significantly from the lindard model at low energies. The authors confirm this deviations with recent measurements from an experiment using fast neutrons at high recoil energies. Deviation from the lindhard model effects the WIMP sensitivity calculations as the sensitivity is overstated at the lower WIMP masses.

 

