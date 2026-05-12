# Neuroimaging Ecosystems

Modern neuroimaging pipelines are compositional. A workflow may combine tools from multiple ecosystems rather than staying inside one software package.

Example:

FSL EDDY -> MRtrix3 tractography -> QSIPrep orchestration

The thesis focuses on reasoning across these ecosystems: tools, dependencies, ordering constraints, and interoperability.

## FSL

Role:
- classic preprocessing ecosystem
- widely used diffusion MRI toolbox

Important tools:
- TOPUP
- EDDY
- DTIFIT
- TBSS
- BedpostX
- ProbtrackX

Mental model:

> Robust traditional diffusion toolbox.

## MRtrix3

Role:
- advanced diffusion analysis
- tractography
- flexible pipelines

MRtrix3 is often combined with FSL.

Mental model:

> Advanced tractography ecosystem.

## TORTOISE

Role:
- specialized diffusion preprocessing
- robust correction workflows

Mental model:

> Highly specialized preprocessing framework.

## NiPreps / QSIPrep

Role:
- orchestration framework
- reproducible workflows
- BIDS-based preprocessing

QSIPrep can combine tools from:
- FSL
- MRtrix3
- ANTs
- DIPY

Mental model:

> Workflow orchestration ecosystem.

## Interoperability Questions

- Which file formats does each tool expect?
- Which metadata are required?
- Which outputs from one ecosystem can be used by another?
- Which preprocessing steps are duplicated across ecosystems?
- Which tools are wrappers around other tools?
- What assumptions does each tool make about acquisition data?
