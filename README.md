# REDEDIT
# REDEditing: Relationship-Driven Precise Backdoor Poisoning on Text-to-Image Diffusion Models
---
> This paper presents a novel backdoor attack method for on T2I diffusion model based on model editing, which is recise, stealthy, and cost-effective. Our approach, called REDEditing, achieves inserting backdoor on diffusion model such as Stable Diffusion v2.1. This repository provides the code to reproduce the results and use the proposed method.


## Environment Setup

To run the code, you need to set up the following environment:

### Prerequisites

- Python 3.8+
- PyTorch 2.0
- CUDA 11.7
- Other dependencies listed in `REDEditing_requirements.txt`

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/ysl-05/REDEditing
   cd your-repo-name
   ```
###
2. Install the required dependencies:
```bash
pip install -r REDEditing_requirements.txt
```
###
3. How to Training
>To train the model on Stable Diffusion v2.1, run the following command:

```bash
python train_backdoor.py --concepts 'your_trigger' --guided_concepts 'your_poison' --base '2.1'
```
4. Evaluation
To evaluate the trained model on the test set, use:

```bash
python generate_image.py --model path/to/your_backdoor_model
```
