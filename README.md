# Image-Sharpness-Map-Generator
The Image Sharpness Map Generator analyzes the clarity of an image by computing pixel-level and region-level sharpness. It visualizes how sharp or blurry different parts of an image are using the Laplacian operator, providing both heatmaps and numerical sharpness maps for detailed inspection.  This tool can be used for image quality assessment.

## What the Project Does

The script generates two types of visual outputs:

### 1. Sharpness Heatmap (Color Visualization)
- Converts the image to grayscale  
- Applies Laplacian to measure sharpness  
- Smooths the result and visualizes it using the JET colormap  
- This gives a clear heatmap showing sharp (red/yellow) and blurry (blue) regions

### 2. Numeric Block-wise Sharpness Map
- Divides the image into small blocks  
- Calculates sharpness value for each block  
- Plots it as a heatmap with numbers  
- Useful for analysis, ML preprocessing, or image quality evaluation

### Run Commands
1. Clone the repository
git clone <https://github.com/Madhu-1106/Image-Sharpness-Map-Generator.git>
cd Sharpness-Map-Generator

2. Install dependencies
   
pip install -r requirements.txt

4. Launch the Jupyter Notebook
   
jupyter notebook sharpness_map.ipynb

6. Load input image
   
Place images inside:

Input Imgs/
(Notebook reads the image path directly.)

5. Execute all cells
   
Run → Run All

This generates:
Sharpness heatmap
Block-wise numerical sharpness map
Output files stored in:

outputs/

--- Optional: If asked about running in Colab

Upload sharpness_map.ipynb
Upload an image into /content/Input Imgs/
pip install -r requirements.txt
Run all cells
