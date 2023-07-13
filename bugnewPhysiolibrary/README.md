Model produces warning during compilation
```

Check of modelECMORespiratoryVR.ECMOSimNoRegVentilatorVCFlat:

Modifier for protected component EnthalpyNotUsed. This is not legal Modelica.
Modelica Text: line 10
Context: modelECMORespiratoryVR.ECMOSimNoRegVentilatorVCFlat.lungs.EnthalpyNotUsed
Original declaration of EnthalpyNotUsed:
File: C:/Users/tomas/Projects-local/physiome/Physiolibrary/Physiolibrary/Fluid.mo, line 717
Context: Physiolibrary.Fluid.Interfaces.Accumulation.EnthalpyNotUsed

Inconsistency for connectors dimensioned using parameter with annotation(Dialog(connectorSizing=true)).
Some connector elements are not connected.
This is either because the connections and/or parameters has been edited textually to an inconsistent state
or because the default for the parameter is not 0. The unconnected connectors are:
LungCapilars.q_in[1]
LungsVeins.q_in[1]
LungsVeins.q_in[2]
LungsVeins.q_in[3]
LungsArteries.q_in[1]
LungsArteries.q_in[2]

The model has the same number of unknowns and equations: 11075

Check of modelECMORespiratoryVR.ECMOSimNoRegVentilatorVCFlat successful.

WARNINGS have been issued.
```

