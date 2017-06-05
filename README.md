# 3dsdump [JetZux]

## Dump ancient 3ds info

## Change Log
### 2015-05-29 
#### added
- +. show track info
- +. show key info

### 2015-10-20
- +. show pivot matrix

## .3ds chunks info (from wiki)
0x4D4D // Main Chunk
  0x0002 // M3D Version
  0x3D3D // 3D Editor Chunk
    0x4000 // Object Block
      0x4100 // Triangular Mesh
        0x4110 // Vertices List
        0x4120 // Faces Description
          0x4130 // Faces Material
          0x4150 // Smoothing Group List
        0x4140 // Mapping Coordinates List
        0x4160 // Local Coordinates System
      0x4600 // Light
       0x4610 // Spotlight
      0x4700 // Camera
    0xAFFF // Material Block
       0xA000 // Material Name
       0xA010 // Ambient Color
       0xA020 // Diffuse Color
       0xA030 // Specular Color
       0xA200 // Texture Map 1
       0xA230 // Bump Map
       0xA220 // Reflection Map
          /* Sub Chunks For Each Map */
          0xA300 // Mapping Filename
          0xA351 // Mapping Parameters
  0xB000 // Keyframer Chunk
     0xB002 // Mesh Information Block
     0xB007 // Spot Light Information Block
     0xB008 // Frames (Start and End)
        0xB010 // Object Name
        0xB013 // Object Pivot Point
        0xB020 // Position Track
        0xB021 // Rotation Track
        0xB022 // Scale Track
        0xB030 // Hierarchy Position
