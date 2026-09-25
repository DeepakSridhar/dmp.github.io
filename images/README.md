# Images Directory

This directory should contain the following figures extracted from the paper:

## Required Images:

1. **teaser.png** - Figure 1 from page 2 showing the comparison of DMP vs existing approaches
   - Shows: Few-shot prompt tuning, Prompt retrieval, and Ours (DMP) with their pros/cons

2. **method.png** - Figure 4 from page 16 (Appendix) showing the DMP framework
   - Left: Text-to-Prompt Synthesis
   - Right: Prompt Variation Synthesis

3. **composite_results.png** - Table 4 from page 7 showing composite classification results
   - 55 dataset pairs classification accuracy

4. **hierarchical_results.png** - Figure 2 from page 8 showing Mean Treecut Accuracy
   - Bar chart comparing CoOp, BPL, and DMPCoOp

5. **variation_results.png** - Figure 3 from page 8 showing generalization of DMPVariation
   - Comparison of TI vs DMP for various prompts

6. **composition.png** - Figure 17 from page 29 showing identity composition
   - Scale 9.0 to 10.0 composition results

7. **negative_prompting.png** - Figure 9 from page 24 showing negative prompting examples
   - DMP-Negative Prompting (SD-RV) results

8. **generalization.png** - Figure 16 from page 29 showing cross-context generalization
   - TI vs DMP comparison across different contexts

## How to Extract Images from PDF:

You can extract these images from `DMP_NeurIPS_2026.pdf` using one of these methods:

### Method 1: Using a PDF tool
- Open the PDF in Adobe Acrobat or Preview
- Take screenshots of the relevant figures
- Save them with the names listed above

### Method 2: Using command line (if you have pdftoppm installed)
```bash
pdftoppm -png -r 300 DMP_NeurIPS_2026.pdf images/page
```

Then crop and rename the specific figures.

### Method 3: Manual export
- Use an online PDF to image converter
- Extract the specific pages
- Crop and save the figures

## Image Specifications:
- Format: PNG (preferred) or JPG
- Resolution: 300 DPI minimum for best quality
- Size: Optimize for web (under 500KB each if possible)
