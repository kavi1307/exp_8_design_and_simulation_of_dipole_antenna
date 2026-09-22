# exp_8_design_and_simulation_of_dipole_antenna
4. **Assign the excitation:**
   - At the feed gap, create a small sheet/line and assign a **Lumped Port** (with an appropriate impedance line and resistance, typically 50 Ω) or a **Lumped RLC/Gap Source**.
5. **Create the radiation boundary:**
   - Draw an **air box** (vacuum) around the dipole, at least λ/4 away from the antenna in all directions.
   - Assign the outer surface of the air box as a **Radiation Boundary**.
6. **Set up the analysis:**
   - Add a **Solution Setup** with the solution frequency equal to the design frequency.
   - Add a **Frequency Sweep** (Fast/Interpolating) over the band of interest.
7. **Add radiation pattern reports:**
   - Insert a **Far Field Setup** (Infinite Sphere) to compute the 3-D radiation pattern.
8. **Validate and run the simulation** (Validation Check → Analyze All).
9. **Post-process the results:**
   - Plot **S11 (return loss)** vs frequency.
   - Plot **VSWR** vs frequency.
   - Plot the **2-D polar** and **3-D radiation patterns**.
   - Note the **gain**, **directivity** and **radiation efficiency** at the resonant frequency.

---

## Observations

<img width="1600" height="899" alt="WhatsApp Image 2026-09-07 at 13 33 42 (1)" src="https://github.com/user-attachments/assets/73b9755a-d8ed-432a-ac8c-89bed092f4df" />
<img width="1600" height="899" alt="WhatsApp Image 2026-09-07 at 13 33 42 (2)" src="https://github.com/user-attachments/assets/8721fe6b-e260-4abd-a979-0611c371f488" />



### Graphs

* S11 vs frequency
<img width="1600" height="899" alt="WhatsApp Image 2026-09-07 at 13 33 42" src="https://github.com/user-attachments/assets/940d2d45-9ab9-4e6f-82fb-d1caae76885d" />


* VSWR vs frequency
<img width="1600" height="899" alt="WhatsApp Image 2026-09-07 at 13 33 42 (4)" src="https://github.com/user-attachments/assets/c0ea32ae-add0-4925-8fb1-fede51a7cdbd" />

* 2-D E-plane and H-plane radiation patterns


<img width="1623" height="666" alt="Screenshot 2026-09-13 093541" src="https://github.com/user-attachments/assets/a5e1f18e-996a-47b7-bcef-11dd12605305" />


---

## Precautions

1. Ensure the radiation boundary is at least λ/4 away from the antenna structure on all sides to avoid reflection errors.
2. Mesh the model finely enough (especially near the feed gap) for accurate convergence.
3. Verify that the port impedance matches the intended feed impedance before analysing S11/VSWR.
4. Check for geometry validation errors before running the simulation.

## Result
 
Resonant Frequency = 2.4GHz  

Return loss = -20dB

VSWR = 1.22

Gain = 2.15DBI

## Conclusion
A half-wave dipole antenna was designed and simulated at ___2.4___ GHz using Ansys HFSS.
