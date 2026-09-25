# Diffusion Meta-Prompting (DMP) - Project Website

Official project page for "Diffusion Meta-Prompting and Steering for Generalizable Foundation Model Adaptation" (NeurIPS 2026).

## 🌐 Website Setup

This repository contains the source code for the DMP project webpage.

### Files Structure

```
dmp.github.io/
├── index.html           # Main webpage
├── style.css            # Stylesheet
├── DMP_NeurIPS_2026.pdf # Paper PDF (add this file)
├── images/              # Figures from the paper
│   ├── teaser.png
│   ├── method.png
│   ├── composite_results.png
│   ├── hierarchical_results.png
│   ├── variation_results.png
│   ├── composition.png
│   ├── negative_prompting.png
│   ├── generalization.png
│   └── README.md        # Guide for extracting images
└── README.md            # This file
```

### Setup Instructions

1. **Add the Paper PDF**
   - Copy your `DMP_NeurIPS_2026.pdf` file to the root directory

2. **Extract Figures**
   - Follow the instructions in `images/README.md` to extract figures from the PDF
   - Save them in the `images/` directory with the correct filenames

3. **Test Locally**
   - Open `index.html` in a web browser to preview the site
   - Check that all images load correctly

4. **Deploy to GitHub Pages**
   ```bash
   git add .
   git commit -m "Initial website setup"
   git push origin main
   ```
   - Go to your repository Settings → Pages
   - Set source to "main" branch
   - Your site will be live at: `https://[username].github.io/dmp.github.io/`

### Customization

- **Colors**: Edit the gradient in `style.css` (search for `#667eea` and `#764ba2`)
- **Content**: Modify `index.html` to add or remove sections
- **Add more figures**: Simply add images to the `images/` folder and reference them in the HTML

### Features

✅ Responsive design (mobile-friendly)
✅ Clean academic layout
✅ Smooth scrolling navigation
✅ Comparison tables
✅ Citation section with BibTeX
✅ Links to paper, code, and supplementary materials
✅ Professional color scheme

### Dependencies

The website uses:
- Font Awesome 6.0 (for icons) - loaded from CDN
- Pure HTML/CSS - no JavaScript required
- No build process needed

### Browser Compatibility

Tested and working on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📝 Citation

If you use this template or find our work useful, please cite:

```bibtex
@inproceedings{sridhar2026dmp,
  title={Diffusion Meta-Prompting and Steering for Generalizable Foundation Model Adaptation},
  author={Sridhar, Deepak and Li, Yi and Bhardwaj, Kartikeya and Liu, Shuangjun and Jing, Taotao and Li, Yuan and Zhang, Shuai and Lyu, Jiancheng and Gao, Dashan and Vasconcelos, Nuno},
  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
  year={2026}
}
```

## 👥 Authors

- **Deepak Sridhar** (UC San Diego) - desridha@ucsd.edu
- **Yi Li** (Qualcomm Technologies)
- **Kartikeya Bhardwaj** (Qualcomm Technologies)
- **Shuangjun Liu** (Qualcomm Technologies)
- **Taotao Jing** (Qualcomm Technologies)
- **Yuan Li** (Qualcomm Technologies)
- **Shuai Zhang** (Qualcomm Technologies)
- **Jiancheng Lyu** (Qualcomm Technologies)
- **Dashan Gao** (Qualcomm Technologies)
- **Nuno Vasconcelos** (UC San Diego)

## 📄 License

This project page template is available under MIT License. Feel free to use and modify.

## 🔗 Links

- Paper: [DMP_NeurIPS_2026.pdf](DMP_NeurIPS_2026.pdf)
- Code: Coming soon!
- Project Page: https://[your-username].github.io/dmp.github.io/

---

© 2026 Deepak Sridhar. All rights reserved.
