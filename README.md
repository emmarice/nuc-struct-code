# py-relex
---
Emma Rice,
emmarice@berkeley.edu,
1/12/2023

---
Adapted from the [Bertulani '99](https://www.sciencedirect.com/science/article/pii/S0010465598001416) fortran code by the same name for relativistic Coulomb excitation.
---
# Intro


|  Inputs |   |  
|---|---|
| **ap, zp, at, zt**  |  masses and charges of projectile and target | 
| **eca**  | bombarding energy per nucleon (MeV) | 
| **iw** | =0 for projectile, =1 for target  |  
|**iout**  | =0 for no statistical tensor output, =1 for yes  |  
| **nb**  | number points in impact parameter (b) mesh  |  
| **accur**  | accuracy for time integration at each impact parameter  |  
| **bmin**  | minimum impact parameter for integration of cross section  |  
| **itot**  | =0 does not print impact parameter probabilities, =1 does print|  
| **iopw**  |=0 no optical potential entered, =1 optical potential entered (in optw.in)|  
| **iopnuc**  | =0 do not compute nuclear excitation, =1 do compute  |  
| **nst**  | number of nuclear levels  |  
| **i, ex(i), spin(i)**  | state label, energy, and spin. i ranges from 1 to nst.  |  
|**state1, state2, mate1, mate2, matm1**  | reduced matrix elements from e1, e2, m1 excitations  |  



# Example

|  Inputs |   |  
|---|---|
| **ap, zp, at, zt**  | 25.01, 9., 208.98, 83.  | 
| **eca**  | 100 | 
| **iw** | 0 |  
|**iout**  | 1  |  
| **nb**  | 40 |  
| **accur**  | 0.001 |  
| **bmin**  | 10. |  
| **itot**  | 1 |  
| **iopw**  | 0 |  
| **iopnuc**  | 0 |  
| **nst**  | 2 |  
| **i, ex(i), spin(i)**  | 1, 0.0, 2.5  |  
| **i, ex(i), spin(i)**  | 2, 3.3, 4.5  | 
|**state1, state2, mate1, mate2, matm1**  | 1, 2, 0., 10.5, 0. |  
|**state1, state2, mate1, mate2, matm1**  | 0, 0, 0., 0., 0. | 
