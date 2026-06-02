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

- **[nbd-vram](https://github.com/c0dejedi/nbd-vram)** - CUDA daemon that backs an NBD block device with GPU VRAM. Turns your graphics card into a 1.3 GB/s swap device. No kernel module, no P2P API - just `dlopen(libcuda.so)` and a Unix socket.
- **[llm-fit](https://github.com/c0dejedi/llm-fit)** - LD_PRELOAD hook that redirects `cudaMalloc` to `cudaMallocManaged`. Hypothesis: models slightly over VRAM capacity load fully on GPU via CUDA Unified Memory. Finding: works in a narrow ~200-300MB sweet spot. Beyond that, PCIe page migration is slower than Ollama's native CPU split.

## Writing

No-fluff takes on cloud strategy, AI architecture, and the decisions that separate good systems from great ones.

→ [seanlobjoit.com](https://www.seanlobjoit.com) · [LinkedIn](https://linkedin.com/in/seanlobjoit)
