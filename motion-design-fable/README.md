# Motion Design with Fable 5.2: from zero to your first video in 10 minutes

**Original tutorial:** [Read the complete article on X](https://x.com/i/article/2121728254080143360) · [Post shared by anstap](https://x.com/anstapnever/status/2121750611691712817)

This page follows the original tutorial's section order and hands-on flow. The source article is the canonical version for its full prompts, examples, media, and wording; the notes below are a companion outline, not a verbatim copy.

## How it works, in one minute

Ask Claude to write an animated HTML page, preview it in Chrome, then export the animation as an MP4. For smoother output, render the page frame by frame instead of recording the screen.

## What you need and what it costs

- A Claude plan with access to the model specified by the article.
- A computer with Google Chrome.
- For the command-line route: Claude Code, Python, Playwright, and FFmpeg.

The article discusses model/API costs and subscription limits. Check the original and current provider pricing before relying on its estimates; they are not independently verified here.

## Path 1: no install, in the Claude app

1. Open Claude in the app or browser and select the model described by the tutorial.
2. Ask for a short animation as a single HTML file that can be opened in Chrome.
3. Preview it, request adjustments in plain language, then download the HTML.
4. Open the file in Chrome and record the animation for a quick first result.

The article notes that screen recording is convenient, while frame-by-frame rendering is better when consistent frame rate matters.

## Path 2: Claude Code, on Windows or Mac

Install Claude Code and FFmpeg using the platform-specific setup instructions in the [original tutorial](https://x.com/i/article/2121728254080143360). Start Claude Code in a new project folder, have it create the animation, and ask it to render and check the result. The article also provides a Python/Playwright renderer for exporting frames deterministically.

## Your first video: one line, and what it gives you

Start with one concise request: specify the subject, approximate duration, and that the result should be one HTML file previewable in Chrome. Review the first draft, then refine one or two concrete things at a time.

## The director's template: the 6 lines that make it yours

The tutorial's prompt template turns a broad idea into production direction. Fill in the subject/audience, dimensions and playback behavior, visual style and colors, timed sequence of events, motion behavior, and sound. See the source for its complete copyable template.

## How to ask for changes: 12 phrases that work

Give specific edits with a location or timestamp and a measurable change. For example, ask to slow a named interval, enlarge a title by a percentage, or move an element by a number of pixels. The source article includes the full set of example requests.

## Vertical video for Reels, TikTok and Shorts

Choose a portrait canvas before generating the animation. The tutorial demonstrates a 9:16 layout and recommends keeping text legible on a phone, planning the loop, and staging motion for the taller frame. Consult the article's size table for its platform-specific dimensions.

## Turn it into an MP4

For a quick draft, record the browser preview. For a clean export, use the source's frame-by-frame Python/Playwright workflow and encode the captured frames with FFmpeg. Your existing fork: [benyamin-persia/FFmpeg](https://github.com/benyamin-persia/FFmpeg). The original article contains the full renderer and commands.

## Add music

Place the music track under the rendered video, combine the audio and video, and fade the ending if needed. Use the commands in the source article and make sure you have permission to use the audio.

## 4 more prompts you can copy

The article includes four additional starter prompts. They cover alternate animation concepts and formats; use the source article for the exact prompts and example outputs.

## 10 beginner mistakes and their fixes

The tutorial's troubleshooting section pairs common issues—unclear direction, crowded timing, readability, pacing, and export problems—with concrete corrections. Its full fix table is in the original article.

## The short version

Prompt an animation as HTML → preview and revise it in Chrome → export to MP4, using FFmpeg and frame-by-frame rendering when output smoothness matters.

### Forks

The post links to the tutorial, not to GitHub repositories. No new fork was needed; FFmpeg was already forked in your account. The article mentions Claude Code, Chrome, Python, Playwright, and FFmpeg as workflow tools.
