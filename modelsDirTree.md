# models directory structure

```text
[665G]  models/
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
├── [ 25G]  Qwen3-30B-A3B-Instruct-2507/
│   └── [ 25G]  Qwen3-30B-A3B-Instruct-2507-UD-Q6_K_XL.gguf
├── [ 61G]  Qwen3-Coder-Next/
│   ├── [5.7M]  Qwen3-Coder-Next-UD-Q6_K_XL-00001-of-00003.gguf
│   ├── [ 47G]  Qwen3-Coder-Next-UD-Q6_K_XL-00002-of-00003.gguf
│   └── [ 15G]  Qwen3-Coder-Next-UD-Q6_K_XL-00003-of-00003.gguf
├── [ 64G]  Qwen3-Next-80B-A3B-Thinking/
│   ├── [ 46G]  Qwen3-Next-80B-A3B-Thinking-UD-Q6_K_XL-00001-of-00002.gguf
│   └── [ 17G]  Qwen3-Next-80B-A3B-Thinking-UD-Q6_K_XL-00002-of-00002.gguf
├── [ 21G]  Qwen3-VL-30B-A3B-Thinking/
│   ├── [1.0G]  mmproj-F16.gguf
│   └── [ 20G]  Qwen3-VL-30B-A3B-Thinking-UD-Q5_K_XL.gguf
├── [ 20G]  Qwen3-VL-32B-Instruct/
│   ├── [1.1G]  mmproj-F16.gguf
│   └── [ 19G]  Qwen3-VL-32B-Instruct-UD-Q4_K_XL.gguf
├── [5.5G]  Qwen3-VL-4B-Thinking/
│   ├── [797M]  mmproj-F16.gguf
│   └── [4.7G]  Qwen3-VL-4B-Thinking-UD-Q8_K_XL.gguf
├── [8.1G]  Qwen3-VL-8B-Instruct/
│   ├── [1.1G]  mmproj-F16.gguf
│   └── [7.0G]  Qwen3-VL-8B-Instruct-UD-Q6_K_XL.gguf
├── [8.1G]  Qwen3-VL-8B-Thinking/
│   ├── [1.1G]  mmproj-BF16.gguf
│   └── [7.0G]  Qwen3-VL-8B-Thinking-UD-Q6_K_XL.gguf
└── [8.7G]  translategemma-12b-it-i1/
    ├── [7.9G]  translategemma-12b-it.i1-Q5_K_M.gguf
    └── [815M]  translategemma-12b-it.mmproj-f16.gguf

 665G used in 26 directories, 48 files
```
