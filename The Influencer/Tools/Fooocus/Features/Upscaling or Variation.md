Before First Enhancement

- always use original prompts for upscaling or variation
- improved details when enhancing due to larger canvas size
- less context of image composition due to inpainting with 1024x1024
- recommended for enhancing smaller areas (details, faces, eyes)

After Last Enhancement

- may apply changes to the image which were already fixed by enhance
- recommended for enhancing large areas (backgrounds, clothes, whole persons)
- choose which prompt to use for upscaling or variation, use either original prompts or last filled enhancement prompts with non-empty value (increases subject recognition, prevents subject from being changed back to original prompt after enhancement. Use this when substantially changing the subject described in the original prompts)


|Original (generated)|Upscale (before)|Enhance|
|---|---|---|
|[![image](https://github.com/user-attachments/assets/d6a5ff85-2766-4e5d-b025-4d3243150e13)](https://github.com/user-attachments/assets/d6a5ff85-2766-4e5d-b025-4d3243150e13)|[![image](https://github.com/user-attachments/assets/5dd16d65-47c5-4cd7-9448-57415719f7da)](https://github.com/user-attachments/assets/5dd16d65-47c5-4cd7-9448-57415719f7da)|[![image](https://github.com/user-attachments/assets/94a4a975-4187-49dd-9907-648ed342281d)](https://github.com/user-attachments/assets/94a4a975-4187-49dd-9907-648ed342281d)|

|Original (generated)|Enhance|Upscale (after)|
|---|---|---|
|[![image](https://github.com/user-attachments/assets/502894b2-55a9-42a5-b03a-ba60e5bbdcaf)](https://github.com/user-attachments/assets/502894b2-55a9-42a5-b03a-ba60e5bbdcaf)|[![image](https://github.com/user-attachments/assets/2cbadb44-cdb3-4899-a998-82bdd7d519d1)](https://github.com/user-attachments/assets/2cbadb44-cdb3-4899-a998-82bdd7d519d1)|[![image](https://github.com/user-attachments/assets/45a4fed7-47da-4156-a5bc-a002bb13fe77)](https://github.com/user-attachments/assets/45a4fed7-47da-4156-a5bc-a002bb13fe77)|