# dMRI Tools

This folder documents diffusion MRI tools as structured workflow knowledge.

The goal is not only to describe tools, but to make their inputs, outputs, assumptions, dependencies, and interoperability explicit enough for agent reasoning.

## Folder Structure

```text
02_dMRI_Tools/
├── 00_Templates/
│   ├── tool_template.md
│   ├── ecosystem_template.md
│   └── workflow_template.md
├── 01_Ecosystems/
│   ├── FSL/
│   ├── MRtrix3/
│   ├── TORTOISE/
│   └── QSIPrep/
├── 02_Preprocessing_Steps/
├── 03_Workflows/
├── 04_Interoperability/
└── 05_Evaluation/
```

## How to Use This Folder

Use `01_Ecosystems/` for software ecosystems and individual tools.

Use `02_Preprocessing_Steps/` for problem-centered notes such as denoising, eddy correction, susceptibility correction, and registration.

Use `03_Workflows/` for ordered pipelines.

Use `04_Interoperability/` for compatibility between ecosystems, file formats, metadata, and handoff points.

Use `05_Evaluation/` for criteria that test whether a tool, workflow, or AI agent recommendation is correct.

## Standard Tool Questions

Every tool note should answer:

- What problem does this tool solve?
- Which ecosystem does it belong to?
- What inputs does it require?
- What outputs does it produce?
- What assumptions does it make?
- Where does it sit in the preprocessing order?
- Which tools can run before it?
- Which tools can run after it?
- Which metadata are required?
- What failure modes or edge cases matter?
- What should an AI agent know before recommending it?

## Related Notes

- [[dmri_preprocessing_intuition|dMRI Preprocessing Intuition]]
- [[neuroimaging_ecosystems|Neuroimaging Ecosystems]]
- [[agent_reasoning_scope|Agent Reasoning Scope]]
