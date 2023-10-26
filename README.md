# NeoPixelBus_wrapper

**NeoPixelBus_wrapper**: A minimal wrapper to replace Adafruit_NeoPixel API to use Makuna's NeoPixelBus API.

(c) 2023, Ton Huisman for ESPEasy.

### How to use

- Add this library to your `lib` folder
- Add the [NeoPixelBus](https://github.com/Makuna/NeoPixelBus) library to your `lib` folder
- Replace the `#include <Adafruit_NeoPixel.h>` line by `#include <NeoPixelBus_wrapper.h>`
- Replace your type `Adafruit_NeoPixel` variable(s) by type `NeoPixelBus_wrapper` variable(s)
- When using runtime instantiation of the wrapper object, replace your `pixels = new Adafruit_NeoPixel(...)` call by `pixels = new NeoPixelBus_wrapper(...)`
- Compile, and presto!

### Limitations

- Currently only supports the most commonly used NeoPixel stripes `NEO_GRB` and `NEO_GRBW`, and the default `NEO_KHZ800` method. (That's all what is used in ESPEasy...)

### Support

For questions and improvement requests, please use the Github Issues system.

### Reference

- [NeoPixelBus](https://github.com/Makuna/NeoPixelBus)
- [Adafruit_NeoPixel](https://github.com/adafruit/Adafruit_NeoPixel)