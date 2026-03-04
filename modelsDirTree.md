# models directory structure

```text
[586G]  models/
├── [605M]  bge-m3/
│   └── [605M]  bge-m3-Q8_0.gguf
├── [ 11G]  gemma-3-12b-it/
│   ├── [9.8G]  gemma-3-12b-it-UD-Q6_K_XL.gguf
│   └── [815M]  mmproj-BF16.gguf
├── [ 19G]  gemma-3-27b-it-qat/
│   ├── [ 18G]  gemma-3-27b-it-qat-UD-Q5_K_XL.gguf
│   └── [818M]  mmproj-F16.gguf
├── [4.1G]  gemma-3-4b-it/
│   ├── [3.3G]  gemma-3-4b-it-UD-Q6_K_XL.gguf
│   └── [812M]  mmproj-BF16.gguf
├── [6.2G]  gemma-3n-E4B-it/
│   └── [6.2G]  gemma-3n-E4B-it-UD-Q6_K_XL.gguf
├── [ 95G]  GLM-4.5-Air/
│   ├── [ 46G]  GLM-4.5-Air-UD-Q6_K_XL-00001-of-00003.gguf
│   ├── [ 46G]  GLM-4.5-Air-UD-Q6_K_XL-00002-of-00003.gguf
│   └── [2.1G]  GLM-4.5-Air-UD-Q6_K_XL-00003-of-00003.gguf
├── [ 93G]  GLM-4.6V/
│   ├── [ 46G]  GLM-4.6V-UD-Q6_K_XL-00001-of-00002.gguf
│   ├── [ 45G]  GLM-4.6V-UD-Q6_K_XL-00002-of-00002.gguf
│   └── [1.6G]  mmproj-F16.gguf
├── [9.9G]  GLM-4.6V-Flash/
│   ├── [8.3G]  GLM-4.6V-Flash-UD-Q6_K_XL.gguf
│   └── [1.7G]  mmproj-F16.gguf
├── [ 24G]  GLM-4.7-Flash/
│   └── [ 24G]  GLM-4.7-Flash-UD-Q6_K_XL.gguf
├── [1.7G]  GLM-OCR/
│   ├── [906M]  GLM-OCR-Q8_0.gguf
│   └── [829M]  mmproj-GLM-OCR-f16.gguf
├── [ 59G]  gpt-oss-120b/
│   ├── [ 12M]  gpt-oss-120b-mxfp4-00001-of-00003.gguf
│   ├── [ 30G]  gpt-oss-120b-mxfp4-00002-of-00003.gguf
│   └── [ 29G]  gpt-oss-120b-mxfp4-00003-of-00003.gguf
├── [ 11G]  gpt-oss-20b/
│   └── [ 11G]  gpt-oss-20b-mxfp4.gguf
├── [ 11G]  gpt-oss-20b-heretic-v2/
│   └── [ 11G]  gpt-oss-20b-heretic-v2.i1-MXFP4_MOE.gguf
├── [498M]  granite-docling-258M/
│   ├── [316M]  granite-docling-258M-bf16.gguf
│   └── [181M]  mmproj-model-f16.gguf
├── [ 59G]  kldzj_gpt-oss-120b-heretic-v2/
│   ├── [ 37G]  kldzj_gpt-oss-120b-heretic-v2-MXFP4_MOE-00001-of-00002.gguf
│   └── [ 22G]  kldzj_gpt-oss-120b-heretic-v2-MXFP4_MOE-00002-of-00002.gguf
├── [ 20G]  Magistral-Small-2509/
│   ├── [ 19G]  Magistral-Small-2509-UD-Q6_K_XL.gguf
│   └── [837M]  mmproj-F16.gguf
├── [ 20G]  Mistral-Small-3.2-24B-Instruct-2506/
│   ├── [ 19G]  Mistral-Small-3.2-24B-Instruct-2506-UD-Q6_K_XL.gguf
│   └── [837M]  mmproj-F16.gguf
├── [1.3G]  PaddleOCR-VL-1.5/
│   ├── [1.8K]  chat_template_llama.jinja
│   ├── [841M]  mmproj-PaddleOCR-VL-1.5.gguf
│   └── [475M]  PaddleOCR-VL-1.5-Q8_0.gguf
├── [ 25G]  Qwen3.5-27B/
│   ├── [885M]  mmproj-F16.gguf
│   └── [ 24G]  Qwen3.5-27B-UD-Q6_K_XL.gguf
├── [ 31G]  Qwen3.5-35B-A3B/
│   ├── [858M]  mmproj-F16.gguf
│   └── [ 30G]  Qwen3.5-35B-A3B-UD-Q6_K_XL.gguf
├── [4.5G]  Qwen3.5-4B/
│   ├── [641M]  mmproj-F16.gguf
│   └── [3.9G]  Qwen3.5-4B-UD-Q6_K_XL.gguf
├── [9.0G]  Qwen3.5-9B/
│   ├── [876M]  mmproj-F16.gguf
│   └── [8.2G]  Qwen3.5-9B-UD-Q6_K_XL.gguf
├── [ 61G]  Qwen3-Coder-Next/
│   ├── [5.7M]  Qwen3-Coder-Next-UD-Q6_K_XL-00001-of-00003.gguf
│   ├── [ 47G]  Qwen3-Coder-Next-UD-Q6_K_XL-00002-of-00003.gguf
│   └── [ 15G]  Qwen3-Coder-Next-UD-Q6_K_XL-00003-of-00003.gguf
└── [8.7G]  translategemma-12b-it-i1/
    ├── [815M]  mmproj-translategemma-12b-it.f16.gguf
    └── [7.9G]  translategemma-12b-it.i1-Q5_K_M.gguf

 586G used in 25 directories, 48 files
```
