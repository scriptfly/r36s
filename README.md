# r36s – Crackling Sound Fix on dArkOSRE

## This README describes how to fix the crackling sound problem on the r36s and compatible clones.

The fix was developed for my G80CA-MB V1.3-20251212 clone, which has a low-quality speaker that cannot reproduce lower frequencies correctly. As a result, low-frequency sounds produce an annoying crackling noise instead of clean audio.

Fortunately, RetroArch provides a dedicated option for configuring DSP effects. This can be used to filter out low frequencies from the audio output and eliminate the crackling noise.

### Instalation

1. Download the HighPassFilter.dsp file - [link](https://github.com/scriptfly/r36s/blob/main/HighPassFilter.dsp).
2. Put downloaded .dsp file into **/home/ark/.config/retroarch/filters/audio/** and **/home/ark/.config/retroarch32/filters/audio/** folders on your dArkOSRE SD card.
3. Boot the system
4. Launch a game, open the RetroArch Quick Menu (typically via Select + X or Fn + X), press B (back) and navigate to Settings > Audio > DSP Plugins.
5. Select **HighPassFilter.dsp**.
6. Go back and save the configuration (Configuration File > Save Current Configuration).

The equalizer profile is now active and filters out low frequencies from the audio output. You should no longer hear most of the crackling.

> Note: This configuration applies only to the specific RetroArch instance where it was created. Repeat the steps above for both RetroArch and RetroArch32.
