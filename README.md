# Neopixel protocol decoder for Saleae Logic Analyzer

Decode the 800 kHz protocol used in Neopixel (WS2812) LEDs with a Saleae-brand logic analyzer.

Provides bytes above the bit data stream.

## Installation

1. Clone this repo `git clone git@github.com:mcauser/neopixel-saleae.git`
2. Install [Saleae Protocol Analyzer SDK](https://github.com/saleae/AnalyzerSDK) as a submodule `git submodule update --init`
3. Run `python build_analyzer.py`
4. The compiled libraries can be found in the newly created debug and release folders.

## Next steps

1. The signal doesn't properly reset after 50us (the last byte continues forever).
2. Provide test data for use in developing the protocol decoder as recommended in the Saleae documentation.
3. Group the bytes into 24-bit groups and show the actual LED color!
4. Provide releases pre-built for the major OSes.

## License

Copyright 2016 Julien Vanier. Released under the MIT license.
