# MRI Fundamentals

## What is MRI?
Magnetic Resonance Imaging (MRI) creates detailed images of internal body structures using magnetic fields and radio waves.

It aligns protons that are normally randomly oriented. [1]

MRI measures signals from hydrogen nuclei after radiofrequency excitation. The scanner does not take a photograph; it measures signals and reconstructs images mathematically.

Mental model:

> MRI is signal measurement, not photography.

## What is not MRI ?
It is not X-rays, and it is not CT (computed tomography).

## Brain MRI
Used to visualize:
- brain anatomy
- tissue structure
- abnormalities

## Important Concepts

### Signal
MRI produces signals that are transformed into images.

### Voxel
A voxel is a 3D measurement unit. Each voxel contains averaged signal information from a small volume of tissue.

Mental model:

> Each voxel is a tiny noisy signal container.

### Noise
MRI data contains random noise that can reduce image quality.

### Artifacts
MRI images may contain distortions or acquisition artifacts.

### Contrast
Different tissues appear differently depending on imaging parameters.

### T1-weighted MRI
In T1-weighted images:
- white matter is usually brighter
- CSF is usually dark

### T2-weighted MRI
In T2-weighted images:
- CSF is bright
- fluid-related changes are more visible

Main takeaway:
Different tissues produce different signal intensities depending on the acquisition.

## Why Preprocessing Exists
Raw MRI data is imperfect and often requires correction before analysis.

Preprocessing is needed because MRI data can contain:
- noise
- motion artifacts
- magnetic field distortions
- reconstruction artifacts
- misalignment between images or modalities

These problems matter even more in [[dMRI_intuition|diffusion MRI]], because diffusion images are directional, noisy, and sensitive to distortion.

## Questions
- How is diffusion MRI different from standard MRI?
- Which artifacts are most important in dMRI?

## Facts

- MRI measures signals emitted by hydrogen nuclei after radiofrequency excitation.
- Different tissues relax differently, creating image contrast.
- MRI images are reconstructed mathematically from measured signals.
- Preprocessing exists because MRI signals are noisy and distorted by motion and magnetic effects.


## Sources 
- [1][MRI  Basics](https://case.edu/med/neurology/NR/MRI%20Basics.htm?)
- [ 2 ] [Magnetic Resonance Imaging (MRI)](https://www.nibib.nih.gov/science-education/science-topics/magnetic-resonance-imaging-mri)
- [3][Magnetism - Questions and Answers ​in MRI](https://mriquestions.com/how-does-fmri-work.html?)
