# MRE sample dataset


The following datasets contain displacement field acquired from MRE:

1.	Homogeneous phantom data(phantom_homogeneous/)
2.	Phantom data with two embedded objects, one soft and one hard (phantom_inclusion/)
3.	Brain data with Meningioma. （brain_tumor/） with t1w map
4.	Healthy liver data. (liver_healthy/)
5.	Liver data with hepatic siderosis & cirrhosis (liver_Iron_deposition/)
6.	Liver data with tumour (liver_tumor/)


All dataset were acquired using a 3T scanner (uMR790, United Imaging Healthcare, Shanghai, China). MRE was implemented using a single-shot spin-echo echo-planar imaging sequence (TR/TE = 4000/65ms) with a motion-encoding gradient of 40 mT/m.

In each folder, three mat files were included:

### W_*.mat 
- W:unwrapped complex displacement array
- - with 5 dimensions:| dim_x | dim_y | dim_z | displacement direction | frequency |
- - dim_x, dim_y, dim_z are the dimensions for the 3 axes
- - displacement direction contains the 3 displacement components Ux, Uy, Uz
- - frequency corresponds to the frequency 
- dxyz: pixel resolution (m)
- Freq_list: frequency list (Hz)

### G_*.mat
- G:  shear modulus calcualted by TWENN [2]

### mag_*.mat
- mag:  magnitude of MRE image


If you use these datasets for your research, please cite the following papers:

[1] Qiu, S., He, Z., Wang, R., Li, R., Zhang, A., Yan, F., & Feng, Y. (2021). An electromagnetic actuator for brain magnetic resonance elastography with high frequency accuracy. NMR in Biomedicine, 34(12), 1–17. https://doi.org/10.1002/nbm.4592, 

[2] Ma, S., Wang, R., Qiu, S., Li, R., Yue, Q., Sun, Q., Chen, L., Yan, F., Yang, G.-Z., & Feng, Y. (2023). MR Elastography With Optimization-Based Phase Unwrapping and Traveling Wave Expansion-Based Neural Network (TWENN). IEEE Transactions on Medical Imaging, 42(9), 2631–2642. https://doi.org/10.1109/TMI.2023.3261346

[3] Qiu, S., He, Z., Wang, R., Li, R., Jin, W., Chen, L., … Feng, Y. (2024). Indirect Shear Wave Excitation for Brain Magnetic Resonance Elastography with Minimal Cerebral Blood Flow Alteration. IEEE Transactions on Biomedical Engineering, PP, 1–9. https://doi.org/10.1109/TBME.2024.3381708

Any questions, please contact:  fengyuan@sjtu.edu.cn
