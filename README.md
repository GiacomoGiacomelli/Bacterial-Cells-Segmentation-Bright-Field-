# Bacterial-Cells-Segmentation-Bright-Field 
Semi automated bacterial cells segmentation and binary mask construction in absence of phase constrast (optimized for Elyra7 images)

NOTE: the binary masks obtained from the combination of the two macros contained within this repository require manual refining.

Fiji macro 1 (Binary Mask):
- Input: Bright field/Phase contrast image
-Output: Binary Mask (scaled 10 times, bicubic interpolation)
-Output format: .tif , .txt

Fiji macro 2 (Watershed):
-Input: Binary Mask (.tif)
-Manual input required: Select area that needs watersheding
-Output: Binary Mask, selected area changes to watersheded version (Can be applied multiple times to different areas within the binary mask - used to segmentate cells)
-Output format: Requires manual save once satisfied with manual changes (.tif)
