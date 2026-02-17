# Configured llama.cpp in a folder

## get models

Models are saved in gguf in the `models` subfolder. Configuration and parameters are in [models.ini](models.ini).

[Current list of files](modelsDirTree.md). Made with:

```sh
echo -e "# models directory structure\n\n\`\`\`text\n$(tree -h --du --dirsfirst -F models)\n\`\`\`" > modelsDirTree.md
```

## run engine

ROCm and Vulkan docker containers configured in [compose.yaml](compose.yaml).

Run with:

```sh
docker compose up -d
```

Logs with:

```sh
docker logs llamacpp-r
#or
docker logs llamacpp-v
```

## use it

Built-in WebUI and all APIs are under `http://localhost:8083/` for Vulkan or `http://localhost:8080/` for ROCm.
