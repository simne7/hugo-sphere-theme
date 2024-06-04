# Create Screenshot

1. Dev Tools: set ".section {padding-bottom: 0}" to reduce padding between sections
2. Screenshot for style1
3. Set style in config.toml
4. Screenshot for style2
5. Repeat for other styles
6. Crop main area and sidebar: `convert -crop "1920x3480+960+84" style1.png 1.png`
7. Crop sidebar only: `convert -crop "468x3480+2412+84" style2.png 2.png`
8. Repeat for other styles
9. Append cropped images: `convert +append *.png append.png`
10. Crop to 3:2 screenshot: `convert -quality 80 +repage -crop "4260x2840+0+0" append.png screenshot.jpg`
11. Resize to thumbnail: `convert -resize 900x600 screenshot.jpg tn.jpg`

(Based on 3840x3894px screenshots)
