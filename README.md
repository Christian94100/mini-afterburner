# 🚀 Mini Afterburner

A retro-style shoot'em up inspired by SEGA's After Burner, implemented in C using SDL2.

 http://www.hardcoregaming101.net/after-burner-iii/ (https://www.gamesdatabase.org/game/arcade/after-burner/screenshot1.jpg) ](https://www.mobygames.com/game/22833/after-burner-iii/screenshots/sega-cd/169744/) 

## ✨ Features

- Fast-paced arcade shooting action
- Smooth sprite animations
- Particle effects system
- Dynamic background scrolling
- Persistent high scores
- Configurable audio settings
- Neo Geo style graphics

## 🎮 Controls

- **Arrow Keys**: Move your aircraft
- **Space**: Fire weapons
- **Enter**: Start game
- **O**: Options menu
- **Esc**: Return/Quit

## 🛠️ Building from Source

### Prerequisites

```bash
# Install required development libraries
sudo apt-get update
sudo apt-get install -y gcc make libsdl2-dev libsdl2-ttf-dev libsdl2-mixer-dev
```

### Compilation

```bash
make
```

Or manually:

```bash
gcc -o afterburner main.c game.c -lSDL2 -lSDL2_ttf -lSDL2_mixer -lm
```

## 📁 Project Structure

```
.
├── src/
│   ├── game.h        # Game declarations
│   ├── game.c        # Game implementation
│   └── main.c        # Entry point
├── assets/
│   ├── player.bmp    # Player sprite sheet
│   ├── enemy.bmp     # Enemy sprite sheet
│   ├── arial.ttf     # Font file
│   ├── synthwave.ogg # Background music
│   ├── laser.wav     # Shot sound effect
│   └── explode.wav   # Explosion sound
└── Makefile          # Build configuration
```

## 🎯 Design Patterns

- **State Pattern**: Game state management (Menu, Playing, Options)
- **Game Loop Pattern**: Fixed time step update/render cycle
- **Component Pattern**: Entity management (player, enemies, particles)
- **Resource Manager**: Asset loading and cleanup
- **Observer Pattern**: Collision and event handling

## 🌐 WebAssembly Port

The game can be compiled to WebAssembly using Emscripten:

```bash
emcc -o web/game.js src/*.c -s USE_SDL=2 -s USE_SDL_TTF=2 -s USE_SDL_MIXER=2
```

See [WebAssembly Guide](docs/wasm.md) for details.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
