# Freecube Engine - Specs / Especificaciones

## 🎧 Technical Specifications / Especificaciones Técnicas

| Category / Categoría | Detail / Detalle |
|----------------------|-----------------|
| **Type / Tipo** | Audio Engine / Motor de audio |
| **Language / Lenguaje** | C++17 |
| **Dependencies / Dependencias** | PortAudio (for audio output) / PortAudio (para salida de audio) |
| **Output Channels / Canales de salida** | Stereo 2.0 (interleaved) / Estéreo 2.0 (intercalado) |
| **Sample Rate / Frecuencia de muestreo** | 48 kHz (upgradeable to Hi-Res internally) / 48 kHz (ampliable a Hi-Res internamente) |
| **Bit Depth / Bits** | 32-bit float internally / 32-bit flotante internamente |
| **Basic DSP / DSP básico** | Test tone generator (sine wave) / Generador de tono de prueba (senoide) |
| **License / Licencia** | MIT |
| **Supported Platforms / Plataformas soportadas** | macOS, Linux, Windows (CMake) |
| **Future Integration / Integración futura** | - Binaural processing (HRTF) / Procesamiento binaural (HRTF)<br>- 5.1 / Surround upmix / Upmix 5.1 / Surround<br>- EQ / Reverb / Convolution filters / Filtros EQ / Reverb / Convolución<br>- Hi-Res support (24-bit / 96 kHz) / Soporte Hi-Res (24-bit / 96 kHz)<br>- Audio capture from Dolphin via virtual device / Captura de audio de Dolphin vía dispositivo virtual |
| **Project Structure / Estructura del proyecto** | `src/` with `main.cpp`, `audio_engine.cpp` and `audio_engine.h`, `CMakeLists.txt`, `README.md`, `LICENSE` / `src/` con `main.cpp`, `audio_engine.cpp` y `audio_engine.h`, `CMakeLists.txt`, `README.md`, `LICENSE` |
| **Current Status / Estado actual** | Minimal functional engine (test tone) ready to expand / Motor mínimo funcional (tono de prueba) listo para expandir |

## 💡 Notes / Notas importantes
- Freecube Engine is **not an OS or emulator**, only an **audio engine**. / Freecube Engine **no es un sistema operativo ni emulador**, solo un **motor de audio**.
- Can process **real-time audio** from any source redirected to PortAudio. / Puede procesar **audio en tiempo real** desde cualquier fuente redirigida a PortAudio.
- Quality depends on the original source (e.g., GameCube audio is 16-bit / 48 kHz). / La calidad depende de la fuente original (por ejemplo, el audio de GameCube es 16-bit / 48 kHz).