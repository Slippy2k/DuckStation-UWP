# DuckStation-UWP (ARM)
Fast PlayStation 1 emulator for Windows ARM32 (UWP)

## Compatibility 
- Windows Build (15035+)
- DirectX 11 Feature Level 10+
- DirectX 11 Feature Level 9.1 (Partially, Software render)
- Don't enable recompiler option still not working

## Surface (ARM64)
- Please note Qualcomm and Windows are no longer support ARM32 (which what I do)
- Good news is the ARM64 is officially adopted [Click here](https://github.com/stenzek/duckstation/releases)
- My work is focus on legacy support for older devices and ARM devices that still support ARM32

## Performance
After few tests it worked good on `Adreno 330` but slow on `Adreno 305`

You may achieve better performance by manipulating Speed options

GPUs `Adreno 400+` are perfect and they will work with full speed.

## Screenshots
<details>
<summary>Screenshots</summary>
<img src="https://github.com/basharast/DuckStation-UWP-ARM/assets/3244951/2b1b1f81-2d41-45bf-8862-0c010725cab8" width="760"/>
<img src="https://github.com/basharast/DuckStation-UWP-ARM/assets/3244951/5fd26bb4-3a2c-477c-922a-4a0284dd8a7f" width="250"/>
<img src="https://github.com/basharast/DuckStation-UWP-ARM/assets/3244951/8637920b-34e6-4da3-bf1e-0ac4ff687a62" width="250"/>
<img src="https://github.com/basharast/DuckStation-UWP-ARM/assets/3244951/b1e61420-86f9-4816-ba7a-9ac39a404c52" width="250"/>
</details>


## Overview:
[DuckStation](https://github.com/stenzek/duckstation) is PS1 emulator by [Connor McLaughlin](https://github.com/stenzek) (stenzek)

This emulator is really good and fast even on old ARM devices like Windows Phone, all credits goes to **stenzek**


## UWP Support
Supported by **[UWP2Win32](https://github.com/basharast/UWP2Win32)**


## What's new?

- UWP Storage solution
- You can choose custom data folder
- Include and improved touch screen functions
- Added On-Screen touch controller
- Improved files browser
- Fixed few issues with retroachievements
- Other minor fixes related to (Windows Legacy builds, Touch and UWP)
- Support launch by file or URI


## Help

Checkout the official documentation ([Click here](https://github.com/stenzek/duckstation/wiki))

Read about features and performance tips ([Click here](https://github.com/basharast/DuckStation-UWP-ARM/wiki))


# Build 

This was hardly ported to older hardware, things aren't organized

I don't care about code quality more than the result

if you are going to build this for modern hardware, use the official repo

there are certain changes added for testing the performance on older hardware

before you start note the following:

- I'm un-aware nor I care for any issues on ARM64 or x64 (runtime or build)

- This port meant for older hardware which use ARM32.

- Don't post any issue related to other than ARM32

- If you saw the src around 1GB it maybe because there was some compiled stuff are in sub folders and I made it quickly, and no time to safely clean those.

## Steps

Ensure to have:
- SDK: 10240, 17763, 19041
- Visual Studio 2022 ( with platform tools v143)
- Only use ReleaseUWP (tested for ARM, ARM64 and x64)

## Important

Some linked projects at Dependencies require to be build manually

like project `util`, I guess also `fmt`, in anycase you got that `.lib` is missing

go to Dependencies and build it manually (Right click, Build)


# Credits

Connor McLaughlin (stenzek) DuckStation Emulator

ImGui (Dear ImGui) [Omar](https://github.com/ocornut/imgui)

Bashar Astifan (UWP Storage manager and other UWP improvements)
