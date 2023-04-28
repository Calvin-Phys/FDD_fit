# Fermi Edge Fitting and Fermi Dirac Distribution Correction

This tool can fit the shape of a cut's Fermi edge and apply resolution-convoluted Fermi-Dirac Distribution correction. The relevant factors include the Fermi level, the linear background density of state, the temperature, the resolution and the constant background noise.

Basic Workflow:

1. Select and plot the desired data
    - **The Fermi Edge of the selected data should be around 0 eV.**
2. Find the figure number of the plot and input it into `Fig. Num` text area. Click "Get" to select an area in the figure, and the EDC of the selected area will appear in the lower left corner axes.
    - The Y Scale of the axes can be changed to `Linear` or `Log`. 
3. Select a Fit Mode
    > Mod 1: standard FDD <br>
    > Mod 2: FDD and constant background noise <br>
    > Mod 3: FDD with linear background density of states and constant background noise <br>
    > Mod 4: Resolution-convoluted FDD <br>
    > Mod 5: Resolution-convoluted FDD with linear background density of states and constant background noise **[recommand]** <br>
    > Mod 6: Resolution-convoluted FDD with linear background density of states and constant background noise; the temperature is set by the user <br>
    - usually, Mod 5 is the primary choice, which includes most factors
    - choose Mod 6 when you need to fix the temperature. 
4. Click the "Get Fit Area" button and select the energy range on the EDC to fit FDD.
    - When using Mod 6, input the temperature first and then click the button.
5. Wait for the results to come out. The fitted curve would appear in the axes shortly.
    - Check if the fitting is satisfying. Adjust the fitting area and repeat the process to achieve better results.
6. When the results are good enough, click "Offset & Renormalise" to apply the FDD correction.
    - The data should be selected in the list.

---
Contact: Cheng Peng <cheng.peng@physics.ox.ac.uk>