Methodology:
Here’s a clean methodology (bullet points) for both assignments you can write in report/practical file.

🔵 Assignment-1 Methodology

Learning PDF using parameterized model

Step-1: Data Collection

Download air quality dataset from Kaggle.

Select NO₂ concentration as feature (x).

Remove missing values from dataset.

Step-2: Compute transformation parameters

Use university roll number 
𝑟
r.

Calculate:

𝑎
𝑟
=
0.05
×
(
𝑟
 
m
o
d
 
7
)
a
r
	​

=0.05×(rmod7)

𝑏
𝑟
=
0.3
×
(
𝑟
 
m
o
d
 
5
+
1
)
b
r
	​

=0.3×(rmod5+1)

Step-3: Transform variable

Apply nonlinear transformation:

𝑧
=
𝑥
+
𝑎
𝑟
sin
⁡
(
𝑏
𝑟
𝑥
)
z=x+a
r
	​

sin(b
r
	​

x)

This generates transformed variable 
𝑧
z.

Step-4: Estimate probability density

Assume Gaussian-like PDF:

𝑝
^
(
𝑧
)
=
𝑐
 
𝑒
−
𝜆
(
𝑧
−
𝜇
)
2
p
^
	​

(z)=ce
−λ(z−μ)
2

Compute histogram of transformed data.

Use curve fitting or estimation technique to learn parameters:

𝜆
λ (spread)

𝜇
μ (mean)

𝑐
c (scaling constant)

Step-5: Parameter learning

Fit PDF to histogram data.

Optimize parameters using curve fitting.

Obtain best values of λ, μ and c.

Step-6: Visualization

Plot histogram of transformed variable z.

Plot learned PDF curve on same graph.

Compare actual vs predicted distribution.

Step-7: Final Output

Report transformation parameters: ar, br

Report learned PDF parameters: λ, μ, c
<img width="636" height="485" alt="image" src="https://github.com/user-attachments/assets/2d2218ca-1195-4f63-b4c9-04f19a336156" />
<img width="653" height="92" alt="image" src="https://github.com/user-attachments/assets/447d2b66-0832-4535-8f6a-91388c20f4f0" />
