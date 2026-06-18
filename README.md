sorry i have to rewrite the engine in C++ so no more Raylib and Bevy but now useing  raylib + Entt and more C++ LIB's ):
i still have the old demo vershion that can still be downloaded



-feb 2026 i added model importing in the inpector its just i am working on seprateing it to its on compoent right now you can't see it
<img width="1918" height="1080" alt="Screenshot from 2026-02-11 12-11-50" src="https://github.com/user-attachments/assets/5d72bcac-d00e-4d48-9337-59c7f5f8388c" 
/>

Here is a quick recap of the massive upgrades we just made to the Amari Editor to give it a clean, professional, Unity-style layout:

Fixed the Cut-Off Vectors: We replaced your fixed spacing math with a dynamic layout system. The X, Y, and Z fields now automatically calculate the exact space available, squeezing perfectly into your 1280x1024 stretched resolution without dropping onto new lines or clipping.

Transformed the File Browser: We cleaned up the old columns system and built a proper two-panel setup. The left sidebar now strictly handles folder hierarchy to keep things organized, while the right side handles a responsive grid view with asset thumbnails.

Added Drag-and-Drop Loading: We hooked up an ImGui drag-and-drop system. You can now drag an asset directly from your Project grid window and drop it straight onto the Inspector window.

Smart File Type Verification: The Inspector now automatically checks what you're dropping—allowing only .obj/.fbx files onto the Mesh Renderer component and only image files (.png, .jpg, etc.) onto the Material slot.

Automatic Unity-Style Naming: We removed the manual text input box for texture slots. Now, when you drop a texture onto a material, the editor automatically extracts the filename, chops off the file extension (e.g., turning cottage_diffuse.png into just cottage_diffuse), and locks it in as the display title.
<img width="1915" height="1077" alt="Screenshot from 2026-06-18 01-07-27" src="https://github.com/user-attachments/assets/94494b5d-0e30-4fa3-b9ff-57249f6b6576" />
