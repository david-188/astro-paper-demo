---
author: Sat Naing
pubDatetime: 2022-09-25T15:20:35Z
title: The Implementation Path of Sora
featured: false
draft: false
tags:
  - sora
  - sora ai
  - text to video
description:
  sora is a large-scale model focused on video generation, enabling various forms of video editing through input text or images, including generation, connection, and extension, falling into the category of multimodal large-scale models. Such models extend and expand upon language models like GPT.
---

The significance of Sora lies in its redefining of the upper limit of AIGC in AI-driven content creation. Prior to this, text-based models like ChatGPT had already begun assisting content creation, including generating illustrations and images, and even producing short videos using virtual characters. Sora, on the other hand, is a large-scale model focused on video generation, enabling various forms of video editing through input text or images, including generation, connection, and extension, falling into the category of multimodal large-scale models. Such models extend and expand upon language models like GPT.

Sora operates on video "patches" in a similar way to how GPT-4 handles text tokens. Its key innovation lies in treating video frames as a sequence of patches, akin to word tokens in language models, enabling it to effectively manage various video information. By combining text-conditioned generation, Sora can generate contextually relevant and visually coherent videos based on text prompts.

In principle, Sora achieves video training through three main steps. Firstly, a video compression network is employed to reduce videos or images to a compact and efficient form. Secondly, spatio-temporal patch extraction breaks down visual information into smaller units, each containing spatial and temporal information of a part of the view, facilitating targeted processing in subsequent steps. Finally, video generation involves decoding and encoding based on input text or images, with the Transformer model (i.e., the ChatGPT-based transformer) determining how these units are transformed or combined to form complete video content.

Overall, the emergence of Sora will further drive the development of AI video generation and multimodal large-scale models, bringing new possibilities to the field of content creation.






