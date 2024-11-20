# Always Night Mod for 7 Days to Die

This mod for **7 Days to Die** forces the in-game world to stay at night, ensuring that the player experiences a permanent nighttime environment. This is ideal for players who want a more challenging and atmospheric game

## Features

- Forces the world time to remain at **night**.
- The mod is fully compatible with other mods that do not interfere with the time system.
- Configurable (optional): Change the night duration or world time based on your preference.

## Requirements

- **7 Days to Die** (version compatible with your mod's patching).
- **Harmony** library (included with the mod).

## Installation

1. **Download the mod**:  
   [Click here to download the mod]([#](https://github.com/MoreKronos/Always-Night-7d2d-Mod/releases)) scroll around for a release that suits you

2. **Clone or download this repository** to your computer.

3. **Copy the mod files**:  
   Copy the folders downloaded from this repository and place it in your **7 Days to Die Mods** folder, making sure it is unzipped .  
   By default, the Mods folder is located here:  
   `C:\Program Files (x86)\Steam\steamapps\common\7 Days To Die\Mods`

4. **Install Harmony Library**:  
   This mod requires **Harmony** to patch the game. Ensure that **Harmony** is included in your mod's folder or otherwise use the one added to the mod download.

5. **Launch the game**:  
   Start **7 Days to Die**. The mod will automatically be applied.

## How It Works

This mod uses the **Harmony** patching library to override the default world time getter method in the game. By hooking into the game’s `World` class, it intercepts the time calculation and forces it to remain at **night** (world time set to 25000, which corresponds to night in the game).

### Key Technical Details

- **Target Method**: The mod targets the `SetWorldTime` or equivalent method in the `World` class (using Harmony’s reflection system).
- **Patch Logic**: The patch forces the game to skip over its default world time getter and instead always return the value for **night**.

## How to Use

Once the mod is installed:
- **No configuration is needed**: The world will always remain at night.
- You can modify the mod's source code if you wish to adjust the time of day or enable specific conditions for when it becomes night.

## Troubleshooting

- **Mod not working?** Ensure you have placed the mod in the correct folder: `7DaysToDie/Mods/AlwaysNight/`.
- **Harmony issues?** Make sure that the Harmony mod is installed and properly initialized.
- **Game crashes**: If the game crashes or behaves unexpectedly, check the mod log for any errors related to time patching.

## Development

This mod uses the [Harmony](https://github.com/pardeike/Harmony) library to patch methods in 7 Days to Die. It modifies the game's world time to always remain at night. If you are interested in contributing or modifying the mod, feel free to fork the repository and submit a pull request.

### Contributing

1. Fork the repository.
2. Create your feature branch.
3. Commit your changes.
4. Push to the branch.
5. Open a pull request.

### License

This mod is released under the **MIT License**. Feel free to use, modify, and distribute it, as long as you credit the original author.

---

## Contact

For any questions, issues, or feature requests, feel free to open an issue in the GitHub repository, or reach out via [email](mailto:your-email@example.com).

