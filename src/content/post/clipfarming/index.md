---
title: "Creating an Automated Workflow for Clip Farming"
description: "Here is my journey of creating a clipfarm program."
publishDate: "April 6 2026"
tags: ["gemma", "whisper", "ollama"]
pinned: true
---

## Introduction

I always encountered Minecraft videos when scrolling through YouTube Shorts from content creators such as [DrDonut](https://www.youtube.com/DrDonutt), [JudeLow](https://www.youtube.com/@JudeLoSasso), and some clips from the UnstableSMP.

I always thought that this could be automated such as searching for clips and editing the videos. With the release of artificial intelligence and my time all freed up, I can finally put make this idea to use.

## Development

I wasn't sure on how to actually implement everything, so I separated the project into 3 different subprojects:
1. A process that watches YouTube streams (let's call this the "worker")
2. The backend that can start the processes mentioned above
3. The frontend to interact with the backend

### Building the Minimal Viable Product

Implementing the worker process was a little difficult since this was the only thing that was new to me at the time. I used [uv](https://github.com/astral-sh/uv) to manage the Python dependencies and used [OpenAI's Whisper](https://openai.com/index/whisper/) to transcribe the audio from an audio stream given from [Streamlink](https://github.com/streamlink/streamlink). However this was not enough to determine if a clip is high quality enough to be uploaded to a short-form content platform.
