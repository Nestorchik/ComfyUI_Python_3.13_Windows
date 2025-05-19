# ComfyUI & Python_3.13 & Windows
"ComfuUI" + Python 3.13 + Windows

"ComfyUI" installation code for "Python-3.13" 

- mkdir c:\Test313
- cd /D c:\Test313
- git clone https://github.com/comfyanonymous/ComfyUI.git
- git clone https://github.com/Comfy-Org/ComfyUI-Manager.git c:\Test313\ComfyUI\custom_nodes\ComfyUI-Manager
- uv venv --python 3.13
- uv pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
- powershell Invoke-WebRequest -Uri "https://github.com/Nestorchik/Dzen/releases/download/dzen/sentencepiece-0.2.0-cp313-cp313-win_amd64.whl" -OutFile "sentencepiece-0.2.0-cp313-cp313-win_amd64.whl"
- uv pip install sentencepiece-0.2.0-cp313-cp313-win_amd64.whl
- uv pip install pip
- uv pip install numpy==2.2.5
- uv pip install -r c:\Test\ComfyUI\requirements.txt
- uv run c:\Test313\ComfyUI\main.py --windows-standalone-build --front-end-version Comfy-Org/ComfyUI_frontend@latest
- pause

**Install Log:**
![image](https://github.com/user-attachments/assets/49de38fe-ee25-4712-b40e-8f6ad59a48fa)

**Start & generation Log:**
![image](https://github.com/user-attachments/assets/72ff39a5-5a18-43e5-bda3-73223e2d1320)


