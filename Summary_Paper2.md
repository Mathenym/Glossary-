##"Atomic Limits in the Search for Galactic Dark Matter" A brief Summary  

This paper talks about the shortcomings of the Linhard model and introduces a few corrections to hopefully correct for the discrepancies between model and experiment in the low energy regime for nuclear recoils. 

### Lindhard Model:

In the context of this paper, the Lindhard model is used to determine the amount of electronic excitation produced by a recoiling atom is quenched by relative to a recoiling electron of the same energy. 
The question asked by the paper seems straight forward enough: For a recoiling atom with a known energy $E$, how much of the energy loss $\eta$ is given to the electrons? In other-words, how much energy is transferred into the electronic system or, what is the ionization efficiency/ quenching factor? The author assumes that the remaining energy that is not transferred into the electronic system $\nu,$ is lost due to atomic motion and unless phonon energy is measured, $\eta$ is the upper limit to the available signal. The total energy is therefore $E = \eta + \nu$ 
The average energy given to atomic motion and therefore not the electronic system is defined as such:
\
$k \epsilon^{1/2}\nu^{'}(\epsilon) = \int_{0}^{\epsilon^{2}} \frac{dt}{2t^{\frac{3}{2}}}f(t^{1/2})(\nu(\epsilon -\frac{t}{\epsilon}) - \nu(\epsilon)+\nu(\frac{t}{\epsilon})) $
\
Where 
\
$\epsilon = E\frac{a}{2Z^2e^2}$
\
is the dimensionless energy. 

The formulation of this equation is dependent upon 4 assumptions: 

1) Ionized electrons do not produce recoil atoms of appreciable energy, 
2) The atomic binding energy u of electrons is negligible.
3) Energy Transfers to electrons are small relative to energy transfers to atoms. 
4) The treatment of atomic and electronic collisions are separable. 

Of the 4 assumptions, the second is thought to have the most effect at low nuclear recoil energies, which the author will make a correction for. 

##### Nuclear Stopping Cross Section 
The model for scattering is a 2 body scattering in a screening potential. The screening potential is defined by as your typical coulombic potential but with a single atom Thomas-Fermi screening function tagged on. **see notes for form** The problem is simplified by treating the interactions as a two body central force scattering. Essentially Rutheford scattering that takes into account the movement (recoil) of the target atom, and then transforms into the center of mass frame to turn a 2 body problem into a 1 body problem.  

##### Electronic Stopping Cross Section

The electronic stopping power can be written as follows: 
\
 $S_e(\epsilon) = \frac{d\epsilon}{d\rho} = k\epsilon^{1/2}$
 \
 Where $\rho$ is the reduced range of interaction. This implies that velocity and stopping power are proportional. This inherently assumes that we model the atomic electrons as an electron gas, where in reality our detectors are semiconductors with large band gaps. The author assumes that this would not be the case, but this phenomenon is still observed in materials with large band gaps. There is however a reduced energy cut off or threshold velocity in which the particle suffers no energy loss to the electronic system. The threshold velocity should be able to be calculated from kinematic constraints, like point particles. But reference 22 in the paper shows that these constraints do not hold for atomic like projectiles. The author mentions that intuitively the materials band structure should effect the low-energy electronic response to nuclear recoils, but the assumption that the atomic binding energy of electrons are negligible in the model seem to be the reason this effect isn't noticed.  

 ##### Standard Solutions 


 $\nu(\epsilon) = \frac{\epsilon}{1+kg(\epsilon)}$

 $g(\epsilon) = 3\epsilon^{0.15} + 0.7*\epsilon^{0.6} + \epsilon $

The ionization yield due to nuclear recoil is therefore: 
 
 $f_n = \frac{\epsilon - \nu}{\epsilon} = \frac{kg(\epsilon)}{1+kg(\epsilon)}$
 
where
 
 $k = 0.133Z^{2/3}A^{1/2}$ 

 The residuals between the right and left hand side in the main equation grow dramatically as we approach lower nuclear recoil energies. 

 $<5\%$ at $\epsilon = 10^{-1}$ about $25\%$ at $\epsilon = 10^{-3}$ and more than $50\%$ at $\epsilon = 10^{-4}$ See figure 1 in paper. 

##### Solutions Near Threshold 

To correct this, the author added a constant q 

 $\nu(\epsilon) = \frac{\epsilon}{1+kg(\epsilon)} + q$

 When removing the 2 assumption stated above, adding the constant q improves the behavior for energies smaller than 1keV

The quenching function only begins to differ from the above equation for $E > 100eV$

 $f_n = \frac{kg(\epsilon)}{1+kg(\epsilon)} + \frac{q}{\epsilon}$ 

The residuals however, are reduced to a few percent across the entire reduced energy spectrum. 

##### Atomic Binding Energy 

When the recoiling atom slows down, some of the energy must be spent on atomic binding. The model consider average quantities, therefor the binding energy can be thought of as the average energy to create an electron-hole pair. To account for the binding energy, the author replaces $\nu(\frac{t}{\epsilon})$ with $\nu(\frac{t}{\epsilon-u})$ where $u = 1.06*10^{-5}$. The result is a sharp cutoff as seen in the plot, which is now a cutoff in the fraction of energy given to the electrons at a nuclear recoil energy of $E_r \approx 100eV$. The % error in the solution increases rapidly as the derivative at that point approaches a constant. 
\
The author tries a different way to define $\nu$ by parameterizing using a simple power law. It gave a similar fit, but the cutoff due to atomic binding occurs at a higher energy by a factor of 2, concluding that accounting for binding energy is a better parameterization. 

##### Effects on Dark Matter Direct Detection Sensitivity. 

The correction for atomic binding energy to the Lindhard model dramatically decreased the sensitivity to low mass dark matter. (Except for Argon, but Argon deviated at higher energies.) This model showed that there is an kinematic cutoff due to binding energy and is an inherent and usually ignored part of the Lindhard model. This has shed light on the expectations for quenching at very low energy nuclear recoils. 