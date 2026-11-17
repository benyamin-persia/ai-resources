# Fable 5.2: Creative-App Automation Playbook

Tutorial shared in [0xWast3's post](https://x.com/0xWast3/status/2122373100075450431), via the quoted [full X article](https://x.com/i/article/2120468399515992064).

This companion follows the article's progression: diagnose what the model may not know, supply the app-specific contract, generate scripts, and let the target application validate the result. The article covers 3ds Max, Unreal Engine, Blender, Illustrator, and Figma. Its model, API, pricing, and product-version details are claims from the article and may be time-sensitive; verify them against current official documentation.

## Tutorial flow

### 1. Separate missing knowledge from unreliable defaults

The article distinguishes post-training changes, which require supplying current release information, from older or ambiguous APIs where the model may choose a familiar but unsuitable pattern.

### 2. Make the app the grader

Treat generated code as a draft. Use the application, compiler, registration check, or other native validation result as the acceptance signal, then feed failures back into the next attempt.

### 3. Automate each creative app through its own scripting surface

- 3ds Max: convert reference drawings and measurements into structured inputs, then generate geometry with version-aware scripts.
- Unreal Engine: keep the experimental Python layer narrow and validate actions inside the editor.
- Blender: account for API changes and use the article's described generate-and-check loop.
- Illustrator: choose the supported scripting surface for the desired automation rather than assuming an unavailable API.
- Figma: provide current plugin typings and compile/check generated plugin code in stages.

### 4. Keep the handoff editable and repeatable

The playbook favors scripts and structured outputs that can be reopened and revised, with version-pinned context and automated checks instead of trusting a single generation.

## Source and fork status

The post and article do not link GitHub repositories, so there was nothing to fork. This page is a summary; follow the original article for its full examples, screenshots, and prompts.
