# PicoAudio: Enabling Precise Timing and Frequency Controllability of Audio Events in Text-to-audio Generation
**Bullet contribution**:
* A data simulation pipeline tailored specifically for controllable audio generation frameworks;
* Propose a timing-controllable audio generation framework, enabling precise control over the timing and frequency of sound event;
* Achieve any precise control related to timing by integrating of large language models.


## Simulated Dataset
Simulated data can be downloaded from [GoogleDrive](https://drive.google.com/file/d/1oez7kzFFhqU9JZQhqJdDshXrRQczBmlp/view?usp=sharing) or [BaiduNetDisk](https://pan.baidu.com/s/1rGrcjtQCEYFpr3o6y9wI8Q?pwd=pico) with the extraction code "pico". 
The metadata is stored in *"data/meta_data/{}.json"*, one instance is as follows:
```python
{
  "filepath": "data/multi_event_test/syn_1.wav",
  "onoffCaption": "cat meowing at 0.5-2.0, 3.0-4.5 and whistling at 5.0-6.5 and explosion at 7.0-8.0, 8.5-9.5",
  "frequencyCaption": "cat meowing two times and whistling one times and explosion two times"
}
```
where:
* *"filepath"* indicates the path to the audio file.  
* *"frequencyCaption"* contains information about the occurrence frequency.
* *"onoffCaption"* contains on- & off-set information.
* For test file *"test-frequency-control_onoffFromGpt_{}.json"*, the *"onoffCaption"* is derived from *"frequencyCaption"* transformed by GPT-4, which is used for evaluation in the frequency control task.

<!--
### Hi there 👋
**PicoAudio/PicoAudio** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
