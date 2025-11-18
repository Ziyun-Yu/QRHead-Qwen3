## Installation

You can install all dependencies by running:
```bash
pip install -r requirements.txt
```

**Supported models**:
* `Llama-3.2-1B-Instruct`
* `Llama-3.2-3B-Instruct`
* `Llama-3.1-8B-Instruct`
* `Llama-3.1-70B-Instruct`
* `Qwen2.5-7B-Instruct`
* `Qwen3-4B-Instruct-2507`
* `Qwen3-32B`
* `Qwen3-Embedding-8B`

## Modifications

The following modifications have been made to extend support for Qwen3 series models:

1. **Custom Qwen3 Implementation**: Created `src/qrretriever/custom_modeling_qwen3.py` to enable Qwen3 series models' implementation.

2. **QR Head Configurations on FIRE Dataset**: Added QR head configurations tested on the [FIRE dataset](https://huggingface.co/papers/2407.11522) in `src/qrretriever/configs/`:
   - `Qwen3-4B-Instruct-2507_qr_head.yaml`
   - `Qwen3-32B_qr_head.yaml`
   - `Qwen3-Embedding-8B_qr_head.yaml`

3. **Modified `attn_retriever.py`**: Extended to support Qwen3 models.

4. **Dependencies**: Added `requirements.txt` with tested package versions.

## Credits

This is an extension of [princeton-pli/QRHead](https://github.com/princeton-pli/QRHead) to support Qwen3 series models. Part of the code is adapted from [In-Context-Reranking](https://github.com/OSU-NLP-Group/In-Context-Reranking).
