# Regional_Volume_estimation
The Project: Develop a method for estimating the dynamic and static volume at an independent sagittal location from a 4D Dynamic MRI image, 
For using the integration between the Yolo and SAM2, please download the model sam2_hiera_large from https://github.com/facebookresearch/sam2

Project Structure
│
├── run/
│   └── Contains the pretrained YOLO model and scripts used for lung detection and segmentation.
│

├── analysis/
│   └── Contains signal processing and analysis modules, including:
│       • EE–EI (End-Expiration and End-Inspiration analysis)
│       • EMD (Empirical Mode Decomposition)
│       • Filtering methods for respiratory signal extraction and noise reduction
│

├── sam2/
│   └── Contains the implementation and execution scripts for the SAM2 model,
│       which performs detailed lung segmentation using the YOLO-generated regions.
│

├── Sample_MRI/
│   └── Sample free-breathing MRI datasets used for testing and validation.
│       The dataset consists of 2D sagittal MRI time-series images with a
│       temporal resolution of approximately 350 ms between consecutive frames.
│

└── Sample_Mask/
    └── Contains segmentation masks generated from the corresponding MRI images.

        These masks represent the lung regions extracted by the segmentation pipeline. 

