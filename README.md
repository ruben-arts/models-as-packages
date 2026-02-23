# Example repository for packaging models as conda packages

This repository is a proof of concept. With no intent to maintain it.

It contains a few recipes you can build to create conda packages for different whisper.cpp models in ggml format.

You can find the built packages in the `proto-model-forge` channel on prefix.dev, but you can also build and publish them yourself with the provided GitHub workflow and recipe.

Try out whisper.cpp in this project with:

```bash
pixi run tiny some-audio-file.mp3
```

Or build the model packages yourself locally with:

```bash
pixi run build
```
