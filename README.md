# Supra-Rust 100M in the browser

The page now lives at https://lab-ietf.ayourt.ch/supra-rust/ (the model files are served from there, not from GitHub).

`page-index.html` is the page source. It loads wllama 3.8.1 (`esm/index.js`, `esm/wasm/wllama.wasm`, from npm) and a
q8_0 GGUF split in two parts under `model/`. A 100M-parameter base model continued-pretrained from
[SupraLabs/Supra2-100M-Instruct](https://huggingface.co/SupraLabs/Supra2-100M-Instruct) (Apache-2.0) on Rust,
IETF RFCs, fd.io VPP C, OpenStax textbooks and Stack Exchange math/physics Q&A. Credits and licenses are on the page.

Test switches on the page: `?compat=1` (hide JSPI, so wllama takes its Safari path), `?nocache=1`, `?clear=1`.
