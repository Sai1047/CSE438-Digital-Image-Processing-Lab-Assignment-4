# CSE438-Digital-Image-Processing-Lab-Assignment-4

# Custom Weighted Filter on Grayscale Image

This project applies a custom 3×3 weighted filter to a black and white image fetched from a URL. The filter is applied in two ways: manually using NumPy and via OpenCV's `cv2.filter2D` function. The goal is to validate manual convolution against OpenCV’s built-in implementation.

## Filter Kernel

The custom filter used is:
[1, 1, 1]

[1, 2, 1]

[1, 1, 1]

It is normalized by dividing by the sum of its weights (10) to preserve brightness.

## Steps

1. Load a grayscale image from a URL.
2. Define and normalize the custom kernel.
3. Apply the filter manually using nested loops.
4. Apply the same kernel using OpenCV’s `filter2D`.
5. Display the original, manual, and OpenCV-filtered images side by side.

## Output

- **Original Image**: The unaltered grayscale image.
- **Manual Filtered**: Output after applying the filter manually.
- **cv2.filter2D**: Output after applying the same filter using OpenCV.

The outputs are visually similar, confirming the correctness of the manual implementation.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- Pillow
- Requests
