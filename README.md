# Sean Lobjoit

Cloud and AI practitioner. Founder of [Perpetual Squared](https://perpetualsquared.com).

I help organisations cut through hype and build AI and cloud systems that actually work. I'm also the type of guy to spend a weekend figuring out how to run a 14B LLM on a laptop with soldered RAM and 8GB VRAM, just because it's an interesting opportunity to solve for.

## Enterprise

- Cloud architecture: AWS, GCP, Azure
- AI/LLM systems and agent frameworks
- Platform engineering and DevSecOps
- MLOps and AI infrastructure
- Enterprise architecture and cost optimisation at scale

## Projects

I work in a variety of domains professionally but in my spare time been looking into solving some hardware limitations I've run into:

- **[nbd-vram](https://github.com/c0dejedi/nbd-vram)** - a CUDA daemon that backs an NBD block device with GPU VRAM. Turns your graphics card into a multi-threaded swap device (~2.7 GB/s sequential read, ~310k random 4K IOPS under load). No kernel module, no P2P API - just dlopen(libcuda.so) and a Unix socket.
- **[llm-fit](https://github.com/c0dejedi/llm-fit)** - a LD_PRELOAD shim that routes CUDA allocations through unified memory and over-reports free VRAM, so Ollama/vLLM can fit more layers on the GPU. On an 8GB card with llama3.1:8b q8, 27 to 31 layers, performance goes from ~13 to ~22 tok/s.

## Writing

No-fluff takes on cloud strategy, AI architecture, and the decisions that separate good systems from great ones.

→ [seanlobjoit.com](https://www.seanlobjoit.com) · [LinkedIn](https://linkedin.com/in/seanlobjoit)
