# Cyclic Tensile Test Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jJQlW4wBg_2Gf00Zuq0MDDVkDpR5o60_?usp=sharing)

A Python notebook for automated analysis of cyclic tensile test data from <span style="color:red">**Instron-generated CSV files**</span>, providing key mechanical properties and generating stress-strain visualizations.

## Features

- Automatic cycle identification and segmentation
- Calculation of mechanical properties:
  - Hysteresis energy
  - Elastic (Young's) modulus
  - Stress and strain ranges
- Signal-to-noise ratio assessment
- Customizable stress-strain curve visualization
- Choice of integration methods for hysteresis calculations

## Input Requirements

The notebook accepts <span style="color:red">**Instron-generated CSV files**</span> with the following columns:
- Time (s)
- Displacement (mm)
- Force (kN)
- Tensile strain (%)
- Tensile stress (MPa)

## Usage

1. Click the "Open in Colab" badge above
2. Run all cells using `Runtime > Run all`
3. Upload your CSV file when prompted
4. Select your preferred:
   - Integration method (Shoelace or Trapezoidal)
   - Color scale for visualization (Grayscale, Maroon, or Gold)

## Outputs

- Stress-strain plots with cycle-based coloring
- CSV file containing cycle statistics:
  - Signal-to-noise ratio
  - Hysteresis energy
  - Elastic modulus
  - Stress/strain ranges

## Important Notes

<span style="color:pink">**Note: If any of the cycles in your data have a signal-to-noise ratio of < 13 dB, you need to treat these calculations with caution and independently verify their accuracy.**</span>

## Author

Created by <span style="color:cyan">**Logan Hessefort**</span> at the <span style="color:gold">Center for Sustainable Macromolecular Materials and Manufacturing, Arizona State University</span>. Supported by NSF EFRI award #213218.

## Contact
- [LinkedIn Profile](https://www.linkedin.com/in/logan-hessefort/)

## Disclaimer

Users should independently verify calculations. The author assumes no responsibility for any errors arising from the use of this notebook.
