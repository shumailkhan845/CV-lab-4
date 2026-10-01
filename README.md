# CV-lab-4
### 1. Why is Gaussian filtering applied before Canny detection?

Gaussian filtering is applied to reduce noise and small unwanted variations in the skin image before edge detection. This helps Canny focus on important intensity changes, such as the boundary between the lesion and surrounding skin, and reduces false edges caused by image noise.

### 2. How did the three Canny threshold settings affect the result?

The three threshold settings produced different amounts of detected edges. The **50–100** setting detected more edges, including some unwanted noise and small details. The **100–200** setting produced a cleaner and more balanced edge map. The **150–250** setting detected fewer edges and could miss weaker parts of the lesion boundary.

### 3. Which threshold produced the best lesion boundary?

The **100–200 threshold** produced the clearest overall lesion boundary in this experiment. It provided a good balance between removing unwanted edges and preserving the important boundary of the lesion.

### 4. Why are edges useful for detecting skin lesions?

Edges represent locations where image intensity or color changes significantly. A skin lesion often has a visible transition between the lesion and surrounding skin, so detecting these edges can help identify and locate the lesion boundary.

### 5. What problems did you observe in detecting the lesion boundary?

Some images had weak or unclear lesion boundaries because the lesion and surrounding skin had similar intensity or color. Noise, hair, skin texture, shadows, and uneven illumination also produced unwanted edges. In some cases, the detected edges were incomplete, making it difficult to obtain a single closed contour.

### 6. How could your method be improved?

The method could be improved by using better preprocessing and segmentation techniques. Hair and other artifacts could be removed before edge detection, and adaptive thresholding could be used instead of fixed Canny thresholds. More advanced morphological operations, active contours, or segmentation models could also produce more accurate lesion boundaries. Testing the method on a larger number of images would provide a more reliable evaluation.
