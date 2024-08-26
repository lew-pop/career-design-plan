Inpainting/Outpainting Settings in Fooocus:

![[inpaint-1.png]]

This “Fooocus Inpaint” is not only a user-friendly UI but also an algorithm production. Fooocus uses its own algorithm DPMPP Fooocus inpaint, and also uses Fooocus's own control model to minimized the influence to the style of base models. The method is partially inspired by [Diffusion-based semantic image editing with mask guidance](https://openreview.net/forum?id=3lge0p5o-M-).

In the entire open source community of SDXL, the Fooocus is the only software that allows you to use control-model-based inpaint with arbitary base models.

Note that this method, in general, expects processing generated images with unchanged or minorly changed prompts. We encourage users to drag image like this:

![[inpaint-2.png]]

# Inpaint Example

![[inpaint-3.png]]
![[inpaint-4.png]]
# Outpaint Example

Use the pan to outpan

![[inpaint-5.png]]
# Advanced: Detail Fix (face, hand, eyes, ...)

From time to time, you may get images like this:
![[inpaint-6.png]]

Everything is perfect, but the eyes / faces are just annoying:
![[inpaint-7.png]]
Now you can fix details like this:
![[inpaint-8.png]]

Note that this interface also allows you to add some prompts just for this inpaint pass. If you are too lazy, you can also use the shortcuts here:
![[inpaint-9 1.png]]
![[inpaint-10.png]]
Another example:

before:
![[inpaint-11.png]]
after:
![[inpaint-12.png]]
# Advanced: Add New Objects / Change Background

You can always add new objects just using default setting. But if the modification is too large, a better idea is to use
![[inpaint-13 1.png]]
For example:
![[inpaint-14.png]]
Change Background:

This "modification" mode will completely ignore original content and is good at handling images with solid color backgrounds like
![[inpaint-15.png]]
![[inpaint-16.png]]

# Very Advanced: Multiple-pass inpaint

You can first use general inpaint to get the image, drag the image to inpaint input again, and then change the mode to "Improve Detail" and then inpaint again. In this way you will get extremely high quality result. (Improve Detail can be used to improve details of anything, not only faces or hands).