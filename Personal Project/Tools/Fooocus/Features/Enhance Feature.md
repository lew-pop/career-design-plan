# Fooocus 2.5.0: Enhance
## What does this feature do?

- Enhance allows you to automatically upscale and/or improve parts of the picture based on either a prompt or an input image. It is comparable to ADetailer ([repository](https://github.com/Bing-su/adetailer)), but offers better and more flexible object detection and replacement with detection and replacement prompts instead of static detection models, each having ~140MB.

## How do i use it?

### Disclaimer

- It is highly recommended to use performance `Speed` or `Quality` (no performance which loads a LoRA) as any inpaint engine uses a LoRA, which may not produce the best results when combined with other performance LoRAs. Using inpaint mode `Improve Detail (face, hand, eyes, etc.)` does not set an inpaint engine, making it compatible with all performances. The documentation of inpaint modes can be found here: https://github.com/lllyasviel/Fooocus/discussions/414) All of this is also the case for normal inpainting without enhancements.

- ControlNets (`ImagePrompt`, `PyraCanny`, `CPDS`, `FaceSwap`) are currently not supported for enhance steps but can be used for image generation used as basis for enhance.

### With image generation

1. Generate any image with the settings you'd like to use
2. If you're satisfied, disable random seed and open the enhance tab  
    2.1. (optional) Enable and define order upscaling or variation (default disabled)  
    2.2. Enable and configure any amount of other improvement steps.  
    2.3. Input detection prompt (what you want to detect in the image)  
    2.4. Input positive / negative prompt (what you want to replace the detected masks with, defaults to your normal prompts if not set)
3. Generate image

### Based on an existing image

- Simply open Image Input and upload an image to the Enhance tab. Prompt processing will be skipped and only enhancement steps are processed. Follow steps 2+ above.  

- You may set `--enable-auto-describe-image` to automatically generate the prompt after image upload.

## Examples

![[Screenshot from 2024-08-02 13-12-12.png]]

![[Screenshot from 2024-08-02 13-03-36 1.png]]

**Above Images Zoomed In**

![[Screenshot from 2024-08-02 13-01-08.png]]

![[Screenshot from 2024-08-02 13-02-21.png]]

## Example Output

|[Original (generated)](https://gallery.mashb1t.de/gallery/-8ubXvDC-HwkxOv8Oem8cabO/vd1Wm0E8WZdNbimHmVzTXTR_)|Enhance|
|---|---|
|[![22732ab04379cb552d97ebf38de6](https://github.com/lllyasviel/Fooocus/assets/9307310/06aced0d-a967-4b58-ac5a-ae7fd5fbf62a)](https://github.com/lllyasviel/Fooocus/assets/9307310/06aced0d-a967-4b58-ac5a-ae7fd5fbf62a)|[![image - 2024-06-17T001252 624](https://github.com/lllyasviel/Fooocus/assets/9307310/33fd2d83-73c0-4192-b99e-515c39ae853f)](https://github.com/lllyasviel/Fooocus/assets/9307310/33fd2d83-73c0-4192-b99e-515c39ae853f)|

|Original (generated)|Upscale (before)|`#1` Yellow Sundress|`#2` Hands replacement|
|---|---|---|---|
|[![342070683-260e6a0b-5f42-47a3-83fd-fc3f4310d3a7](https://github.com/user-attachments/assets/f273197c-1c12-44a9-b097-ad2e77de643f)](https://github.com/user-attachments/assets/f273197c-1c12-44a9-b097-ad2e77de643f)|[![image](https://github.com/user-attachments/assets/41da80f2-7fbe-482a-b4ab-e60cf1c7954a)](https://github.com/user-attachments/assets/41da80f2-7fbe-482a-b4ab-e60cf1c7954a)|[![image](https://github.com/user-attachments/assets/c8d5cbe3-f7fb-4b96-924a-795ec3ef6a0e)](https://github.com/user-attachments/assets/c8d5cbe3-f7fb-4b96-924a-795ec3ef6a0e)|[![image](https://github.com/user-attachments/assets/bb20c49f-9d34-42b6-a451-996a8c41350c)](https://github.com/user-attachments/assets/bb20c49f-9d34-42b6-a451-996a8c41350c)|
