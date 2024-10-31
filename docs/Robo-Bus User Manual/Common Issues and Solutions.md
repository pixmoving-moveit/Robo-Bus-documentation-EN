# Frequently Asked Questions (FAQ)

This section compiles various common issues related to the chassis and their solutions. If the problems are not resolved by this document, please contact the relevant technical personnel.

**Q: The chassis cannot drive, and the remote control shows no alarms.**

A: 
1. Check if the power battery has sufficient charge.
2. Check if all emergency stop switches are released.
3. Confirm that the handbrake is off.
4. Ensure the vehicle is in remote control mode.
5. Confirm that the brakes are properly released and check if the vehicle can be pushed.
6. Check if the motor controller's high-voltage power supply is normal.
7. Inspect the fuse box for the motor controller's wake-up power relay to ensure it is functioning properly.

---

**Q: The chassis will not power on.**

A: 
1. Check if all emergency stop switches are released.
2. Check if the 12V battery is discharged.
3. Inspect the fuses in each fuse box for any issues.
4. Check if the low-voltage fuse box has power.
5. Verify that the VCU power supply is normal.
6. Check for short circuits or disconnections in the CAN bus.

---

**Q: The remote control displays SOC = 0%.**

A: 
1. Check for any other alarms on the remote control. If there are any, refer to Appendix 1: "Remote Control Fault Code Analysis and Troubleshooting Suggestions" for resolution.
2. Check the power battery level of the chassis and charge it if necessary.
3. Inspect the 12V battery for discharge, as this may prevent the power battery from outputting power. Charge the battery if needed.
4. Verify that all fuses in the fuse boxes are intact and check for short circuits or disconnections in the wiring.
5. Read the chassis CAN messages and contact technical support for assistance.

---

**Q: The chassis cannot charge.**

A: 
1. Confirm the charging sequence: plug in the charging gun first, then connect to the 220V power supply.
2. Check if the main switch (knob switch, if available) is turned on. The system will not charge if the main switch is off.
3. Check the status of the charger indicator lights to confirm the charging state (red light flashing slowly means charging; green light solid means charging completed).
4. Inspect the charging line for any short circuits or disconnections.
5. Read the chassis messages and contact technical support for assistance.

---

**Q: The chassis steering is ineffective.**

A: 
1. Check if there are any alarms on the remote control and troubleshoot according to the fault code.
2. Verify that the handbrake and braking systems are functioning correctly and that the low-voltage power supply is normal.
3. Check if the 12V battery is discharged.
4. Inspect the fuse box to ensure no fuses are blown.
5. Check the steering motor relay to confirm it is not damaged and validate by cross-checking.

---

**Q: The chassis brakes are ineffective.**

A: 
1. Check if there are any alarms on the remote control and troubleshoot according to the fault code.
2. Verify that the handbrake and steering systems are functioning correctly and that the low-voltage power supply is normal.
3. Check if the 12V battery is discharged.
4. Inspect the fuse box to ensure no fuses are blown.
5. Check the braking relay to confirm it is not damaged and validate by cross-checking.

---

**Q: The chassis handbrake is ineffective.**

A: 
1. Check if there are any alarms on the remote control and troubleshoot according to the fault code.
2. Verify that the braking and steering systems are functioning correctly and that the low-voltage power supply is normal.
3. Check if the 12V battery is discharged.
4. Inspect the fuse box to ensure no fuses are blown.
5. Check the handbrake relay to confirm it is not damaged and validate by cross-checking.

---

**Q: Abnormal communication on the CAN port.**

A: 
1. Check if there are any alarms on the remote control and confirm that other functions of the chassis are normal, and the VCU is operating correctly.
2. Use a multimeter in voltage mode to measure the voltage on pins 2 and 7 of the CAN port. The negative should connect to the chassis ground. Under normal conditions, pin 2 should have a low voltage (around 2.25V) and pin 7 should have a higher voltage (around 2.75V). If the voltages are normal, check the other end of the CAN connection.
3. If the voltage is abnormal, trace the CAN line to check for short circuits or disconnections.

---

**Q: Remote control startup abnormal handling.**

A: After the vehicle powers on successfully, the remote display will show "Ready" at the bottom. If it fails to power on, the vehicle will not enter "Ready" mode. Check for a triangle exclamation mark above "Ready." If there is none, the driver can operate the vehicle. If there is an exclamation mark, it indicates that there is a fault with the vehicle. The driver should press the Display Switch button to toggle the display to the second screen and view specific system faults. For further troubleshooting, connect through the OBD interface to the vehicle’s CAN network to read detailed fault codes. The vehicle can only be driven after resolving the faults.