# 3d-particles
*A starter repository from the Awwwards workshop class "Impress everyone with a 3D particle scene starting from bad models"*

---
## Requirements
Make sure you have [Node.js](https://nodejs.org/it/) installed on your machine.
- Required minimum Node version: at least 10
- Required minimum NPM version: at least 6

Download and install [Blender](https://www.blender.org/)
- Required minimum Blender versione: 2.91.2

---
## Install & Run
Download the repo on your machine, enter the repo folder with your terminal and run the following

```
npm install
```

After installing all depencies, you can run the server with
```
npm run start
```
that will open a new window on your browser http://localhost:8080/

---
## Links
### 🤓 Dev
- [Node.js](https://nodejs.org/it/)
- [Parcel.js](https://parceljs.org/)
  - [parcel-plugin-static-files-copy](https://www.npmjs.com/package/parcel-plugin-static-files-copy)
- [Three.js](https://threejs.org/)
  - [Particles Example](https://threejs.org/examples/?q=particles#webgl_buffergeometry_custom_attributes_particles)
  - [MeshSurfaceSampler](https://threejs.org/docs/#examples/en/math/MeshSurfaceSampler)
- [Gsap](https://greensock.com/gsap/)
- [VisualCode](https://code.visualstudio.com/)
  - [Shader languages support for VS Code - Extension](https://marketplace.visualstudio.com/items?itemName=slevesque.shader)

### 🗿 3D
- [Blender](https://www.blender.org/)
- [Free3d](https://free3d.com/)
- [Skull 3D Model](https://free3d.com/3d-model/skull-v3--785914.html)
- [Horse 3D Model](https://free3d.com/3d-model/american-paint-horse-nuetral-v1--575385.html)

### 🪄 Further Readings
- [The Book of Shaders](https://thebookofshaders.com/)
- [Three.js Foundamentals](https://threejsfundamentals.org/)
- [WebGL Foundamentals](https://webglfundamentals.org/)

---

### 📝 Vertex Shader Sample
``` 
void main() {
  vec4 mvPosition = modelViewMatrix * vec4( position, 1.0 );
  gl_Position = projectionMatrix * mvPosition;
  gl_PointSize = 8.0 / -mvPosition.z;
}
```

### 📝 Fragment Shader Sample
``` 
void main() {
 gl_FragColor = vec4(1.0, 1.0, 1.0, 1.0);
}
```

---

## Troubleshooting
- [Troubleshooting installing Node](https://github.com/mattdesl/bartlett-dfpi/blob/362ac5b0ef5d195114f496284f11798b2ca0fd05/guides/node-and-npm.md#troubleshooting-eaccess-errors)
