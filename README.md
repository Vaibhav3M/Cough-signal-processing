<p align="center">
  <img width="250" src="./Images/WAVE.png">
</p>
<h2 align="center">Cough Signal Processing ( csp ) </h2>



<p align="center">A micro framework for cough singal processing </p>
<p align="center"> Contribute and Support </p>


[![GitHub license](https://img.shields.io/badge/License-Creative%20Commons%20Attribution%204.0%20International-blue)](https://github.com/coughresearch/Cough-signal-processing/blob/master/LICENSE)
[![GitHub commit](https://img.shields.io/github/last-commit/coughresearch/Cough-signal-processing)](https://github.com/coughresearch/Cough-signal-processing/commits/master)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

### Features

- Spectrogram features extraction
- Contiguous features
- Cough event detection
- Experiments on noise removal, Silence in cough sounds
- Applying different types of filters
- Audio augmentation techniques


### Quick Start

```python
from csp import SpectrogramFeatures

# path of the cough audio
sp   = SpectrogramFeatures('cough_sound_9412.m4a')
data = sp.spectrogram_data()

```

#### output

<img width="350" src="./Images/spectrogram_one.png">


### Audio augmentation techniques
#### Speed tuning

```python
from csp import AudioAugmentation

# Audio_augmentation speed tuning
Audio_aug = AudioAugmentation.speed_tuning(data['signal'])

```

#### output

<img width="350" src="./Images/spectrogram_two.png">


#### Time shifting
```python

# Audio augmentation time shifting
aug = AudioAugmentation.time_shifting(data['signal'])

```

#### output

<img width="350" src="./Images/spectrogram_three.png">


#### Feature extraction { @thileepanp }
<p align="center">
  <img width=850" src="./Images/Audio Feature Classification.PNG">
</p>
