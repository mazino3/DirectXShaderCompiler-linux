# Copyright (C) Microsoft Corporation. All rights reserved.
# This file is distributed under the University of Illinois Open Source License.
# See LICENSE.TXT for details.

add_llvm_library(LLVMDxilCompression
  DxilCompression.cpp
  miniz.c

  ADDITIONAL_HEADER_DIRS
)

add_dependencies(LLVMDxilCompression intrinsics_gen)

