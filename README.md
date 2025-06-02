# <img src="https://raw.githubusercontent.com/idiap/coqui-ai-TTS/main/images/coqui-log-green-TTS.png" height="56"/>


**🐸 Coqui TTS is a library for advanced Text-to-Speech generation.**

🚀 Pretrained models in +1100 languages.

🛠️ Tools for training new models and fine-tuning existing models in any language.

📚 Utilities for dataset analysis and curation.

[![Discord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coqui-tts)](https://pypi.org/project/coqui-tts/)
[![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
[![PyPI version](https://badge.fury.io/py/coqui-tts.svg)](https://pypi.org/project/coqui-tts/)
[![Downloads](https://pepy.tech/badge/coqui-tts)](https://pepy.tech/project/coqui-tts)
[![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
[![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/tests.yml/badge.svg)](https://github.com/idiap/coqui-ai-TTS/actions/workflows/tests.yml)
[![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/docker.yaml/badge.svg)](https://github.com/idiap/coqui-ai-TTS/actions/workflows/docker.yaml)
[![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/style_check.yml/badge.svg)](https://github.com/idiap/coqui-ai-TTS/actions/workflows/style_check.yml)
[![Docs](<https://readthedocs.org/projects/coqui-tts/badge/?version=latest&style=plastic>)](https://coqui-tts.readthedocs.io/en/latest/)

</div>

## 📣 News
- **Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)**
- 0.25.0: [OpenVoice](https://github.com/myshell-ai/OpenVoice) models now available for voice conversion.
- 0.24.2: Prebuilt wheels are now also published for Mac and Windows (in addition to Linux as before) for easier installation across platforms.
- 0.20.0: XTTSv2 is here with 17 languages and better performance across the board. XTTS can stream with <200ms latency.
- 0.19.0: XTTS fine-tuning code is out. Check the [example recipes](https://github.com/idiap/coqui-ai-TTS/tree/dev/recipes/ljspeech).
- 0.14.1: You can use [Fairseq models in ~1100 languages](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) with 🐸TTS.

## 💬 Where to ask questions
Please use our dedicated channels for questions and discussion. Help is much more valuable if it's shared publicly so that more people can benefit from it.

| Type                                         | Platforms                           |
| -------------------------------------------- | ----------------------------------- |
| 🚨 **Bug Reports, Feature Requests & Ideas** | [GitHub Issue Tracker]              |
| 👩‍💻 **Usage Questions**                       | [GitHub Discussions]                |
| 🗯 **General Discussion**                    | [GitHub Discussions] or [Discord]   |

[github issue tracker]: https://github.com/idiap/coqui-ai-TTS/issues
[github discussions]: https://github.com/idiap/coqui-ai-TTS/discussions
[discord]: https://discord.gg/5eXr5seRrv
[Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials

The [issues](https://github.com/coqui-ai/TTS/issues) and
[discussions](https://github.com/coqui-ai/TTS/discussions) in the original
repository are also still a useful source of information.


## 🔗 Links and Resources
| Type                            | Links                               |
| ------------------------------- | --------------------------------------- |
| 💼 **Documentation**              | [ReadTheDocs](https://coqui-tts.readthedocs.io/en/latest/)
| 💾 **Installation**               | [TTS/README.md](https://github.com/idiap/coqui-ai-TTS/tree/dev#installation)|
| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/idiap/coqui-ai-TTS/blob/main/CONTRIBUTING.md)|
| 🚀 **Released Models**            | [Standard models](https://github.com/idiap/coqui-ai-TTS/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/idiap/coqui-ai-TTS#example-text-to-speech-using-fairseq-models-in-1100-languages-)|

## Features
- High-performance text-to-speech and voice conversion models, see list below.
- Fast and efficient model training with detailed training logs on the terminal and Tensorboard.
- Support for multi-speaker and multilingual TTS.
- Released and ready-to-use models.
- Tools to curate TTS datasets under ```dataset_analysis/```.
- Command line and Python APIs to use and test your models.
- Modular (but not too much) code base enabling easy implementation of new ideas.

## Model Implementations
### Spectrogram models
- [Tacotron](https://arxiv.org/abs/1703.10135), [Tacotron2](https://arxiv.org/abs/1712.05884)
- [Glow-TTS](https://arxiv.org/abs/2005.11129), [SC-GlowTTS](https://arxiv.org/abs/2104.05557)
- [Speedy-Speech](https://arxiv.org/abs/2008.03802)
- [Align-TTS](https://arxiv.org/abs/2003.01950)
- [FastPitch](https://arxiv.org/pdf/2006.06873.pdf)
- [FastSpeech](https://arxiv.org/abs/1905.09263), [FastSpeech2](https://arxiv.org/abs/2006.04558)
- [Capacitron](https://arxiv.org/abs/1906.03402)
- [OverFlow](https://arxiv.org/abs/2211.06892)
- [Neural HMM TTS](https://arxiv.org/abs/2108.13320)
- [Delightful TTS](https://arxiv.org/abs/2110.12612)

### End-to-End Models
- [XTTS](https://arxiv.org/abs/2406.04904)
- [VITS](https://arxiv.org/pdf/2106.06103)
- 🐸[YourTTS](https://arxiv.org/abs/2112.02418)
- 🐢[Tortoise](https://github.com/neonbjb/tortoise-tts)
- 🐶[Bark](https://github.com/suno-ai/bark)

### Vocoders
- [MelGAN](https://arxiv.org/abs/1910.06711)
- [MultiBandMelGAN](https://arxiv.org/abs/2005.05106)
- [ParallelWaveGAN](https://arxiv.org/abs/1910.11480)
- [GAN-TTS discriminators](https://arxiv.org/abs/1909.11646)
- [WaveRNN](https://github.com/fatchord/WaveRNN/)
- [WaveGrad](https://arxiv.org/abs/2009.00713)
- [HiFiGAN](https://arxiv.org/abs/2010.05646)
- [UnivNet](https://arxiv.org/abs/2106.07889)

### Voice Conversion
- [FreeVC](https://arxiv.org/abs/2210.15418)
- [kNN-VC](https://doi.org/10.21437/Interspeech.2023-419)
- [OpenVoice](https://arxiv.org/abs/2312.01479)

### Others
- Attention methods: [Guided Attention](https://arxiv.org/abs/1710.08969),
  [Forward Backward Decoding](https://arxiv.org/abs/1907.09006),
  [Graves Attention](https://arxiv.org/abs/1910.10288),
  [Double Decoder Consistency](https://erogol.com/solving-attention-problems-of-tts-models-with-double-decoder-consistency/),
  [Dynamic Convolutional Attention](https://arxiv.org/pdf/1910.10288.pdf),
  [Alignment Network](https://arxiv.org/abs/2108.10447)
- Speaker encoders: [GE2E](https://arxiv.org/abs/1710.10467),
  [Angular Loss](https://arxiv.org/pdf/2003.11982.pdf)

You can also help us implement more models.

<!-- start installation -->
## Installation

🐸TTS is tested on Ubuntu 24.04 with **python >= 3.10, < 3.13**, but should also
work on Mac and Windows.

If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the pretrained 🐸TTS models, installing from PyPI is the easiest option.

```bash
pip install coqui-tts
```

If you plan to code or train models, clone 🐸TTS and install it locally.

```bash
git clone https://github.com/idiap/coqui-ai-TTS
cd coqui-ai-TTS
pip install -e .
```

### Optional dependencies

The following extras allow the installation of optional dependencies:

| Name | Description |
|------|-------------|
| `all` | All optional dependencies |
| `notebooks` | Dependencies only used in notebooks |
| `server` | Dependencies to run the TTS server |
| `bn` | Bangla G2P |
| `ja` | Japanese G2P |
| `ko` | Korean G2P |
| `zh` | Chinese G2P |
| `languages` | All language-specific dependencies |

You can install extras with one of the following commands:

```bash
pip install coqui-tts[server,ja]
pip install -e .[server,ja]
```

### Platforms

If you are on Ubuntu (Debian), you can also run the following commands for installation.

```bash
make system-deps
make install
```

<!-- end installation -->

### 🚀 Docker Image

You can easily run the XTTS server using Docker without manually downloading the model. The container will automatically download the model on first startup.

🐳 Running the Container
>docker-compose.yml

```yml
services:
  xtts:
    image: ghcr.io/idiap/coqui-tts-cpu
    container_name: xtts-server
    ports:
      - "5002:5002"
    entrypoint: /bin/bash
    command: -c "python3 TTS/server/server.py --model_name tts_models/multilingual/multi-dataset/xtts_v2"
```
> [!Note]
📥 Model Download Inside Container
When you start the service for the first time, Docker will automatically download the model to:

> /root/.local/share/tts.

No manual downloading or setup is needed.

> [!Important]
>🔁 Changing the Model
You can switch to a different Coqui TTS model by modifying this line:

```bash
command: -c "python3 TTS/server/server.py --model_name <model_name>"
```
Example:
```bash
command: -c "python3 TTS/server/server.py --model_name tts_models/ar/css10/vits"
```
### Installation
```python
docker-compose up --build
```
### 📦 Supported Models
<details close>
<summary><h4>⬅️ Text-to-Speech Models</h4></summary>
  
```bash
  1: tts_models/multilingual/multi-dataset/xtts_v2
  2: tts_models/multilingual/multi-dataset/xtts_v1.1
  3: tts_models/multilingual/multi-dataset/your_tts
  4: tts_models/multilingual/multi-dataset/bark
  5: tts_models/bg/cv/vits
  6: tts_models/cs/cv/vits
  7: tts_models/da/cv/vits
  8: tts_models/et/cv/vits
  9: tts_models/ga/cv/vits
 10: tts_models/en/ek1/tacotron2
 11: tts_models/en/ljspeech/tacotron2-DDC
 12: tts_models/en/ljspeech/tacotron2-DDC_ph
 13: tts_models/en/ljspeech/glow-tts
 14: tts_models/en/ljspeech/speedy-speech
 15: tts_models/en/ljspeech/tacotron2-DCA
 16: tts_models/en/ljspeech/vits
 17: tts_models/en/ljspeech/vits--neon
 18: tts_models/en/ljspeech/fast_pitch
 19: tts_models/en/ljspeech/overflow
 20: tts_models/en/ljspeech/neural_hmm
 21: tts_models/en/vctk/vits
 22: tts_models/en/vctk/fast_pitch
 23: tts_models/en/sam/tacotron-DDC
 24: tts_models/en/blizzard2013/capacitron-t2-c50
 25: tts_models/en/blizzard2013/capacitron-t2-c150_v2
 26: tts_models/en/multi-dataset/tortoise-v2
 27: tts_models/en/jenny/jenny
 28: tts_models/es/mai/tacotron2-DDC
 29: tts_models/es/css10/vits
 30: tts_models/fr/mai/tacotron2-DDC
 31: tts_models/fr/css10/vits
 32: tts_models/uk/mai/glow-tts
 33: tts_models/uk/mai/vits
 34: tts_models/zh-CN/baker/tacotron2-DDC-GST
 35: tts_models/nl/mai/tacotron2-DDC
 36: tts_models/nl/css10/vits
 37: tts_models/de/thorsten/tacotron2-DCA
 38: tts_models/de/thorsten/vits
 39: tts_models/de/thorsten/tacotron2-DDC
 40: tts_models/de/css10/vits-neon
 41: tts_models/ja/kokoro/tacotron2-DDC
 42: tts_models/tr/common-voice/glow-tts
 43: tts_models/it/mai_female/glow-tts
 44: tts_models/it/mai_female/vits
 45: tts_models/it/mai_male/glow-tts
 46: tts_models/it/mai_male/vits
 47: tts_models/ewe/openbible/vits
 48: tts_models/hau/openbible/vits
 49: tts_models/lin/openbible/vits
 50: tts_models/tw_akuapem/openbible/vits
 51: tts_models/tw_asante/openbible/vits
 52: tts_models/yor/openbible/vits
 53: tts_models/hu/css10/vits
 54: tts_models/el/cv/vits
 55: tts_models/fi/css10/vits
 56: tts_models/hr/cv/vits
 57: tts_models/lt/cv/vits
 58: tts_models/lv/cv/vits
 59: tts_models/mt/cv/vits
 60: tts_models/pl/mai_female/vits
 61: tts_models/pt/cv/vits
 62: tts_models/ro/cv/vits
 63: tts_models/sk/cv/vits
 64: tts_models/sl/cv/vits
 65: tts_models/sv/cv/vits
 66: tts_models/ca/custom/vits
 67: tts_models/fa/custom/glow-tts
 68: tts_models/fa/custom/vits-female
 69: tts_models/bn/custom/vits-male
 70: tts_models/bn/custom/vits-female
 71: tts_models/be/common-voice/glow-tts
```

</details>
<details close>
<summary><h4>⬅️ Vocoder Models</h4></summary>

  ```bash
  1: vocoder_models/universal/libri-tts/wavegrad
  2: vocoder_models/universal/libri-tts/fullband-melgan
  3: vocoder_models/en/ek1/wavegrad
  4: vocoder_models/en/librispeech100/wavlm-hifigan
  5: vocoder_models/en/librispeech100/wavlm-hifigan_prematched
  6: vocoder_models/en/ljspeech/multiband-melgan
  7: vocoder_models/en/ljspeech/hifigan_v2
  8: vocoder_models/en/ljspeech/univnet
  9: vocoder_models/en/blizzard2013/hifigan_v2
 10: vocoder_models/en/vctk/hifigan_v2
 11: vocoder_models/en/sam/hifigan_v2
 12: vocoder_models/nl/mai/parallel-wavegan
 13: vocoder_models/de/thorsten/wavegrad
 14: vocoder_models/de/thorsten/fullband-melgan
 15: vocoder_models/de/thorsten/hifigan_v1
 16: vocoder_models/ja/kokoro/hifigan_v1
 17: vocoder_models/uk/mai/multiband-melgan
 18: vocoder_models/tr/common-voice/hifigan
 19: vocoder_models/be/common-voice/hifigan
```
</details>
<details close>
<summary><h4>⬅️ Voice Conversion Models</h4></summary>

  ```bash
  1: voice_conversion_models/multilingual/vctk/freevc24
  2: voice_conversion_models/multilingual/multi-dataset/knnvc
  3: voice_conversion_models/multilingual/multi-dataset/openvoice_v1
  4: voice_conversion_models/multilingual/multi-dataset/openvoice_v2
```
</details>
You can also try out Coqui TTS without installation with the docker image.
Simply run the following command and you will be able to run TTS:


```bash
docker run --rm -it -p 5002:5002 --entrypoint /bin/bash ghcr.io/idiap/coqui-tts-cpu
python3 TTS/server/server.py --list_models #To get the list of available models
python3 TTS/server/server.py --model_name tts_models/en/vctk/vits # To start a server
```

You can then enjoy the TTS server [here](http://[::1]:5002/)
More details about the docker images (like GPU support) can be found
[here](https://coqui-tts.readthedocs.io/en/latest/docker_images.html)


## Synthesizing speech by 🐸TTS
<!-- start inference -->
### 🐍 Python API

#### Multi-speaker and multi-lingual model

```python
import torch
from TTS.api import TTS

# Get device
device = "cuda" if torch.cuda.is_available() else "cpu"

# List available 🐸TTS models
print(TTS().list_models())

# Initialize TTS
tts = TTS("tts_models/multilingual/multi-dataset/xtts_v2").to(device)

# List speakers
print(tts.speakers)

# Run TTS
# ❗ XTTS supports both, but many models allow only one of the `speaker` and
# `speaker_wav` arguments

# TTS with list of amplitude values as output, clone the voice from `speaker_wav`
wav = tts.tts(
  text="Hello world!",
  speaker_wav="my/cloning/audio.wav",
  language="en"
)

# TTS to a file, use a preset speaker
tts.tts_to_file(
  text="Hello world!",
  speaker="Craig Gutsy",
  language="en",
  file_path="output.wav"
)
```

#### Single speaker model

```python
# Initialize TTS with the target model name
tts = TTS("tts_models/de/thorsten/tacotron2-DDC").to(device)

# Run TTS
tts.tts_to_file(text="Ich bin eine Testnachricht.", file_path=OUTPUT_PATH)
```

#### Voice conversion (VC)

Converting the voice in `source_wav` to the voice of `target_wav`:

```python
tts = TTS("voice_conversion_models/multilingual/vctk/freevc24").to("cuda")
tts.voice_conversion_to_file(
  source_wav="my/source.wav",
  target_wav="my/target.wav",
  file_path="output.wav"
)
```

Other available voice conversion models:
- `voice_conversion_models/multilingual/multi-dataset/knnvc`
- `voice_conversion_models/multilingual/multi-dataset/openvoice_v1`
- `voice_conversion_models/multilingual/multi-dataset/openvoice_v2`

For more details, see the
[documentation](https://coqui-tts.readthedocs.io/en/latest/vc.html).

#### Voice cloning by combining single speaker TTS model with the default VC model

This way, you can clone voices by using any model in 🐸TTS. The FreeVC model is
used for voice conversion after synthesizing speech.

```python

tts = TTS("tts_models/de/thorsten/tacotron2-DDC")
tts.tts_with_vc_to_file(
    "Wie sage ich auf Italienisch, dass ich dich liebe?",
    speaker_wav="target/speaker.wav",
    file_path="output.wav"
)
```

#### TTS using Fairseq models in ~1100 languages 🤯
For Fairseq models, use the following name format: `tts_models/<lang-iso_code>/fairseq/vits`.
You can find the language ISO codes [here](https://dl.fbaipublicfiles.com/mms/tts/all-tts-languages.html)
and learn about the Fairseq models [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms).

```python
# TTS with fairseq models
api = TTS("tts_models/deu/fairseq/vits")
api.tts_to_file(
    "Wie sage ich auf Italienisch, dass ich dich liebe?",
    file_path="output.wav"
)
```

### Command-line interface `tts`

<!-- begin-tts-readme -->

Synthesize speech on the command line.

You can either use your trained model or choose a model from the provided list.

- List provided models:

  ```sh
  tts --list_models
  ```

- Get model information. Use the names obtained from `--list_models`.
  ```sh
  tts --model_info_by_name "<model_type>/<language>/<dataset>/<model_name>"
  ```
  For example:
  ```sh
  tts --model_info_by_name tts_models/tr/common-voice/glow-tts
  tts --model_info_by_name vocoder_models/en/ljspeech/hifigan_v2
  ```

#### Single speaker models

- Run TTS with the default model (`tts_models/en/ljspeech/tacotron2-DDC`):

  ```sh
  tts --text "Text for TTS" --out_path output/path/speech.wav
  ```

- Run TTS and pipe out the generated TTS wav file data:

  ```sh
  tts --text "Text for TTS" --pipe_out --out_path output/path/speech.wav | aplay
  ```

- Run a TTS model with its default vocoder model:

  ```sh
  tts --text "Text for TTS" \
      --model_name "<model_type>/<language>/<dataset>/<model_name>" \
      --out_path output/path/speech.wav
  ```

  For example:

  ```sh
  tts --text "Text for TTS" \
      --model_name "tts_models/en/ljspeech/glow-tts" \
      --out_path output/path/speech.wav
  ```

- Run with specific TTS and vocoder models from the list. Note that not every vocoder is compatible with every TTS model.

  ```sh
  tts --text "Text for TTS" \
      --model_name "<model_type>/<language>/<dataset>/<model_name>" \
      --vocoder_name "<model_type>/<language>/<dataset>/<model_name>" \
      --out_path output/path/speech.wav
  ```

  For example:

  ```sh
  tts --text "Text for TTS" \
      --model_name "tts_models/en/ljspeech/glow-tts" \
      --vocoder_name "vocoder_models/en/ljspeech/univnet" \
      --out_path output/path/speech.wav
  ```

- Run your own TTS model (using Griffin-Lim Vocoder):

  ```sh
  tts --text "Text for TTS" \
      --model_path path/to/model.pth \
      --config_path path/to/config.json \
      --out_path output/path/speech.wav
  ```

- Run your own TTS and Vocoder models:

  ```sh
  tts --text "Text for TTS" \
      --model_path path/to/model.pth \
      --config_path path/to/config.json \
      --out_path output/path/speech.wav \
      --vocoder_path path/to/vocoder.pth \
      --vocoder_config_path path/to/vocoder_config.json
  ```

#### Multi-speaker models

- List the available speakers and choose a `<speaker_id>` among them:

  ```sh
  tts --model_name "<language>/<dataset>/<model_name>"  --list_speaker_idxs
  ```

- Run the multi-speaker TTS model with the target speaker ID:

  ```sh
  tts --text "Text for TTS." --out_path output/path/speech.wav \
      --model_name "<language>/<dataset>/<model_name>"  --speaker_idx <speaker_id>
  ```

- Run your own multi-speaker TTS model:

  ```sh
  tts --text "Text for TTS" --out_path output/path/speech.wav \
      --model_path path/to/model.pth --config_path path/to/config.json \
      --speakers_file_path path/to/speaker.json --speaker_idx <speaker_id>
  ```

#### Voice conversion models

```sh
tts --out_path output/path/speech.wav --model_name "<language>/<dataset>/<model_name>" \
    --source_wav <path/to/speaker/wav> --target_wav <path/to/reference/wav>
```

<!-- end-tts-readme -->
