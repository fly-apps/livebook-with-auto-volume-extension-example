# livebook-with-auto-volume-extension-example

This is a simple example on how to use auto volume extension from your fly.toml

The magic comes from the fields called `auto_extend_*` under your mounts section

```toml
[[mounts]]
  source = "data"
  destination = "/data"
  auto_extend_size_threshold = 80
  auto_extend_size_increment = "1GB"
  auto_extend_size_limit = "5GB"
```

https://github.com/fly-apps/livebook-with-auto-volume-extension-example/blob/d5dd0d8a6921d7a05e36ab6eb20a31f275996de9/fly.toml#L22-L24
