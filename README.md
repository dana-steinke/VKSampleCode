To set up Visual Studio, navigate to the project properties under the Project tab. Under C/C++ > General > Additional Include Directories, add the file locations for:
glfw-3.4.bin.WIN64\glfw-3.4.bin.WIN64\include
glm-1.0.1-light
stb-master\stb-master
tinyobjloader-release\tinyobjloader-release
Under Linker > General > Additional Library Directories, add the file locations for:
VulkanSDK\1.3.283.0\Lib
glfw-3.4.bin.WIN64\glfw-3.4.bin.WIN64\lib-vc2022
Under Linker > Input > Additional Dependencies, add the file locations for:
VulkanSDK\1.3.283.0\Lib\vulkan-1.lib
glfw-3.4.bin.WIN64\glfw-3.4.bin.WIN64\lib-vc2022\glfw3.lib
Under C/C++ > Language > C++ Language Standard, make sure it is set to ISO C++17 Standard.

To load custom objects, put the .obj file into the objects folder and the texture into the textures folder. Replace 'const std::string MODEL_PATH = "models/viking_room.obj";
const std::string TEXTURE_PATH = "textures/viking_room.png";' with the names of the files. If it does not render correctly, the object may be too big and will need to be resized. 
