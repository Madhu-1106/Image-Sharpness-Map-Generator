# Image Sharpness Map Generator

This project focuses on analyzing how sharp or blurry different regions of an image are.  
As part of my internship/academic learning, I built a visualization tool that highlights image sharpness using the Laplacian operator. The idea is to help understand image clarity and detect blur patterns in a clear and visual way.



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

---

## Project Structure

Sharpness-Map-Generator/
│
├── src/
│ └── sharpness_map.ipynb # main script
│
├── samples/
│ └── example.jpg (any image with both clear and blur parts) # sample input image
│
├── outputs/
│ └── heatmap.png # sample output (sharpness heatmap generated)
│
├── README.md
└── requirements.txt


---

## How to Run

You can run this project in:
- **Google Colab**
- **Local Python environment**

### Steps:
1. Install dependencies:
   
   pip install -r requirements.txt

2. Upload an image in Colab or place it in the project folder.

3. Run the script to generate:

     *Original image

     *Grayscale version

     *Sharpness heatmap

     *Block-wise numeric heatmap

Output visuals will appear side-by-side for easy comparison.

** Why I Built This

As a final-year AIML student, I wanted to explore image processing concepts and understand how algorithms detect blur/sharpness.
This project helped me learn:

*Laplacian and edge-based sharpness detection

*Image normalization and smoothing

*Heatmap generation

*Python visualization (matplotlib & seaborn)


** Contributions

This is a learning-oriented project, but suggestions and improvements are always welcome.

** License

This project is open-source under the MIT License.
