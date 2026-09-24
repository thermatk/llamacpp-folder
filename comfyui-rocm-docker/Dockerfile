FROM python:3.14-slim

ENV DEBIAN_FRONTEND=noninteractive \
    PYTHONUNBUFFERED=1 \
    PIP_NO_CACHE_DIR=1 \
    PYTHONDONTWRITEBYTECODE=1

# Basic system dependencies
RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    ca-certificates \
    build-essential \
    libgl1 \
    libglib2.0-0 \
    libgomp1 \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /opt

# Clone ComfyUI
RUN git clone --depth 1 \
    https://github.com/Comfy-Org/ComfyUI.git \
    /opt/ComfyUI

WORKDIR /opt/ComfyUI


# Install exact ROCm/PyTorch nightly stack.
# https://github.com/Comfy-Org/ComfyUI/issues/15436
# alternative: pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/rocm10.0
COPY requirements-rocm.txt /tmp/requirements-rocm.txt
RUN pip install -r /tmp/requirements-rocm.txt

# Install other ComfyUI dependencies
RUN pip install -r requirements.txt


# Install ComfyUI-GGUF
RUN git clone --depth 1 \
    https://github.com/molbal/ComfyUI-GGUF.git \
    /opt/ComfyUI/custom_nodes/ComfyUI-GGUF \
    && pip install \
    -r /opt/ComfyUI/custom_nodes/ComfyUI-GGUF/requirements.txt

# Persistent directories
RUN mkdir -p \
    /opt/ComfyUI/user

EXPOSE 8188

WORKDIR /opt/ComfyUI

CMD ["python", "main.py", "--listen", "0.0.0.0", "--port", "8188"]
