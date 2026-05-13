  # Source Engine Configurator

  <img src="source-configurator.png" alt="Source Engine Configurator icon" width="128">

  Source Engine Configurator is a PowerPC Mac utility for creating native PowerPC builds of select Source Engine games from your own
  legally purchased game files.

  It bundles a PowerPC-compatible Source Engine runtime with supported Source game installs, producing standalone `.app` bundles
  that can run on PowerPC Macs without virtualization or emulation.

  This project is currently an early alpha. Expect bugs, crashes, rendering issues, performance problems, missing effects, audio
  glitches, and game-specific compatibility issues.

  ## Requirements

  - PowerPC G4 or G5 Mac
  - 1.2 GHz or faster CPU recommended
  - 512 MB RAM minimum
  - OpenGL 2.0 capable GPU
  - Mac OS X 10.5.4 or newer
  - Also tested with the PowerPC Snow Leopard alpha
  - Dual-processor G5 strongly recommended

  ## Supported Games

  The configurator currently targets early Source Engine titles, including:

  - Portal
  - Half-Life: Source
  - Half-Life Deathmatch: Source
  - Half-Life 2
  - Half-Life 2: Episode One
  - Half-Life 2: Episode Two
  - Half-Life 2: Deathmatch
  - Counter-Strike: Source
  - Day of Defeat: Source

  Some supported titles may still be incomplete or unstable.

  ## Not Supported

  The following games are not currently supported:

  - Left 4 Dead
  - Left 4 Dead 2
  - Portal 2
  - Team Fortress 2
  - Counter-Strike: Global Offensive
  - Dota 2
  - Garry's Mod

  ## How It Works

  Source Engine Configurator only provides the engine runtime and compatibility tooling. It does not include game assets or source code.

  You provide a legitimate Windows, Linux, or Mac install folder for a supported Source game. The configurator verifies the install,
  copies the required game files, applies the PowerPC engine runtime, and creates a standalone Mac `.app`.

  The generated app can then be configured, updated, and launched directly from the configurator.

  ## Installation

  1. Copy your supported Source game folder to your PowerPC Mac.
  2. Open Source Engine Configurator.
  3. Select the game you want to install.
  4. Choose the source game folder.
  5. Choose an output destination.
  6. Configure video and performance options.
  7. Create and launch the generated `.app`.

  ## Graphics Profiles

  The configurator includes hardware-specific rendering profiles for PowerPC Macs.

  Profiles are set automatically depending on your GPU vendor. These profiles control Source Engine console variables used for rendering, presentation, model rendering, lighting, and
  performance tuning.

  ## Updates

  Source Engine Configurator automatically manages updates to the Source Engine PPC runtime - you will be notified when a game update is available. 
  These releases replace only changed engine binaries and support files without requiring the user to reinstall the original
  game data. This allows existing generated `.app` bundles to be patched as the PowerPC port improves.

  ## Legal

  This project does not include Valve game content, game assets, or Source Engine source code.

  You must own a legitimate copy of any game you use with this tool.

  Do not redistribute Valve assets, game folders, maps, models, materials, sounds, scenes, VPKs, or other copyrighted game content.

  This project is provided free of charge for non-commercial preservation, compatibility, and personal-use purposes. Do not sell
  this tool, bundle it with paid products, distribute it behind a paywall, or use it commercially.

  ## Current Status

  This is a work-in-progress PowerPC Source Engine port.

  The current focus areas are:

  - PowerPC rendering correctness
  - ATI and NVIDIA OpenGL driver compatibility
  - Studio model and animation performance
  - Audio timing and stability
  - Broader Source mod compatibility

  ## Roadmap

  Planned or experimental goals include:

  - Better tested Source mod support
  - Native dedicated server support
  - Improved PowerPC/AltiVec optimization
  - Network compatibility with PC servers where possible
  - Source SDK tooling experiments
  - Expanded game compatibility

  ## Known Issues 
  - Issues with depth testing and clip planes on ATI GPUs (causes low performance and seeing through walls)
  - HW skinning is disabled and slower SW skinning is used as a fallback (causes severe performance issues, `r_drawentities 0` in console will increase performance)
  - NPC bone positions are very wrong (causes distorted animations and bad transition graph data)


  ## Credits

  PowerPC port and configurator by doctashay.

  Additional packaging and dependency support from the PPCPorts project.

  Application icon created by maxtron95.

  ## Links

  - GitHub: https://github.com/doctashay/source-engine-configurator
  - PPCPorts Project: https://macos-powerpc.org
