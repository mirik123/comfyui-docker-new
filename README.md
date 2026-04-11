# ComfyUI RunPod Template

A streamlined and feature-rich RunPod template for ComfyUI with an enhanced user interface, model management, and custom nodes.

### Ready for ComfyUI NSFW workflows:
- Wan2.2 Remix I2V v2.1 SVI2Pro Fully Automatic Reverse Long Video Workflow
- Wan2.2-Remix-I2V

### For importing custom models add env var:
MODELS_CONFIG_URL=https://raw.githubusercontent.com/poomshift/comfyui-docker-new/refs/heads/main/models_config.json

### Included models:
- vae
   - https://huggingface.co/Comfy-Org/Wan_2.1_ComfyUI_repackaged/resolve/main/split_files/vae/wan_2.1_vae.safetensors
- unet
   - https://huggingface.co/FX-FeiHou/wan2.2-Remix/resolve/main/NSFW/Wan2.2_Remix_NSFW_i2v_14b_high_lighting_fp8_e4m3fn_v2.1.safetensors
   - https://huggingface.co/FX-FeiHou/wan2.2-Remix/resolve/main/NSFW/Wan2.2_Remix_NSFW_i2v_14b_low_lighting_fp8_e4m3fn_v2.1.safetensors
   - https://huggingface.co/FX-FeiHou/wan2.2-Remix/resolve/main/NSFW/Wan2.2_Remix_NSFW_i2v_14b_high_lighting_v2.0.safetensors
   - https://huggingface.co/FX-FeiHou/wan2.2-Remix/resolve/main/NSFW/Wan2.2_Remix_NSFW_i2v_14b_low_lighting_v2.0.safetensors
- text_encoders
   - https://huggingface.co/Comfy-Org/Wan_2.1_ComfyUI_repackaged/resolve/main/split_files/text_encoders/umt5_xxl_fp8_e4m3fn_scaled.safetensors
   - https://huggingface.co/NSFW-API/NSFW-Wan-UMT5-XXL/resolve/main/nsfw_wan_umt5-xxl_fp8_scaled.safetensors
- loras
   - https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/LoRAs/Stable-Video-Infinity/v2.0/SVI_v2_PRO_Wan2.2-I2V-A14B_HIGH_lora_rank_128_fp16.safetensors
   - https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/LoRAs/Stable-Video-Infinity/v2.0/SVI_v2_PRO_Wan2.2-I2V-A14B_LOW_lora_rank_128_fp16.safetensors

### Included custom nodes:
- ComfyUI-Manager
- ComfyUI_essentials
- ComfyUI-VideoHelperSuite
- ComfyUI-KJNodes
- ComfyUI-WanVideoWrapper
- ComfyUI-PresetDownloadManager
- ComfyUI_Qwen3-VL-Instruct

### Qwen3-VL-Instruct Abliterated
https://github.com/IuvenisSapiens/ComfyUI_Qwen3-VL-Instruct/pull/69
   - huihui-ai/Huihui-Qwen3-VL-8B-Thinking-abliterated
   - huihui-ai/Huihui-Qwen3-VL-8B-Instruct-abliterated


### 🙏 Acknowledgements

- The template is based on https://github.com/poomshift/comfyui-docker-new
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) by comfyanonymous
- All custom node developers for their valuable contributions
- RunPod.io for the GPU cloud infrastructure
- For more information, visit [PromptAlchemist on Facebook](https://www.facebook.com/PromptAlchemist). 

### Building docker container
- `sed -i -e 's/\r$//' start.sh`
- `docker build --no-cache -t runpod-comfyui-wan .`
- `docker tag runpod-comfyui-wan repository/runpod-comfyui-wan`
- `docker push repository/runpod-comfyui-wan`

### Runpod template
https://runpod.io/gsc?template=4f33nox3uc
