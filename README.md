# Example repository for packaging models as conda packages

The Blog post related to this repository can be found here: https://prefix.dev/blog/packaging-ai-ml-models-as-conda-packages

This repository is a proof of concept. With no intent to maintain it.

It contains a few recipes you can build to create conda packages for different whisper.cpp models in ggml format.

You can find the built packages in the [`proto-model-forge`](https://prefix.dev/channels/proto-model-forge) channel on prefix.dev, but you can also build and publish them yourself with the provided GitHub workflow and recipe.

Try out whisper.cpp in this project with:

```bash
# This will run the small model and use your microphone as input
pixi run mic
# Or use the tiny model
pixi run mic tiny
# Or start the server
pixi run server
```

Or build the model packages yourself locally with:

```bash
pixi run build
```

And you can also publish them to your own channel on prefix.dev with:

```bash
pixi run publish
```

Shout out to the [whisper.cpp](https://github.com/ggml-org/whisper.cpp) for their amazing work on making whisper models available in a lightweight format that can run on edge devices.
