# KiCAD Checklist for relay-pcb

## Release Tasks
- [x] Add version variable on PCB
- [ ] K1 uses the stock JQC-3FF footprint (COM hole 1.3mm; the HF3FF datasheet asks for 1.5mm). Check that the COM pin fits on the first board

## Future Enhancements
- [ ] Add Cacophony logo
- [ ] Latching relay option to save battery when the relay is held on for long periods

## Pre-release checklist
- [ ] Check the M16 pinout against J202 on tc2-plugs-buck-boost-pcb (1 GND, 3 OUT_TX, 6 VOUT)
- [ ] Check the J1 connector gender and the cable to the camera
- [ ] Confirm the contact voltage/current needed on the isolated side (laid out with 3mm clearance)
- [ ] First board: check NC/NO with a meter with the relay off and on
