# Diffusion MRI Intuition

Diffusion MRI extends [[mri_fundamentals|MRI]] by measuring how water moves through tissue.

Unlike structural MRI, diffusion MRI is not mainly asking "what does this tissue look like?" It is asking "how does water move here, and does that movement have a preferred direction?"

## Core Concept

Water diffusion is affected by tissue structure. In white matter, water tends to diffuse more easily along fiber bundles than across them.

Mental model:

> White matter fibers guide water movement like microscopic tubes.

## Isotropic vs Anisotropic Diffusion

### Isotropic diffusion
Water moves equally in all directions.

This can happen in spaces where there is little directional structure.

### Anisotropic diffusion
Water moves more easily in one direction than others.

This is the foundational idea behind diffusion MRI, because directional diffusion can reveal information about white matter organization.

## b-values

A b-value controls how strongly the MRI sequence is sensitized to diffusion.

Intuition:
- higher b-value means stronger diffusion sensitivity
- higher b-value also means lower signal and more noise

## Why Multiple Gradient Directions Matter

One diffusion direction is not enough to estimate tissue orientation. Diffusion MRI uses multiple gradient directions so the scanner can sample water movement from different angles.

## Why dMRI Needs Heavy Preprocessing

Diffusion MRI is especially sensitive to:
- noise
- subject movement
- eddy current distortions
- susceptibility distortions
- image misalignment

This is why preprocessing is central to dMRI analysis, not just a cleanup step.

## Facts

- Diffusion MRI measures water diffusion in tissue.
- Water diffuses preferentially along white matter fibers.
- Directional diffusion is called anisotropy.
- Multiple gradient directions are needed to estimate diffusion orientation.
- Diffusion MRI needs heavy preprocessing because diffusion signals are noisy and easily distorted.

## Related Notes

- [[mri_fundamentals|MRI Fundamentals]]
- [[dmri_preprocessing_intuition|dMRI Preprocessing Intuition]]
- [[neuroimaging_ecosystems|Neuroimaging Ecosystems]]