Model produces error during simulation
```
Log-file of program ./dymosim
(generated: Thu Jul 13 16:41:57 2023)
dymosim started
... "modelECMORespiratoryVR.ECMOSimNoRegVentilatorVCFlat" simulating
... "dsin.txt" loading (dymosim input file)
... "ECMOSimNoRegVentilatorVCFlat.mat" creating (simulation result file)

Integration started at T = 0 using integration method DASSL
(DAE multi-step solver (dassl/dasslrt of Petzold modified by Dassault Systemes))
Error: The following error was detected at time: 0.001071164516279926

Model error - Modelica.Math.log (T/298.15) = Modelica.Math.log (-0.0996489)
The stack of functions is:
molarEntropyPure_Unique83
chemicalPotentialPure_Unique82
Vectorized chemicalPotentialPure_Unique82
electrochemicalPotentials_pTXvI_Unique81
electrochemicalPotentials_pTXvI_Unique81(Alveoly.q_in[1].p, Alveoly.chemicalSolution.T, Alveoly.chemicalSolution.x_baseMolecule, 0.0, 0.0)

Solver will attempt to handle this problem.

Error: The following error was detected at time: 0.00107116768399449

Model error - Modelica.Math.log (T/298.15) = Modelica.Math.log (-0.0048461)
The stack of functions is:
molarEntropyPure_Unique83
chemicalPotentialPure_Unique82
Vectorized chemicalPotentialPure_Unique82
electrochemicalPotentials_pTXvI_Unique81
electrochemicalPotentials_pTXvI_Unique81(Alveoly.q_in[1].p, Alveoly.chemicalSolution.T, Alveoly.chemicalSolution.x_baseMolecule, 0.0, 0.0)

Solver will attempt to handle this problem.

... Error message from dymosim
At time T = 1.071168e-03 and stepsize
H = 6.576618e-15 the corrector could not converge.
Repeated convergence test failures occurred on the last attempted step
in the code. An inaccurate or ill-conditioned Jacobian may be the
problem. Integration will be terminated.

Integration terminated before reaching "StopTime" at T = 0.00107
States and derivatives:
LungsArteries.chemicalSolution.logm[1]=-1.69494 0.123833
LungsArteries.chemicalSolution.logm[2]=-9.21692 0.123833
LungsArteries.chemicalSolution.logm[3]=-7.94157 0.123833
LungsArteries.chemicalSolution.logm[4]=-24.1075 0.123833
LungsArteries.chemicalSolution.logm[5]=-2.95131 0.123833
LungsArteries.chemicalSolution.logm[6]=-8.24963 0.123833
LungsArteries.chemicalSolution.logm[7]=-8.24963 0.123833
LungsArteries.chemicalSolution.logm[8]=-4.09408 0.123833
LungsArteries.chemicalSolution.logm[9]=-4.543 0.123833
LungsArteries.chemicalSolution.logm[10]=-12.1064 0.123833
LungsArteries.chemicalSolution.logm[11]=-7.51307 0.123833
LungsArteries.chemicalSolution.logm[12]=-7.78167 0.123833
LungsArteries.chemicalSolution.logm[13]=-10.243 0.123833
LungsArteries.chemicalSolution.logm[14]=-8.7945 0.123833
LungsArteries.chemicalSolution.logm[15]=-8.57437 0.123833
LungsArteries.chemicalSolution.logm[16]=-7.8833 0.123833
LungsArteries.chemicalSolution.logm[17]=-13.178 0.123833
LungsArteries.chemicalSolution.logm[18]=-7.71938 0.123833
LungsArteries.chemicalSolution.logm[19]=-24.9096 0.123833
LungsArteries.chemicalSolution.logm[20]=-23.1178 0.123833
LungsArteries.chemicalSolution.logm[21]=-27.908 0.123833
LungsArteries.chemicalSolution.logm[22]=-22.0563 0.123833
LungsArteries.chemicalSolution.logm[23]=-24.3546 0.123833
LungsArteries.chemicalSolution.logm[24]=-23.8725 0.123833
LungsArteries.chemicalSolution.logm[25]=-17.3137 0.123833
LungsArteries.chemicalSolution.logm[26]=-19.6163 0.123833
LungsArteries.chemicalSolution.logm[27]=-33.2036 0.123833
LungsArteries.chemicalSolution.logm[28]=-147.234 0.123833
LungsArteries.chemicalSolution.logm[29]=-147.377 0.123833
LungsArteries.chemicalSolution.logm[30]=-7.87521 0.123833
LungsArteries.chemicalSolution.logm[31]=-25.6027 0.123833
LungsArteries.chemicalSolution.logm[32]=-32.908 0.123833
LungsArteries.chemicalSolution.logm[33]=-23.8198 0.123833
LungsArteries.chemicalSolution.logm[34]=-8.18046 0.123833
LungsArteries.chemicalSolution.logm[35]=-2.0046 0.123833
LungsArteries.enthalpy=-2.13442e+06 -264311
LungsArteries.enthalpy_future=-2.13442e+06 -264311
LungsVeins.chemicalSolution.logm[1]=-1.64233 1.33926
LungsVeins.chemicalSolution.logm[2]=-9.16423 1.44308
LungsVeins.chemicalSolution.logm[3]=-7.88908 1.18917
LungsVeins.chemicalSolution.logm[4]=-24.0549 1.33926
LungsVeins.chemicalSolution.logm[5]=-2.8987 1.33926
LungsVeins.chemicalSolution.logm[6]=-8.19702 1.33926
LungsVeins.chemicalSolution.logm[7]=-8.19702 1.33926
LungsVeins.chemicalSolution.logm[8]=-4.04147 1.33926
LungsVeins.chemicalSolution.logm[9]=-4.49039 1.33926
LungsVeins.chemicalSolution.logm[10]=-12.0538 1.33926
LungsVeins.chemicalSolution.logm[11]=-7.46046 1.33926
LungsVeins.chemicalSolution.logm[12]=-7.72906 1.33926
LungsVeins.chemicalSolution.logm[13]=-10.1904 1.33926
LungsVeins.chemicalSolution.logm[14]=-8.7419 1.33926
LungsVeins.chemicalSolution.logm[15]=-8.52176 1.33926
LungsVeins.chemicalSolution.logm[16]=-7.8307 1.33926
LungsVeins.chemicalSolution.logm[17]=-13.1254 1.33926
LungsVeins.chemicalSolution.logm[18]=-7.66677 1.33926
LungsVeins.chemicalSolution.logm[19]=-24.857 1.33926
LungsVeins.chemicalSolution.logm[20]=-23.0652 1.33926
LungsVeins.chemicalSolution.logm[21]=-27.8554 1.33926
LungsVeins.chemicalSolution.logm[22]=-22.0036 1.33926
LungsVeins.chemicalSolution.logm[23]=-24.302 1.33926
LungsVeins.chemicalSolution.logm[24]=-23.8199 1.33926
LungsVeins.chemicalSolution.logm[25]=-17.2611 1.33926
LungsVeins.chemicalSolution.logm[26]=-19.5637 1.33926
LungsVeins.chemicalSolution.logm[27]=-33.151 1.33926
LungsVeins.chemicalSolution.logm[28]=-147.182 1.33926
LungsVeins.chemicalSolution.logm[29]=-147.325 1.33926
LungsVeins.chemicalSolution.logm[30]=-7.8226 1.33926
LungsVeins.chemicalSolution.logm[31]=-25.5501 1.33926
LungsVeins.chemicalSolution.logm[32]=-32.8554 1.33926
LungsVeins.chemicalSolution.logm[33]=-23.7672 1.33926
LungsVeins.chemicalSolution.logm[34]=-8.12785 1.33926
LungsVeins.chemicalSolution.logm[35]=-1.95199 1.33926
LungsVeins.enthalpy=-2.24972e+06 -3.01245e+06
LungsVeins.enthalpy_future=-2.24972e+06 -3.01245e+06
Alveoly.chemicalSolution.logm[1]=-26.9857 -1.9555e+12
Alveoly.chemicalSolution.logm[2]=-32.4535 -1.85445e+12
Alveoly.chemicalSolution.logm[3]=-29.9299 -1.96318e+12
Alveoly.chemicalSolution.logm[4]=-25.8383 -1.96318e+12
Alveoly.enthalpy=-3.69212e-06 7.24278e+06
Alveoly.enthalpy_future=-3.69212e-06 7.24278e+06
LungCapilars.chemicalSolution.logm[1]=-2.62828 -3.40566
LungCapilars.chemicalSolution.logm[2]=-10.0754 -351.622
LungCapilars.chemicalSolution.logm[3]=-8.99404 -10.4305
LungCapilars.chemicalSolution.logm[4]=-25.0408 -3.40566
LungCapilars.chemicalSolution.logm[5]=-3.88465 -3.40566
LungCapilars.chemicalSolution.logm[6]=-9.18297 -3.40566
LungCapilars.chemicalSolution.logm[7]=-9.18297 -3.40566
LungCapilars.chemicalSolution.logm[8]=-5.02742 -3.40566
LungCapilars.chemicalSolution.logm[9]=-5.47635 -3.40566
LungCapilars.chemicalSolution.logm[10]=-13.0397 -3.40566
LungCapilars.chemicalSolution.logm[11]=-8.44641 -3.40566
LungCapilars.chemicalSolution.logm[12]=-8.71502 -3.40566
LungCapilars.chemicalSolution.logm[13]=-11.1764 -3.40566
LungCapilars.chemicalSolution.logm[14]=-9.72785 -3.40566
LungCapilars.chemicalSolution.logm[15]=-9.50772 -3.40566
LungCapilars.chemicalSolution.logm[16]=-8.81665 -3.40566
LungCapilars.chemicalSolution.logm[17]=-14.1114 -3.40566
LungCapilars.chemicalSolution.logm[18]=-8.65272 -3.40566
LungCapilars.chemicalSolution.logm[19]=-25.8429 -3.40566
LungCapilars.chemicalSolution.logm[20]=-24.0512 -3.40566
LungCapilars.chemicalSolution.logm[21]=-28.8414 -3.40566
LungCapilars.chemicalSolution.logm[22]=-22.9896 -3.40566
LungCapilars.chemicalSolution.logm[23]=-25.2879 -3.40566
LungCapilars.chemicalSolution.logm[24]=-24.8058 -3.40566
LungCapilars.chemicalSolution.logm[25]=-18.247 -3.40566
LungCapilars.chemicalSolution.logm[26]=-20.5496 -3.40566
LungCapilars.chemicalSolution.logm[27]=-34.137 -3.40566
LungCapilars.chemicalSolution.logm[28]=-148.168 -3.40566
LungCapilars.chemicalSolution.logm[29]=-148.311 -3.40566
LungCapilars.chemicalSolution.logm[30]=-8.80855 -3.40566
LungCapilars.chemicalSolution.logm[31]=-26.5361 -3.40566
LungCapilars.chemicalSolution.logm[32]=-33.8413 -3.40566
LungCapilars.chemicalSolution.logm[33]=-24.7532 -3.40566
LungCapilars.chemicalSolution.logm[34]=-9.1138 -3.40566
LungCapilars.chemicalSolution.logm[35]=-2.93794 -3.40566
LungCapilars.enthalpy=-839193 2.86563e+06
LungCapilars.enthalpy_future=-839193 2.86563e+06
Arteries.chemicalSolution.logm[1]=-0.890142 -0.123592
Arteries.chemicalSolution.logm[2]=-8.41212 -0.123592
Arteries.chemicalSolution.logm[3]=-7.13677 -0.123592
Arteries.chemicalSolution.logm[4]=-23.3027 -0.123592
Arteries.chemicalSolution.logm[5]=-2.14651 -0.123592
Arteries.chemicalSolution.logm[6]=-7.44483 -0.123592
Arteries.chemicalSolution.logm[7]=-7.44483 -0.123592
Arteries.chemicalSolution.logm[8]=-3.28928 -0.123592
Arteries.chemicalSolution.logm[9]=-3.7382 -0.123592
Arteries.chemicalSolution.logm[10]=-11.3016 -0.123592
Arteries.chemicalSolution.logm[11]=-6.70827 -0.123592
Arteries.chemicalSolution.logm[12]=-6.97687 -0.123592
Arteries.chemicalSolution.logm[13]=-9.43824 -0.123592
Arteries.chemicalSolution.logm[14]=-7.98971 -0.123592
Arteries.chemicalSolution.logm[15]=-7.76957 -0.123592
Arteries.chemicalSolution.logm[16]=-7.07851 -0.123592
Arteries.chemicalSolution.logm[17]=-12.3732 -0.123592
Arteries.chemicalSolution.logm[18]=-6.91458 -0.123592
Arteries.chemicalSolution.logm[19]=-24.1048 -0.123592
Arteries.chemicalSolution.logm[20]=-22.313 -0.123592
Arteries.chemicalSolution.logm[21]=-27.1032 -0.123592
Arteries.chemicalSolution.logm[22]=-21.2515 -0.123592
Arteries.chemicalSolution.logm[23]=-23.5498 -0.123592
Arteries.chemicalSolution.logm[24]=-23.0677 -0.123592
Arteries.chemicalSolution.logm[25]=-16.5089 -0.123592
Arteries.chemicalSolution.logm[26]=-18.8115 -0.123592
Arteries.chemicalSolution.logm[27]=-32.3988 -0.123592
Arteries.chemicalSolution.logm[28]=-146.429 -0.123592
Arteries.chemicalSolution.logm[29]=-146.573 -0.123592
Arteries.chemicalSolution.logm[30]=-7.07041 -0.123592
Arteries.chemicalSolution.logm[31]=-24.7979 -0.123592
Arteries.chemicalSolution.logm[32]=-32.1032 -0.123592
Arteries.chemicalSolution.logm[33]=-23.015 -0.123592
Arteries.chemicalSolution.logm[34]=-7.37566 -0.123592
Arteries.chemicalSolution.logm[35]=-1.1998 -0.123592
Arteries.enthalpy=-4.77309e+06 589917
Arteries.enthalpy_future=-4.77309e+06 589917
Veins.chemicalSolution.logm[1]=0.451187 0.0204852
Veins.chemicalSolution.logm[2]=-7.07079 0.0204806
Veins.chemicalSolution.logm[3]=-5.79545 0.0204866
Veins.chemicalSolution.logm[4]=-21.9614 0.0204852
Veins.chemicalSolution.logm[5]=-0.805182 0.0204852
Veins.chemicalSolution.logm[6]=-6.1035 0.0204852
Veins.chemicalSolution.logm[7]=-6.1035 0.0204852
Veins.chemicalSolution.logm[8]=-1.94795 0.0204852
Veins.chemicalSolution.logm[9]=-2.39687 0.0204852
Veins.chemicalSolution.logm[10]=-9.96027 0.0204852
Veins.chemicalSolution.logm[11]=-5.36694 0.0204852
Veins.chemicalSolution.logm[12]=-5.63554 0.0204852
Veins.chemicalSolution.logm[13]=-8.09691 0.0204852
Veins.chemicalSolution.logm[14]=-6.64838 0.0204852
Veins.chemicalSolution.logm[15]=-6.42824 0.0204852
Veins.chemicalSolution.logm[16]=-5.73718 0.0204852
Veins.chemicalSolution.logm[17]=-11.0319 0.0204852
Veins.chemicalSolution.logm[18]=-5.57325 0.0204852
Veins.chemicalSolution.logm[19]=-22.7635 0.0204852
Veins.chemicalSolution.logm[20]=-20.9717 0.0204852
Veins.chemicalSolution.logm[21]=-25.7619 0.0204852
Veins.chemicalSolution.logm[22]=-19.9101 0.0204852
Veins.chemicalSolution.logm[23]=-22.2084 0.0204852
Veins.chemicalSolution.logm[24]=-21.7264 0.0204852
Veins.chemicalSolution.logm[25]=-15.1676 0.0204852
Veins.chemicalSolution.logm[26]=-17.4702 0.0204852
Veins.chemicalSolution.logm[27]=-31.0575 0.0204852
Veins.chemicalSolution.logm[28]=-145.088 0.0204852
Veins.chemicalSolution.logm[29]=-145.231 0.0204852
Veins.chemicalSolution.logm[30]=-5.72908 0.0204852
Veins.chemicalSolution.logm[31]=-23.4566 0.0204852
Veins.chemicalSolution.logm[32]=-30.7619 0.0204852
Veins.chemicalSolution.logm[33]=-21.6737 0.0204852
Veins.chemicalSolution.logm[34]=-6.03433 0.0204852
Veins.chemicalSolution.logm[35]=0.141527 0.0204852
Veins.enthalpy=-1.82529e+07 -373914
Veins.enthalpy_future=-1.82529e+07 -373914
Tissue.chemicalSolution.logm[1]=-1.93159 -0.120372
Tissue.chemicalSolution.logm[2]=-9.45368 -0.218973
Tissue.chemicalSolution.logm[3]=-8.17819 -0.0900791
Tissue.chemicalSolution.logm[4]=-24.3442 -0.120372
Tissue.chemicalSolution.logm[5]=-3.18796 -0.120372
Tissue.chemicalSolution.logm[6]=-8.48628 -0.120372
Tissue.chemicalSolution.logm[7]=-8.48628 -0.120372
Tissue.chemicalSolution.logm[8]=-4.33073 -0.120372
Tissue.chemicalSolution.logm[9]=-4.77965 -0.120372
Tissue.chemicalSolution.logm[10]=-12.3431 -0.120372
Tissue.chemicalSolution.logm[11]=-7.74972 -0.120372
Tissue.chemicalSolution.logm[12]=-8.01832 -0.120372
Tissue.chemicalSolution.logm[13]=-10.4797 -0.120372
Tissue.chemicalSolution.logm[14]=-9.03116 -0.120372
Tissue.chemicalSolution.logm[15]=-8.81102 -0.120372
Tissue.chemicalSolution.logm[16]=-8.11996 -0.120372
Tissue.chemicalSolution.logm[17]=-13.4147 -0.120372
Tissue.chemicalSolution.logm[18]=-7.95603 -0.120372
Tissue.chemicalSolution.logm[19]=-25.1462 -0.120372
Tissue.chemicalSolution.logm[20]=-23.3545 -0.120372
Tissue.chemicalSolution.logm[21]=-28.1447 -0.120372
Tissue.chemicalSolution.logm[22]=-22.2929 -0.120372
Tissue.chemicalSolution.logm[23]=-24.5912 -0.120372
Tissue.chemicalSolution.logm[24]=-24.1092 -0.120372
Tissue.chemicalSolution.logm[25]=-17.5504 -0.120372
Tissue.chemicalSolution.logm[26]=-19.8529 -0.120372
Tissue.chemicalSolution.logm[27]=-33.4403 -0.120372
Tissue.chemicalSolution.logm[28]=-147.471 -0.120372
Tissue.chemicalSolution.logm[29]=-147.614 -0.120372
Tissue.chemicalSolution.logm[30]=-8.11186 -0.120372
Tissue.chemicalSolution.logm[31]=-25.8394 -0.120372
Tissue.chemicalSolution.logm[32]=-33.1446 -0.120372
Tissue.chemicalSolution.logm[33]=-24.0565 -0.120372
Tissue.chemicalSolution.logm[34]=-8.41711 -0.120372
Tissue.chemicalSolution.logm[35]=-2.24125 -0.120372
Tissue.enthalpy=-1.68463e+06 202705
Tissue.enthalpy_future=-1.68463e+06 202705
lungs.chemicalSolution.logm[1]=-7.40194 0.183946
lungs.chemicalSolution.logm[2]=-13.3469 0.183946
lungs.chemicalSolution.logm[3]=-10.3278 0.183946
lungs.chemicalSolution.logm[4]=-6.23623 0.183946
lungs.enthalpy=-421.502 -77.5338
lungs.enthalpy_future=-421.502 -77.5338
CPU-time for integration : 8.08 seconds
CPU-time for one grid interval : 8.08e+03 milliseconds
CPU-time for initialization : 0.013 seconds
Number of result points : 10
Number of grid points : 2
Number of accepted steps : 123
Number of f-evaluations (dynamics) : 388
Number of crossing function evaluations : 161
Number of Jacobian-evaluations : 152
Number of model time events : 0
Number of input time events : 0
Number of state events : 4
Number of step events : 0
Minimum integration stepsize : 2.24e-13
Maximum integration stepsize : 0.000154
Maximum integration order : 2
Calling terminal section
... "dsfinal.txt" creating (final states)
ERROR: The simulation of modelECMORespiratoryVR.ECMOSimNoRegVentilatorVCFlat FAILED
```
