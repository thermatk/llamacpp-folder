# My selfhosted AI stack
+ One folder for everything
+ Works on my machine ™️. Main targets are:
	+ GNU/Linux (Arch/Debian/Ubuntu/CachyOS)
	+ GPU acceleration via ROCm/Vulkan
+ Main tools:
    - [llama.cpp](https://github.com/ggml-org/llama.cpp)
    - [audio.cpp](https://github.com/0xShug0/audio.cpp)
    - [ComfyUI](https://github.com/comfy-org/comfyui)

## get models

Models are to be saved, mostly in [gguf](https://huggingface.co/docs/hub/gguf), in the `models`, `audiomodels` and `comfymodels` subfolders.

[Current list of files](modelsDirTree.md). Made with:

```sh
echo -e "# models directory structure\n\n\`\`\`text\n$(tree -h --du --dirsfirst -F models audiomodels comfymodels)\n\`\`\`" > modelsDirTree.md
```

Configuration and parameters for llama.cpp [router mode](https://github.com/ggml-org/llama.cpp/blob/master/tools/server/README.md#model-presets) are in [models.ini](models.ini).

## run

Most containers configured in [compose.yaml](compose.yaml).

+ llama.cpp
    - ROCm, llamacpp-r [http://localhost:8080](http://localhost:8080)
    - Vulkan, llamacpp-v [http://localhost:8083](http://localhost:8083)
    - CPU, llamacpp-c [http://localhost:8082](http://localhost:8082)
+ llama.cpp - linked to ministack of models [minimodels.ini](minimodels.ini)
    - Vulkan, llamacpp-t-v [http://localhost:8093](http://localhost:8093)
    - CPU, llamacpp-t-c [http://localhost:8092](http://localhost:8092)
+ audio.cpp at [http://localhost:8081](http://localhost:8081)
+ [Open WebUI](https://github.com/open-webui/open-webui) at [http://localhost:8070](http://localhost:8070)

Run with:

```sh
docker compose up -d
```

Logs with:

```sh
docker logs llamacpp-r
```
and so on.

### ComfyUI
Subfolder `comfyui-rocm-docker`.

Build image with:

```sh
docker compose build
```

Run with:

```sh
docker compose up -d
```

Available at [http://localhost:8182](http://localhost:8182)