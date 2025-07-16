WebGL Liquid Demo

A simple interactive WebGL liquid distortion effect built with Three.js, deployable on GitHub Pages and embeddable via <iframe> into no-code platforms like Webflow, Wix, Framer, etc.

Live Demo

After deployment, your demo will be available at:

https://<your-username>.github.io/webgl-liquid-demo/

Folder Structure

webgl-liquid-demo/
├── index.html            # Main demo file
└── assets/               # Place your custom images here
    └── your-image.jpg

Getting Started

Clone the repo

git clone git@github.com:<your-username>/webgl-liquid-demo.git
cd webgl-liquid-demo

Add your image

Copy your image file into the assets/ folder (e.g., assets/your-image.jpg).

Update the URL

Open index.html in your editor.

Locate the comment:

// REPLACE THIS URL with your own image URL
const imageURL = 'https://<your-username>.github.io/webgl-liquid-demo/assets/your-image.jpg';

Replace the URL inside the quotes with the path to your image in assets/.

Preview locally

Serve with a simple HTTP server to avoid CORS or file:// issues:

# Python 3:
python -m http.server 8000
# Or using npm:
npx serve .

Visit http://localhost:8000/ to see your effect.

Deploy to GitHub Pages

git add .
git commit -m "Add custom image"
git push -u origin main

Then go to GitHub Settings → Pages, select the main branch and / (root) folder, and save.

Embedding in No-Code Platforms

Use this simple <iframe> snippet in your platform’s embed or custom code widget:

<iframe
  src="https://<your-username>.github.io/webgl-liquid-demo/"
  width="100%"
  height="600"
  style="border:none;"
  allowfullscreen
></iframe>

Optionally, wrap with an aspect-ratio container for responsive height:

<div style="position:relative; width:100%; padding-top:(imageHeight/imageWidth*100)%">       
  <iframe src="..." style="position:absolute; top:0; left:0; width:100%; height:100%; border:none;"></iframe>
</div>

License

MIT License © Santi Sarapinas
