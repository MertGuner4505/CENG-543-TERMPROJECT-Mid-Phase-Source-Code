Execution Environment

This project was developed and evaluated using Google Colab to reflect both cloud-scale training and edge-oriented deployment scenarios. The training phase was conducted under unconstrained GPU execution to simulate industry-scale cloud environments, while the evaluation phase was performed under CPU-only execution, restricted to a single core and a strict memory budget, in order to simulate edge-device deployment conditions. All Colab-specific setup, including Google Drive mounting and environment initialization, is handled inside the notebooks and not within project_core.py. The core module is environment-agnostic and can be reused outside Colab.

Running the Experiments (Google Colab)

To reproduce the experiments, open either MiniBERT_Experiment.ipynb or TinyBERT_Experiment.ipynb in Google Colab. Run the first cell to mount Google Drive using from google.colab import drive followed by drive.mount('/content/drive'). Ensure that project_core.py is accessible from the same Google Drive directory as the notebook, or update the import path accordingly. Execute the remaining cells sequentially to reproduce training and edge-device evaluation results.

Generative AI Disclosure

Generative AI tools were used in a limited, assistive capacity during the preparation of this repository, primarily for documentation formatting, organizational guidance, and code refactoring suggestions. All experimental design decisions, implementations, evaluations, and interpretations of results were conducted and validated by the author. Minor numerical variations may occur across runs due to the use of cloud-based execution environments; reported results reflect the configurations described in the accompanying paper.
