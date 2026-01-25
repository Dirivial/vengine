# Things to know
- GLFW for window & user input management
- GLM for math stuff
- glslc for shader compilation

- To generate compile_options.json: cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=1

# Install (Arch, I don't know about other systems)
- For Intel/AMD (Mesa): sudo pacman -Syu vulkan-headers vulkan-tools vulkan-icd-loader vulkan-validation-layers glfw mesa
- For NVIDIA: sudo pacman -Syu vulkan-headers vulkan-tools vulkan-icd-loader vulkan-validation-layers glfw nvidia-utils
- Optional (recommended for development + samples): install the LunarG Vulkan SDK from AUR (vulkan-sdk) if you want the SDK’s debug layers/binaries.

# Important links
- [Vulkan Tutorial](https://vulkan-tutorial.com/)
