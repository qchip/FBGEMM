# Copyright (c) Meta Platforms, Inc. and affiliates.
# All rights reserved.
#
# This source code is licensed under the BSD-style license found in the
# LICENSE file in the root directory of this source tree.

################################################################################
# Target Sources
################################################################################

set(experimental_triton_python_source_files
    triton_gemm/__init__.py
    triton_gemm/fp8_gemm.py
    triton_gemm/matmul_perf_model.py)


################################################################################
# Install Python Files
################################################################################

add_to_package(DESTINATION fbgemm_gpu/experimental/gemm/triton_gemm
    FILES ${experimental_triton_python_source_files})
