# FULL_SUBTRACTOR

**AIM:**
To simulate and synthesis full subtractor using vivado.

**APPARATUS REQUIRED:**

vivado 2023.2 software.

**PROCEDURE:**

STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

**Truth Table and Circuit Diagram**

![301805585-351addef-f7bb-4862-9817-616a41b4c882](https://github.com/pullurur/FULL_SUBTRACTOR/assets/161436550/395944f8-344b-4c79-9d04-b3e6109703c8)

![301805633-906152b8-63bc-4f70-9132-6b6b4420b22d](https://github.com/pullurur/FULL_SUBTRACTOR/assets/161436550/563bc18c-1189-450a-8409-ec3c14227513)

![301805678-7d480140-153a-4a7e-a6d2-5323c6bd4974](https://github.com/pullurur/FULL_SUBTRACTOR/assets/161436550/5397e2f1-c8a8-41d2-9ca1-e9556257be56)


**VERILOG CODE:**

module full_sub(a,b,bin,diff,borrow);

input a,b,bin;

output diff,borrow;

wire w1,w2,w3;

xor g1(w1,a,bin);

and g2(w2,~a,b);

xor g3(diff,w1,bin);

or g4(borrow,w2,w3);

and g5(w3,~w1,bin);

endmodule

**OUTPUT:**

![318266330-9e20d613-eddd-4ca2-a5b5-0df57ce7d984](https://github.com/pullurur/FULL_SUBTRACTOR/assets/161436550/3c5f6a77-45cc-4d79-9aab-057942d2ff7d)


**RESULT:**

Thus the verilog program for decoder has been simulated and verified successfully.
