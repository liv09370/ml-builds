# ML Builds

Pre-built shared libraries for machine learning

Library | Linux | Mac | Windows | Assets | Notes
--- | --- | --- | --- | --- | ---
[BlingFire](https://github.com/Microsoft/BlingFire) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/blingfire-master) |
[Faiss](https://github.com/facebookresearch/faiss) | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/faiss-1.6.1) |
[Interpret](https://github.com/interpretml/interpret) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/interpret-0.1.20) | |
[LIBMF](https://github.com/cjlin1/libmf) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/libmf-master) | Fork, OpenMP disabled
[Multicore t-SNE](https://github.com/DmitryUlyanov/Multicore-TSNE) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/multicore-tsne-master) |
[NGT](https://github.com/yahoojapan/NGT) | ✓ | ✓ | n/a | [View](https://github.com/ankane/ml-builds/releases/tag/ngt-1.10.0) |
[SCS](https://github.com/cvxgrp/scs) | ✓ | ✓ | | [View](https://github.com/ankane/ml-builds/releases/tag/scs-2.0.2) |
[ThunderSVM](https://github.com/Xtra-Computing/thundersvm) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/thundersvm-0.3.4) |
[XGBoost](https://github.com/dmlc/xgboost) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xgboost-1.0.2) | OpenMP disabled (Windows)
[xLearn](https://github.com/aksnzhy/xlearn) | ✓ | ✓ | ✓ | [View](https://github.com/ankane/ml-builds/releases/tag/xlearn-0.4.4) |

View the [build scripts](.github/workflows)

Some projects include shared libraries as part of their releases:

- [LibTorch](https://pytorch.org/)
- [LightGBM](https://github.com/microsoft/LightGBM/releases)
- [ONNX Runtime](https://github.com/microsoft/onnxruntime/releases)
- [OR-Tools](https://developers.google.com/optimization/install/cpp)
- [OSQP](https://bintray.com/bstellato/generic/OSQP#files)

## Details

For portability:

- Linux libraries are built with older `glibc` (todo: build with much older) and `-march=x86-64` (when possible)
- Mac libraries are built with `-march=nehalem` (same as Homebrew) and `MACOSX_DEPLOYMENT_TARGET=10.13`

[Reference](https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html)
