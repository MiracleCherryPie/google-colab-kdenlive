# google-colab-kdenlive
Render kdenlive project in google colab
### What's this?
This is just an jupyter notebook to help render Kdenlive project or any video editor project that uses melt to apply effects.
### But why?
Well, you can use this to render your video inside Google Colab (or even inside headless server running jupyter server).
### Pros:
1. You can render inside cloud environment
2. You can store render result in Google Drive without uploading it from your PC to Google Drive

### Cons:
1. No GPU-based rendering
2. This notebook is hard to use (even this notebook looks simple but you need to understand XML and MLTFramework a bit if an error occurs

### How-to:
1. Use any melt-compatible video editor. I suggest Kdenlive
2. Open your project and click render button (in Kdenlive, Go to Project > Render)
3. Choose any encoding presets (but don't choose any hardware-based encoding preset such as VA-API or NVENC)
4. Depend on your video editor, you can click Generate Script to generate .mlt file, the .mlt file should be located at /path/to/Videos/kdenlive-renderqueue/
5. Upload your .mlt file (and any other file such as video file, background music, etc.) to google colab from file manager
6. Follow instructions in the notebook to render your project
7. If the render result doesn't looks like as expected, fix it manually by editing .mlt file and provide correct path to your project file

### Disclaimer:
Google Colab still have [restrictions](https://research.google.com/colaboratory/faq.html#limitations-and-restrictions) and prioritized for machine learning purpose only. This notebook doesn't designed to render melt project with GPU.
