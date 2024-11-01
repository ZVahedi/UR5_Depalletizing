# UR5_Depalletizing
This repository contains aURscript code for a UR5e robot to perform a de-palletizing task. It is a depalletizing program, meaning the parts are picked from a pallet and placed in front of the worker/participant. After selecting the "depalletizing" in the Wizard section of the Polyscope.

Originally developed in Polyscope, hence it is presented in a text file here. This script demonstrates robot motion planning, gripper control, and logic for item handling in a pallet pattern.

This code is designed for an assembly task when the worker receives the part by a robot. Since the required time for performing the task is Depending on the complexity of the step, the worker needs various timing. Based on this structure, the robot waits after picking the first, 3rd, 5th, and the 6th ones.

The pallet has six rows and six columns. This code is structured in the way to follow the above-mentioned timing for each row. Hence, `total_1_layer := 6 * 1` is defined as the number of parts in one row and on each if condition, a different part is considered.
