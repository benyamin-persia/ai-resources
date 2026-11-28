# OpenFill — Local Generative Fill for PhotoCraft and GIMP

Shared by [DEXTUNE's X post](https://x.com/dextune/status/2126277362153082934). The post links one GitHub repository: [beckettharriman/openfill](https://github.com/beckettharriman/openfill).

## Upstream and your individual fork

| Upstream | Your fork | Status |
|---|---|---|
| [beckettharriman/openfill](https://github.com/beckettharriman/openfill) | [benyamin-persia/openfill](https://github.com/benyamin-persia/openfill) | Newly forked individually; GitHub parent verified as `beckettharriman/openfill` |

The upstream reports an Apache-2.0 license. The fork was created separately from the `ai-resources` catalog repository; it is not just a link or copied entry.

## What it does

OpenFill is an image-editing plugin for PhotoCraft and GIMP 3 that uses a local [ComfyUI](https://github.com/comfyanonymous/ComfyUI) backend. Its documented operations include generative fill from a selected mask, object/background removal, canvas expansion, and text-to-image creation; results are placed on new layers so the original artwork remains editable. The current upstream README also lists upscaling and a Patchy companion integration.

The post says ComfyUI starts in the background, remains warm during editing, and closes with the editor. It describes local mode as requiring no account, telemetry, or bundled model. The upstream documentation confirms that models and ComfyUI may need to be downloaded separately; it also describes optional cloud-provider settings that send images to the selected service when enabled.

## Requirements and caveats

- The upstream marks the software beta. Its current README names PhotoCraft 0.12–0.23 and GIMP 3.2; compatibility and release status can change.
- For local generation, the upstream recommends a supported NVIDIA or AMD GPU with around 8 GB VRAM for its best models, with Apple Silicon support documented for PhotoCraft. Some operations/models may need less; check the current hardware guide before installing.
- Model files are not bundled. The project downloads or discovers models in ComfyUI folders, and each model has its own terms. The upstream specifically notes that some MAT, FLUX.1 Fill, and FLUX.2 Klein 9B choices are non-commercial.
- Its README reports local-only generation on `127.0.0.1` and no telemetry, but the optional cloud mode sends images to the provider selected by the user. Keep it off for local-only use and inspect the settings before processing private images.
- The upstream's install/provenance links mention ComfyUI, GIMP Stable Boy, comfyui-inpaint-nodes, krita-ai-diffusion, and Patchy. These are supporting projects referenced by OpenFill's own README, not additional repositories linked by DEXTUNE's post; this post's one linked project, OpenFill, is the one forked here.

## Links

- [Original post](https://x.com/dextune/status/2126277362153082934)
- [Upstream repository](https://github.com/beckettharriman/openfill)
- [Your fork](https://github.com/benyamin-persia/openfill)
- [Upstream releases](https://github.com/beckettharriman/openfill/releases)
- [Install and hardware documentation](https://github.com/beckettharriman/openfill/tree/main/docs)
- Supporting projects: [ComfyUI](https://github.com/comfyanonymous/ComfyUI), [GIMP Stable Boy](https://github.com/thndrbrrr/gimp-stable-boy), [ComfyUI Inpaint Nodes](https://github.com/Acly/comfyui-inpaint-nodes), [Krita AI Diffusion](https://github.com/Acly/krita-ai-diffusion), and [Patchy](https://github.com/SethRobinson/Patchy).
