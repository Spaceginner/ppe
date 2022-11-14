# Practical Prompt Engineering
## Contributors
- Spaceginner#7688 — put staff together, did absolutely nothing else to this project
- lorendovah#0644 — original idea
- Neural#9281, ᄅƎᴚIℲ∀⊥N∩W █▄ █▄█ █▀█ ▀█▀#9877 — contributed methods
## Disclaimer
All methods that are described here are possible in AUTOMATIC1111's WebUI. Names are taken from that WebUI, too. Also, this guide is not for the begginers, you can still read this document if you feel advanturous.
## Mission
Create a document (or series of documents) that demonstrate(-s) workflow best practices
## Methods
### Landscaping
#### Method contributed by Neural#9281
1. Start prompt with the `concept art of...` and stay less than 15 words (e.g. `concept art of an ancient island temple`), after generate 16 images with `Euler a` sampler and 10 samples.
2. Pick what you like best, send it to `img2img`, set 20 samples, then generate images, while changing denoising strenght, as well as adding words to the prompt based on what you want to add to the base image. You can also use `inpainting` to add things to the image.
3. Send final image from second step to Photoshop to "force" any color changes that you couldn't get.
4. Take that image back to `img2img` or `inpainting`, choose `DDIM` as a sampling method and play with it even more.
5. Repeat steps 3 to 4 until you are satisfied.
6. Send image that you got to `Extras` tab and upscale it in 4 times.
### Highres
#### Method contributed by ᄅƎᴚIℲ∀⊥N∩W █▄ █▄█ █▀█ ▀█▀#9877
1. Use `DPM++2M` sampler with auto gen for high speeds and easy prompt controling.
2. If you see anything that isn't right, change the prompt.
3. Once the prompt is perfected, choose `DPM++ 2s a karras` and 100 samples. Then turn on `Hires. fix` and set as a first pass res. `896x512` and as a final res. `2048x1152`
4. By leaving it on auto gen you can get plenty of images, which can be upscaled using Gigapixel AI to 8K (x4 upscaling). Note, by doing auto gen you can generate and upscale images at the same time in parallel.
5. Then, you can use `GIMP` or `ImageMagick` to convert images in `JPEG` standart with 80% quality, what will save you a space on a storage.
