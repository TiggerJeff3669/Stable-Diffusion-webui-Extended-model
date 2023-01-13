# Stable Diffusion webui for Colab & Import external models

# English | [繁體中文](./docs/README-cht.md)

This repo will guide you how to add more pre-trained model (checkpoint) to your Colab project.

## Prologue
automatic1111's webui project provide Stable Diffusion environment<br>
Not only default V1.4 model,there is more creative model by other user,<br>
So, how to import these models that we can use? 

# Before getting start
As we know, Colab free version provide GPU and storage with no guarantee, but Tesla T4 & 10~12GB RAM and up to 90GB storage space at least.
<br> **"Beware storage usage."**


# Requirement
 * An Google account for colab.
 * Mount Drive permission. (Optional)
 * PixelDrain account. (Optional)

# Where models saved?
I'm upload models to PixelDrain (not affiliated)<br>
It can keep file 60 days then detele. (If nobody access it.)<br>
Connect speed 6~20MB/s by cUrl in colab. (If i found better file sharing host)

# How to import models

```
Model
curl -Lo <name>.ckpt <path/to/PixelDrain/Link>
Vae weight
curl -Lo <name>.vae.pt <path/to/PixelDrain/Link>
```
\<name> is same as model named, like `stable-diffusion-V1.4-puned.ckpt`. <br>
\<path/to/PixelDrain/Link> is "https://pixeldrain.com/api/file/`your-shared-link`?download"
 <br> In my Jupyter Notebook, it's `Anything-V3.0` merge `dbMai` by me (I recommend it!)

 # Feature 
 My jupyter Notebook allow you export output images as zip to Google Drive (generated by yyyy-mm-dd-H-m.zip)

 # More Infomation
Here is some models list. <br>
https://rentry.org/sdmodels
