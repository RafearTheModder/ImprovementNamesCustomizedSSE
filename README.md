# Improvement Names Customized SSE
Improvement Names Customized ported for Skyrim VR.
It has also been restructured to use CMake and newer CommonLib versions.

## Requirements
* [CMake](https://cmake.org/)
    * Add this to your `PATH`
* [PowerShell](https://github.com/PowerShell/PowerShell/releases/latest)
* [Vcpkg](https://github.com/microsoft/vcpkg)
    * Add the environment variable `VCPKG_ROOT` with the value as the path to the folder containing vcpkg
* [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
    * Desktop development with C++
* [CommonLibVR](https://github.com/RafearTheModder/CommonLibVR/tree/vr)
    * You need to build from the RafearTheModder/vr branch
    * Add this as as an environment variable `CommonLibVRPath`

## User Requirements
* [VR Address Library for SKSEVR](https://www.nexusmods.com/skyrimspecialedition/mods/58101)
    * Needed for VR

## Register Visual Studio as a Generator
* Open `x64 Native Tools Command Prompt`
* Run `cmake`
* Close the cmd window

### Building for VR
```
cmake --preset vs2022-windows-vcpkg-vr
cmake --build buildvr --config Release
```

## Settings
Setting | Description
--- | ---
`style` | The improvement string display style. Valid inputs are: `"Vanilla"`, `"VanillaPlus"`, `"PlusN"`, `"Internal"`, `"Custom"`, and `"RomanNumeral"`.
`prefix` | The improvement string prefix.
`postfix` | The improvement string postfix.
`customNames` | A set of strings to be used when `"Custom"` style is selected.

## License
[MIT](LICENSE)