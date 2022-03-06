# ffmpegBlazor-Deployed
 
This is FFmpeg wasm deployed on Netlify(Free Static web site hosting platform), other files are normal Blazorwasm release output files.
Only thing to notice here is `netlify.toml` file
```toml
[[headers]]
  for = "/*"
  [headers.values]
  Cross-Origin-Opener-Policy = "same-origin"
  Cross-Origin-Embedder-Policy = "require-corp"
  ```
  
  On whatever platform you are deploying the site make sure these 2 headers are present.
