# DeepSeek V4.1 Flash 1017 Obliterated

Shared in [0x0SojalSec's X post](https://x.com/0x0SojalSec/status/2123200083026202861): [OBLITERATUS/DeepSeek-V4.1-Flash-1017-obliterated](https://huggingface.co/OBLITERATUS/DeepSeek-V4.1-Flash-1017-obliterated).

The linked Hugging Face card describes this as a BF16, full-precision checkpoint of DeepSeek-V4.1-Flash-1017, produced with OBLITERATUS using the failspy method. It lists 755B parameters and an MIT license. The post itself notes that this full-precision version is for serious multi-GPU setups. This checkpoint is hosted on Hugging Face, not GitHub, so it has no GitHub fork.

## Related GitHub tool

The model card links the ablation toolkit used to produce it:

- Upstream: [elder-plinius/OBLITERATUS](https://github.com/elder-plinius/OBLITERATUS)
- Your individual fork: [benyamin-persia/OBLITERATUS](https://github.com/benyamin-persia/OBLITERATUS)
- Upstream license: AGPL-3.0.

The toolkit README describes itself as an alignment research tool for studying refusal behavior. It also says safety guardrails are removed from resulting models and the hosted Hugging Face Space has telemetry enabled by default. Review its current docs and settings before use.

## Evaluation and limitations

The X post repeats results also shown on the model card: full refusal fell from 81.62% to 4.30% on an 838-prompt evaluation. The card separately reports that 78.28% of the ablated model's responses were classified as harmful assistance, versus 10.38% for the base model. This is a major safety trade-off, not a measure of general usefulness.

The card reports MMLU accuracy of 87.96% for the base and 88.08% for the ablated model on 2,500 questions; its own paired-test result is not statistically significant (p=0.742829). These are the publisher's evaluations, not an independent replication, and they do not establish that all capabilities are “fully intact.”

The card also lists a related quantized GGUF repository: [HumanjavaEnterprises/DeepSeek-V4.1-Flash-1017-obliterated-upstream-GGUF](https://huggingface.co/HumanjavaEnterprises/DeepSeek-V4.1-Flash-1017-obliterated-upstream-GGUF). This remains a very large model; check the files and runtime requirements rather than assuming it will fit a typical single-GPU machine.

Do not use an ablated model to bypass safeguards in ways that could enable harm. Apply human review and suitable safeguards in any research or application setting, and comply with the model and toolkit licenses.
