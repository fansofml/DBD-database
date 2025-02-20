# Doctor-SAM-Doctor Breast Cancer Analysis Dataset (DBD)

## Dataset Overview
The DBD dataset is a comprehensive collection of full-field digital mammography (FFDM) images sourced from screening, diagnostic, and follow-up examinations across the five campuses of the affiliated hospital. This dataset is designed to support research in breast cancer detection and analysis, providing a diverse range of mammographic images with detailed annotations.

## Dataset Composition
- **Total Cases**: 300 cases  
- **Image Count**: 1150 images  
  - 275 cases include two views (MLO and CC) per breast.  
  - 25 cases include two views of a single breast.  
- **Image Types**:  
  - Normal tissue  
  - Masses  
  - Calcifications  
  - Architectural distortions  
  - Asymmetries  
  - Multiple lesions  

## Key Features
1. **Masses**: Defined by three-dimensional presence and well-defined, convex edges, typically observable in both MLO and CC projections.  
2. **Calcifications**: Benign calcifications are larger and coarsely textured, while malignant calcifications are finer and smaller.  
3. **Architectural Distortions**: Localized disturbances in the mammographic pattern, often appearing star-shaped without an associated mass.  
4. **Asymmetries**: Categorized as size asymmetry (volume differences), focal asymmetry (localized areas), or global asymmetry (overall parenchymal discrepancies).  

## Dataset Structure
The dataset is organized into training and testing sets, with detailed annotations provided in CSV format. The structure is as follows:

### CSV File Structure
1. **Header**: Contains unique identifiers and encoding information.  
2. **Labels**: Indicates the benign or malignant status of the breast images.  
3. **ROI Count**: An integer representing the number of annotations within each image.  
4. **ROI File Paths**: JSON files containing labels and point sets for each image, stored in a unified directory.  
5. **Demographic Details**: Includes patient age at the time of imaging and family medical history.  

### Directory Structure

DBD-Dataset/
├── Training/
│   ├── Images/
│   ├── Annotations/
│   └── CSVs/
├── Testing/
│   ├── Images/
│   ├── Annotations/
│   └── CSVs/
├── README.md
└── LICENSE
