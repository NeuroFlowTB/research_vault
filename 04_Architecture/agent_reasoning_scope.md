# Agent Reasoning Scope

The AI agent in this thesis should not only retrieve facts. It should reason over workflow knowledge.

## Target Reasoning Problems

The agent should help answer questions like:
- Which preprocessing steps are needed for this diffusion MRI dataset?
- Which tools can perform each step?
- What inputs does each tool require?
- What order should the steps happen in?
- Which outputs are compatible across ecosystems?
- What does the agent know, and what does it not know yet?

## Knowledge-Grounded Agent

A knowledge-grounded agent should base its answers on structured project knowledge rather than only on general language model memory.

Relevant knowledge types:
- tool capabilities
- tool inputs and outputs
- workflow dependencies
- acquisition metadata
- file formats
- known preprocessing problems
- ecosystem relationships

## Self-Knowledge-Aware Retrieval

Self-knowledge-aware retrieval means the agent should track whether its knowledge is sufficient for a question.

Useful behaviors:
- retrieve relevant notes before answering
- identify missing information
- ask for required metadata when needed
- avoid pretending that uncertain workflow details are known
- explain which knowledge source supports a recommendation

## Thesis Connection

The neuroimaging domain is a good test case because preprocessing decisions depend on structured constraints:
- data type
- acquisition parameters
- available metadata
- software ecosystem
- tool order
- compatibility between outputs and inputs

This makes dMRI preprocessing a strong domain for evaluating workflow reasoning in AI agents.
