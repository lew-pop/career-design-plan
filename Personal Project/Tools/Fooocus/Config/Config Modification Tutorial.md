- You can modify your "/Fooocus/Fooocus/config.txt" using the below keys, formats, and examples.

- This file is a tutorial and example. Please edit "/home/lewpop/Dev Tools/Fooocus/Fooocus/config.txt" to change settings.

- Remember to split the paths with "\\" rather than "\", and there is no "," before the last "}". 

```
{
    "path_checkpoints": [
        "/home/lewpop/Dev Tools/Fooocus/Fooocus/models/checkpoints"
    ],
    "path_loras": [
        "/home/lewpop/Dev Tools/Fooocus/Fooocus/models/loras"
    ],
    "path_embeddings": "/home/lewpop/DevTools/Fooocus/Fooocus/models/embeddings",
    "path_vae_approx": "/home/lewpop/DevTools/Fooocus/Fooocus/models/vae_approx",
    "path_vae": "/home/lewpop/DevTools/Fooocus/Fooocus/models/vae",
    "path_upscale_models": "/home/lewpop//Fooocus/Fooocus/models/upscale_models",
    "path_inpaint": "/home/lewpop/Dev Tools/Fooocus/Fooocus/models/inpaint",
    "path_controlnet": "/home/lewpop/DevTools/Fooocus/Fooocus/models/controlnet",
    "path_clip_vision": "/home/lewpop//Fooocus/Fooocus/models/clip_vision",
    "path_fooocus_expansion": [
	    "/Fooocus/Fooocus/models/prompt_expansion/fooocus_expansion",
    ]
    "path_wildcards": "/home/lewpop/Dev Tools/Fooocus/Fooocus/wildcards",
    "path_safety_checker": "/home/lewpop//Fooocus/Fooocus/models/safety_checker",
    "path_sam": "/home/lewpop/Dev Tools/Fooocus/Fooocus/models/sam",
    "path_outputs": "/home/lewpop/Dev Tools/Fooocus/Fooocus/outputs",
    "temp_path": "/tmp/fooocus",
    "temp_path_cleanup_on_launch": true,
    "default_model": "realisticStockPhoto_v20.safetensors",
    "previous_default_models": [
        "realisticStockPhoto_v10.safetensors"
    ],
    "default_refiner": "None",
    "default_refiner_switch": 0.5,
    "default_loras_min_weight": -2,
    "default_loras_max_weight": 2,
    "default_loras": [
        [
            true,
            "SDXL_FILM_PHOTOGRAPHY_STYLE_V1.safetensors",
            0.25
        ],
        [
            true,
            "None",
            1.0
        ],
        [
            true,
            "None",
            1.0
        ],
        [
            true,
            "None",
            1.0
        ],
        [
            true,
            "None",
            1.0
        ]
    ],
    "default_max_lora_number": 5,
    "default_cfg_scale": 3.0,
    "default_sample_sharpness": 2.0,
    "default_sampler": "dpmpp_2m_sde_gpu",
    "default_scheduler": "karras",
    "default_vae": "Default (model)",
    "default_styles": [
        "Fooocus V2",
        "Fooocus Photograph",
        "Fooocus Negative"
    ],
    "default_prompt_negative": [
    	   "unrealistic, saturated, high contrast, 
    	    big nose, painting, drawing, sketch, cartoon, 
    	    anime, manga, render, CG, 3d, watermark, 
		    signature, label",    
    ]
    "default_prompt": "",
    "default_performance": "Speed",
    "default_image_prompt_checkbox": false,
    "default_enhance_checkbox": false,
    "default_advanced_checkbox": false,
    "default_developer_debug_mode_checkbox": false,
    "default_image_prompt_advanced_checkbox": false,
    "default_max_image_number": 32,
    "default_output_format": "png",
    "default_image_number": 2,
    "checkpoint_downloads": {
        "realisticStockPhoto_v20.safetensors": 
        "https: //huggingface.co/lllyasviel/fav_models/resolve/main/fav/ 
         realisticStockPhoto_v20.safetensors"
    },
    "lora_downloads": {
		"SDXL_FILM_PHOTOGRAPHY_STYLE_V1.safetensors": 
		"https://huggingface.co/mashb1t/fav_models/resolve/main/fav/ 
		 SDXL_FILM_PHOTOGRAPHY_STYLE_V1.safetensors"
    },
    "embeddings_downloads": {},
    "vae_downloads": {},
    "available_aspect_ratios": [
        "704*1408",
        "704*1344",
        "768*1344",
        "768*1280",
        "832*1216",
        "832*1152",
        "896*1152",
        "896*1088",
        "960*1088",
        "960*1024",
        "1024*1024",
        "1024*960",
        "1088*960",
        "1088*896",
        "1152*896",
        "1152*832",
        "1216*832",
        "1280*768",
        "1344*768",
        "1344*704",
        "1408*704",
        "1472*704",
        "1536*640",
        "1600*640",
        "1664*576",
        "1728*576"
    ],
    "default_aspect_ratio": "896*1152",
    "default_inpaint_engine_version": "v2.6",
    "default_selected_image_input_tab_id": "uov_tab",
    "default_uov_method": "Disabled",
    "default_controlnet_image_count": 4,
    "default_ip_image_1": null,
    "default_ip_type_1": "ImagePrompt",
    "default_ip_stop_at_1": 0.5,
    "default_ip_weight_1": 0.6,
    "default_ip_image_2": null,
    "default_ip_type_2": "ImagePrompt",
    "default_ip_stop_at_2": 0.5,
    "default_ip_weight_2": 0.6,
    "default_ip_image_3": null,
    "default_ip_type_3": "ImagePrompt",
    "default_ip_stop_at_3": 0.5,
    "default_ip_weight_3": 0.6,
    "default_ip_image_4": null,
    "default_ip_type_4": "ImagePrompt",
    "default_ip_stop_at_4": 0.5,
    "default_ip_weight_4": 0.6,
    "default_inpaint_advanced_masking_checkbox": false,
    "default_inpaint_method": "Inpaint or Outpaint (default)",
    "default_cfg_tsnr": 7.0,
    "default_clip_skip": 2,
    "default_overwrite_step": -1,
    "default_overwrite_switch": -1,
    "default_overwrite_upscale": -1,
    "example_inpaint_prompts": [
        "highly detailed face",
        "detailed girl face",
        "detailed man face",
        "detailed hand",
        "beautiful eyes"
    ],
    "example_enhance_detection_prompts": [
        "face",
        "eye",
        "mouth",
        "hair",
        "hand",
        "body"
    ],
    "default_enhance_tabs": 3,
    "default_enhance_uov_method": "Disabled",
    "default_enhance_uov_processing_order": "Before First Enhancement",
    "default_enhance_uov_prompt_type": "Original Prompts",
    "default_sam_max_detections": 0,
    "default_black_out_nsfw": false,
    "default_save_only_final_enhanced_image": false,
    "default_save_metadata_to_images": false,
    "default_metadata_scheme": "fooocus",
    "metadata_created_by": "",
    "default_invert_mask_checkbox": false,
    "default_inpaint_mask_model": "isnet-general-use",
    "default_enhance_inpaint_mask_model": "sam",
    "default_inpaint_mask_cloth_category": "full",
    "default_inpaint_mask_sam_model": "vit_b"
}
```