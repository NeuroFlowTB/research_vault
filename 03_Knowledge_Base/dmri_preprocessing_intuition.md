# dMRI Preprocessing Intuition

Diffusion MRI data are noisy, distorted, and motion-sensitive. Preprocessing exists to correct these problems before downstream analysis.

The main idea:

> dMRI preprocessing turns unstable measured signals into data that can be interpreted more safely.

## Problem to Correction Map

| Problem | Correction |
|---|---|
| Noise | Denoising |
| Subject movement | Motion correction |
| Gradient-related distortions | Eddy correction |
| Magnetic field warping | Susceptibility correction |
| Misalignment | Registration |

## Core Steps

### Denoising

Denoising reduces random signal fluctuations. This is important because diffusion signal can be weak, especially at higher b-values.

### Motion correction

Motion correction adjusts images when the subject moves during acquisition. Motion is especially problematic in dMRI because each volume can correspond to a different diffusion direction.

### Eddy correction

Eddy correction handles distortions caused by rapidly changing diffusion gradients. In FSL, this is handled by EDDY.

Important intuition:

> Eddy correction is central because diffusion gradients can distort the same data they help measure.

### Susceptibility correction

Susceptibility correction handles spatial warping caused by magnetic field inhomogeneities, especially in echo-planar imaging.

In FSL, TOPUP is commonly used for this when suitable reverse phase-encoding data are available.

### Registration

Registration aligns images to each other or to a reference space. This can be needed between diffusion images, structural MRI, and standard templates.

## Why Ordering Matters

Preprocessing is a workflow, not a list of independent buttons. Some steps depend on outputs from earlier steps, and some tools expect data in specific formats or acquisition layouts.

This matters for the thesis because an AI agent should reason about:
- which correction is needed
- which tool can perform it
- what inputs the tool requires
- what order the steps should happen in
- which ecosystem outputs can be reused by another ecosystem

## Related Notes

- [[dMRI_intuition|Diffusion MRI Intuition]]
- [[neuroimaging_ecosystems|Neuroimaging Ecosystems]]
