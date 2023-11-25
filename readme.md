## Description
Mycroft wake word plugin for [Nyumaya](https://github.com/nyumaya) version 3.1.0

### Performance
- Pi Zero: CPU 52%
- Pi 3: CPU one core: 12%
- Pi 4: CPU one core: 4%
- i.MX8 CPU one core: 4%
- i.MX6 CPU one core: 11.9% (CortexA9)

## Install

`pip install ovos-ww-plugin-nyumaya`

## Configuration

The default free wake words are included with this plugin

Add the following to your hotwords section in mycroft.conf 

```json
  "hotwords": {
    "alexa": {
        "module": "ovos-ww-plugin-nyumaya",
        "model": "alexa",
        "sensitivity": 0.5,
        "extractor_gain": 1.0
    },
    "marvin": {
        "module": "ovos-ww-plugin-nyumaya",
        "model": "marvin",
        "sensitivity": 0.5,
        "extractor_gain": 1.0
    },
    "sheila": {
        "module": "ovos-ww-plugin-nyumaya",
        "model": "sheila",
        "sensitivity": 0.5,
        "extractor_gain": 1.0
    },
     "firefox": {
        "module": "ovos-ww-plugin-nyumaya",
        "model": "firefox",
        "sensitivity": 0.5,
        "extractor_gain": 1.0
    }
  }
```

Then select what wakeword to use

```json
 "listener": {
      "wake_word": "alexa"
 }
 
```


# Training your own wake word

You can request new wake words [here](https://nyumaya.com/requesting-custom-keywords/)
