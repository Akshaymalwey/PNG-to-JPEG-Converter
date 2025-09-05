# PNG-to-JPEG-Converter
This project implements a simplified version of the JPEG compression pipeline from scratch.
It takes a PNG image as input, splits it into 8×8 blocks, applies Discrete Fourier Transform (DFT), then compresses it using quantization, zig-zag traversal, and run-length encoding (RLE).


Converts PNG images into JPEG-like compressed format.
Implements core JPEG concepts without external compression libraries.
Uses:
8×8 block processing
Discrete Fourier Transform (DFT)
Luminance Quantization Table
Zig-Zag traversal of coefficients
Run-Length Encoding (RLE)
Produces reduced-size images with controlled quality loss.

Compression Workflow
Image Splitting → Break the image into 8×8 blocks.
DFT Transformation → Convert each block into frequency space.
Quantization → Apply luminance quantization table to reduce precision.
Zig-Zag Traversal → Reorder coefficients for efficient encoding.
Run-Length Encoding (RLE) → Compress consecutive zeros.
(Optional) Entropy Coding → Could be extended with Huffman coding.
Reconstruction → Decompression reverses these steps

