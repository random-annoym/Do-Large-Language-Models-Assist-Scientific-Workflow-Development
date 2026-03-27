# Do-Large-Language-Models-Assist-Scientific-Workflow-Development-
The replication package contains the complete prompt sets, benchmark workflow metadata, model outputs, evaluation summaries, and supporting materials required to inspect and reproduce the study. The repository is organized by study phase and workflow system to facilitate navigation and independent verification.


We evaluate three LLMs:
- **GPT-4o**
- **Gemini 2.5 Flash**
- **DeepSeek-V3**

The package includes:
- benchmark workflow list,
- fundamental prompts,
- background questions for Galaxy and Nextflow,
- workflow-specific background prompts,
- workflow-generation prompts,
- LLM outputs,
- evaluation summaries,
- and supporting materials used in the paper.

## Repository Structure

- `paper/` — paper PDF and related materials  
- `benchmark/` — benchmark workflow list and metadata  
- `prompts/` — all prompts used in the study  
- `llm_outputs/` — model responses organized by model and task  
- `evaluation/` — rubric, summaries, and reviewer notes  
- `workflow_references/` — GTN and nf-core reference workflow information  
- `docs/` — reproduction instructions  

## Workflow Systems

Our benchmark covers workflows from two widely used, expert-curated sources:
- **Galaxy Training Network (GTN)**
- **nf-core**

These workflows are used as strong community baselines for comparison.

## Reproducibility

The replication package provides the complete prompt sets, generated outputs, and evaluation materials needed to inspect and understand the study.  
Detailed reproduction instructions are available in `docs/reproduction_guide.md`.

For validation, we used:
- **Galaxy**: `https://usegalaxy.org/`
- **Nextflow**: GitHub Codespaces with the official Nextflow training environment

## Notes

Several benchmark workflows were curated after the training period of the evaluated LLMs, reducing the likelihood of prior exposure.  
We also note that workflows from different online sources are not always correct; therefore, this study evaluates whether LLMs can generate workflows that are accurate, executable, and aligned with expert-curated community standards.
