# A JPEG Data Hiding Method Based on AC Coefficient Selection and Grouping

**Guan-Zhong Su¹, Tung-Shou Chen¹, Wien Hong¹\***

¹ Department of Computer Science and Information Engineering, National Taichung University of Science and Technology, Taiwan

\* Corresponding Author: wienhong@nutc.edu.tw

## Abstract

JPEG images are widely transmitted across networks and preserve residual redundancy after compression, making them suitable as cover media for data hiding. However, existing JPEG data hiding methods typically embed data into specific or non-zero alternating current (AC) coefficients, which restricts flexible embedding across frequency regions and degrades image quality. This paper proposes a JPEG data hiding method based on coefficient selection and grouping. A non-consecutive-zero AC selection strategy is introduced to extract embeddable coefficients, allowing zero-valued ACs to participate in data embedding and increasing embedding capacity. A dynamic grouping mechanism is then designed to reorder and group coefficients according to their frequency distribution, ensuring that data are preferentially embedded into perceptually favorable regions. In addition, a modified exploiting modification direction (EMD) method is developed to embed a (2n+1)-ary digit by modifying at most one coefficient in each group. Experimental results show that, under a quality factor of 90, the proposed method achieves PSNR values above 56 dB when embedding 10,000 bits into 200 images, outperforming the best existing method by an average of 1.54 dB while maintaining high embedding capacity and low file size expansion.

**Keywords:** JPEG data hiding; AC coefficient grouping; Modified EMD embedding.

## Features

- Non-consecutive-zero AC selection
- Dynamic grouping mechanism (DGM)
- Modified exploiting modification direction (EMD)
- JPEG data embedding and extraction
- Embedding capacity estimation
- Image quality evaluation (PSNR and SSIM)

## Requirements

- Python 3
- Jupyter Notebook
- NumPy
- SciPy
- SymPy
- Matplotlib
- scikit-image
- jpegio

Install the required packages:

```bash
pip install numpy scipy sympy matplotlib scikit-image jpegio jupyter
```

## Usage

1. Open `main.ipynb` in Jupyter Notebook.
2. Specify the test image directory.
3. Configure the image name, quality factor, payload, and group size.
4. Execute the embedding and extraction sections.
5. Run the experiments to evaluate image quality under different payloads and group sizes.

### Example Configuration

```python
image_name = "Lena_Gray"
quality_factor = 70
test_image_dir = SOURCE_IMAGE_DIR
target_payload_bits = 10000
group_size = 3
```

The generated stego JPEG images are stored in the `Gray_image_stego/` directory. Ensure that this directory exists before running the embedding procedure.

## Citation

If you use this implementation in your research, please cite our paper:

G.-Z. Su, T.-S. Chen, and W. Hong, "A JPEG Data Hiding Method Based on AC Coefficient Selection and Grouping."

## Contact

For questions regarding the proposed method or its implementation, please contact the authors.

## Acknowledgments

This repository is provided for academic research and educational purposes.
