# HOI4 Mod Utilities

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![VSCode Marketplace](https://img.shields.io/vscode-marketplace/v/TheCascadian.hoi4modutilities?label=VSCode%20Marketplace)](https://marketplace.visualstudio.com/items?itemName=TheCascadian.hoi4modutilities)

A modernized VSCode extension providing utilities for Hearts of Iron IV mod developers.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Extension Settings](#extension-settings)
- [Known Issues](#known-issues)
- [Release Notes](#release-notes)
- [Contributing](#contributing)
- [License](#license)
- [Original README (paraphrased)](#original-readme-paraphrased)

## Features

- World map preview  
- National focus & technology tree visualization  
- Event tree hierarchy display  
- Military-industrial organization (MIO) overview  
- GUI component preview  
- `.gfx` sprite definitions  
- `.dds` & `.tga` image previews  

## Installation

1. Install the extension from the VSCode Marketplace.  
2. Configure the HOI4 install directory:  
   - Use **Select HOI4 Install Path** in the command palette (`Ctrl+Shift+P`), or  
   - Set `hoi4ModUtilities.installPath` in your settings.  
3. Open your mod development folder.  
4. *(Optional)* Select a `.mod` file via **Select Mod File** in the command palette.  

## Usage

- **Command Palette** (`Ctrl+Shift+P`):  
  - **Preview World Map**  
  - **Preview HOI4 File**  
- **Editor Toolbar Button** (visible on `.gfx`, `map/default.map`, focus/tech tree files): launches **Preview HOI4 File**.

## Extension Settings

| Setting                                | Type       | Description                                                                                    |
|----------------------------------------|------------|------------------------------------------------------------------------------------------------|
| `hoi4ModUtilities.installPath`         | `string`   | Path to your Hearts of Iron IV installation (required).                                       |
| `hoi4ModUtilities.loadDlcContents`     | `boolean`  | Include DLC assets in previews (increases memory usage).                                      |
| `hoi4ModUtilities.modFile`             | `string`   | Path to the active `.mod` descriptor (defaults to first found).                                |
| `hoi4ModUtilities.enableSupplyArea`    | `boolean`  | Enable supply area rendering for HOI4 ≤ v1.10.                                                  |
| `hoi4ModUtilities.previewLocalisation` | `enum`     | Language for event tree content.                                                              |
| `hoi4ModUtilities.featureFlags`        | `string[]` | Feature flags to toggle capabilities (reload required).                                        |

## Known Issues

- Focus tree GUI lacks configuration options available to the tech tree.  
- World map border lines may misalign with color regions.  
- Event tree may show duplicate entries when events appear in multiple options.  

## Release Notes

<a name="0.12.2"></a>
### [0.12.2] – 2025-05-XX
- **Fixed**: Support for `|` in symbol types (e.g., `building_state_modifier|dam`) (#105).

## Contributing

- Report issues or request features via [GitHub Issues](https://github.com/TheCascadian/hoi4modutilities/issues).  
- Submit localization updates by pull request to the `i18n` folder.  
- Acknowledgments available in the [CONTRIBUTORS.md](CONTRIBUTORS.md).

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Original README (paraphrased)

```text
HOI4 Mod Utilities: VSCode tools for Hearts of Iron IV modders. Includes map, focus tree, event tree, tech tree, MIO, GUI, `.gfx` & image previews. To start: install extension, set install path (via command or setting), open mod folder, optionally select `.mod`, then use preview commands or toolbar. Settings cover installPath, load DLC, modFile, supply area, localization, feature flags. Known issues: focus GUI config, map edge alignment, duplicate event entries. Release 0.12.2 adds support for `|` in symbol types. Contribute via issues/PRs. Licensed under MIT.
