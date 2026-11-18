# Gaussian Splat Lite for Three.js

Collected from [HazratCrypto's X post](https://x.com/HazratCrypto/status/2122764712840507794), which describes rendering about three million 3D Gaussian splats in a browser, WebGPU with WebGL2 fallback, PLY/SPZ/SOG/RAD/LCC2 support, and streamed large scenes.

The post does not include a repository URL. I matched its feature details to [WilliamLiu-1997/Gaussian-Splat-Lite](https://github.com/WilliamLiu-1997/Gaussian-Splat-Lite): the project README lists the same rendering backends and formats, LCC2 streaming, a 3,000,000 splat budget example, and a Three.js `>=0.187.0` requirement. This is a feature-based identification, rather than a repository explicitly linked by the author.

- Upstream: [WilliamLiu-1997/Gaussian-Splat-Lite](https://github.com/WilliamLiu-1997/Gaussian-Splat-Lite)
- Your individual fork: [benyamin-persia/Gaussian-Splat-Lite](https://github.com/benyamin-persia/Gaussian-Splat-Lite)
- [Live demo](https://gaussian-splat-lite.vercel.app/)

The repository documents WebGPU and WebGL2 rendering, streamed LOD for RAD, SOG, and LCC2 scenes, support for PLY/SPZ/SOG/RAD inputs, and a `three` peer dependency of `>=0.187.0`. Its README states that Three.js `WebGPURenderer` falls back to WebGL2 when WebGPU is unavailable. See the upstream README and license for current details.
