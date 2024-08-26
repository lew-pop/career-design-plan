### Wildcards

- Example prompt: `__color__ flower`

- Processed for positive and negative prompt.

- Selects a random wildcard from a predefined list of options, in this case the `wildcards/color.txt` file. The wildcard will be replaced with a random color (randomness based on seed). You can also disable randomness and process a wildcard file from top to bottom by enabling the checkbox `Read wildcards in order` in Developer Debug Mode.

- Wildcards can be nested and combined, and multiple wildcards can be used in the same prompt (example see `wildcards/color_flower.txt`).

### Array Processing

- Example prompt: `[[red, green, blue]] flower`

- Processed only for positive prompt.

- Processes the array from left to right, generating a separate image for each element in the array. In this case 3 images would be generated, one for each color. Increase the image number to 3 to generate all 3 variants.

- Arrays can not be nested, but multiple arrays can be used in the same prompt. Does support inline LoRAs as array elements!

### Inline LoRAs

- Example prompt: `flower <lora:sunflowers:1.2>`

- Processed only for positive prompt.

- Applies a LoRA to the prompt. The LoRA file must be located in the `models/loras` directory.