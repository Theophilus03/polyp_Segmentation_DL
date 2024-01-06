# Polyp Segmentation
A deep learning project to perform sematic segmentation on polyps in the human colon. Those models will be train on keras framework and evaluated using accuracy, IoU, and DICE Coef. ([paper](https://drive.google.com/file/d/11NF4abFCOKHoWRK2QfGyVbnSLwJjP-Dq/view?usp=sharing))

# Result
<img width="386" alt="Result" src="https://github.com/Theophilus03/polyp_Segmentation_DL/assets/114735443/00ba93cf-68a7-422a-914d-b344d80d1f92">

# Workflow
## Data Collection
The dataset we used in this study is the [Kvasir-SEG dataset from](https://datasets.simula.no/kvasir-seg/). The Kvasir-SEG dataset is an open access dataset that includes 1000 images and corresponding segmentation masks that are manually annotated and verified by experienced gastroenterologists.

## Data Preprocessing
  - Decode image and mask
  - resize image and mask to 256x256
  - expand_dims image and mask
    
## Data Splitting
  - 80% Trainning
  - 10% Testing
  - 10% Validating
    
## Train Model
  - Unet
  - Meta-Polyp
  - Meta-Polyp + CRF
  - Meta-Polyp + TTA
  - Meta-Polyp + CRF + TTA

## Result (Model Evaluation)
<img width="508" alt="image" src="https://github.com/Theophilus03/polyp_Segmentation_DL/assets/114735443/ba0bab06-8855-4ab2-8563-ea24a221cf34">
