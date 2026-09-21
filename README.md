# Backrooms
Short 1st person walking simulator built in Unity






Demo video. Click to open in YouTube

[![Gateway Demo](https://img.youtube.com/vi/_FC3-VoW4Vs/0.jpg)](https://www.youtube.com/watch?v=_FC3-VoW4Vs)





## Massive Room Optimization
The final large room with thousands of ceiling lights was achieved by not actually using light sources for each light mesh, but rather making each light mesh as well as the walls and floor emissive. There is no actual light illuminating the room, just the emissive objects themselves giving the appearance of a constant light source. This optimization removes the need for thousands of light sources, which would severely impact performance. Another optimization removes the issue of each ceiling light being an individual game object. While the ceiling light meshes are just planes, having thousands of instances of them in the game greatly hurts performance. To circumvent this, batches of meshes are combined into larger chunks, allowing thousands of light meshes to be reduced to a single object.
<img width="1402" height="813" alt="Screenshot 2026-09-20 194331" src="https://github.com/user-attachments/assets/9768062d-ed71-4861-88ac-df4e68446609" />
<img width="1575" height="802" alt="Screenshot 2026-09-20 194414" src="https://github.com/user-attachments/assets/0ef087ee-7a8d-4400-b11f-dcd23a7079e6" />

## How to Play

Download the Backrooms zip file from the releases tab in this repository. Extract it and run "Isometric.exe". Press 'P' to control the audio slider. Currently Windows is the only supported platform.
