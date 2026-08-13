There are 4 target configurations relevant for standard production running. Currently, on the white board in the counting house they are written as:
- A.) 'full target': H2 gas in target cell and target chamber  (reads "RG-O Target: H2" on the beamline overview screen)
- B.) 'empty target': H2 gas in target chamber, none in the target cell. (reads "RG-O Target: Empty Cell" on the beamline overview screen)
- C.) 'all empty': Target cell is in the beamline, but there is no gas in the cell or chamber. On the beamline overview screen, currently this state is "undefined", but we will very soon up-date-the MCC status to read something like "NoGas" or "MT-MT". 
- D.) 'no target': The target ladder (containing the cell and aluminum/carbon sheets) is completely removed from the beamline. The beamline overview status will read "Out".

Below is the PRad-II Target overview screen under nominal full-target H2 operating conditions.
![[PRad-IITargetH2 1.pdf]]
The current status of the target is calculated from the position of the EV1/EV2 switches and the Y motor readback. 

Only EV1 or EV2 can be open at one time. 
When EV1 is open, and Y = 50796 (this is the nominal position for the cell as of May 7th 2026), the target status is H2. 
When EV2 is open, and Y = 50796, the status is Empty Cell.
When neither are opened, and Y = 50796, the status is "undefined" but we will have added a correct status by Monday May 11th. You can confirm to MCC that the status is fine and that you really are ready for beam.

When EV1/EV2 are closed, and Y = 4345241, the aluminum foil is in and the target is "Al".
When EV1/EV2 are closed, and Y = 5767473, the carbon foil is in and the target is "C".

## Changing Target Configurations
1. In the Flow Controller field, put the 'Flow set' to 0.

 ![[Pasted image 20260508194126.png]]
2. Close EV1 or EV2 if either are open. 
   ![[Pasted image 20260508194318.png|306]]
3. Move the Y position if necessary. If you need to move the position, call MCC to have them take away beam. Turn off the GEM HVs. Then, open the "Motion Controls" panel on the GUI. 
   ![[Screenshot 2026-05-08 at 19.45.38.png|466]]
   ![[Pasted image 20260508194916.png|534]]
4. On this screen, you can hit one of the buttons to move the target ladder motors to one of the 4 preset Y positions. 'Cell' is for nominal production running. 'Out' is to remove the target ladder from the target chamber. Configurations A-C use "Cell", only configuration "D" uses "Out". Once you have hit one of these buttons, return to the main screen. You should now see in the upper right the motor status for Y change from "STOPPED" to "MOVING". 
   ![[Pasted image 20260508195259.png|697]]
5. Once the target is in the correct position for your desired configuration, if you are running:
	- 'Configuration A'='Full Target'='H2', open EV1 and then set flow to 800 cc/m. Turn on the GEM HVs, call for beam back, and start the run.
    - 'Configuration B'='Empty'='Empty Cell', open EV2 and then set flow 800 cc/m. Turn on the GEM HVs, call for beam back, and start the run.
    - 'Configuration C'='all empty'= No Gas in Chamber OR Cell, but cell in beamline, turn on the GEM HVs, call for beam back, and start the run.
    - 'Configuration D' = OUT, or Carbon or Aluminum, turn on the GEM HVs, call for beam back, and start the run.