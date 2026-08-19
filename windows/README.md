# Windows native runtime

`onnxruntime.dll` is the x64 binary from Microsoft's
`Microsoft.ML.OnnxRuntime.DirectML` NuGet package version `1.21.0`. This build
contains both the CPU and DirectML execution providers.

- Package URL: `https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime.DirectML/1.21.0`
- Package SHA-256: `12bed6e1e870f30e0150e039ebb6853da32eba381eda1c373faeeb17168785e6`
- DLL SHA-256: `d3c7c34aef827763bb3fe3d6bb1becbae68c70e85dece5c21b973a05911aaa5f`
- Architecture: Windows x64

The corresponding upstream notices are retained in `ThirdPartyNotices.txt`.
DirectML is never selected implicitly by this plugin; callers must append that
provider explicitly and should benchmark it against CPU for their graph.
