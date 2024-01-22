# PRINCIPLED BSDF

Combines multiple layers into single node. Can model wide variety of materials. Based on OpenPBR Surface shading model, provides params compatible with similar PBR shaders found in software such as Disney and Standard Surface models.

![Principled BSDF](/assets/shader/principled-bsdf.png)

When adding new material, by default get Principled BSDF and Material Output nodes. Material Output node needs to be connected or it'll appear black.

Volume socket refers to volumetric properties to add to object. Displacement adds depth details to mesh without adding geometry.

Base Color, Metallic, Roughness, and Emission are some basic attributes. Emission particularly visible when Bloom turned on in Render panel.

![Bloom](/assets/interface/bloom.png)

Subsurface refers to subsurface scattering (light penetrating partially), most applicable to organic materials (skin, hair).

Specular most important to materials heavy on reflection.

Sheen best used with fabrics. Need textures.

Clearcoat adds glass-like white shine.

IOR (Index of Refraction) and Transmission affect how light passes through object. Set Transmission to 1 for glass shader.
