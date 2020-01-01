# Rice2D-PostProcess

Post-process shader for Rice2D

1. Add `postprocess.frag.glsl` to your `Shaders` folder in Rice2D project.
2. And make following change to your `khafile.js`:
```js
// List of post-process shader defines: chromatic_abberation, tonemap_reinhard, tonemap_uncharted2, tonemap_acesfilm, vignette
// Add define (atleast one from above list) for particular post-process like,
project.addShaders('Shaders/**', {
    defines: [
        'chromatic_abberation',
        'tonemap_reinhard'
    ]
});

// Add rice_postprocess define to enable post-process
project.addDefine('rice_postprocess');
```
