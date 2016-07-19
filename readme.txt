command line to generate java protobuf source file:

export SRC_DIR=./justgo
export DST_DIR=./java/
export FILE_NAME=${proto_file_name}

protoc -I=$SRC_DIR --java_out=$DST_DIR $SRC_DIR/$FILE_NAME



command line to generate python protobuf source file:

export SRC_DIR=./justgo
export DST_DIR=./python/
export FILE_NAME=${proto_file_name}

protoc -I=$SRC_DIR --python_out=$DST_DIR $SRC_DIR/$FILE_NAME





Google’s ReadMe:

Protocol Buffers - Google's data interchange format
Copyright 2008 Google Inc.
https://developers.google.com/protocol-buffers/

This package contains a precompiled Win32 binary version of the protocol buffer
compiler (protoc).  This binary is intended for Windows users who want to
use Protocol Buffers in Java or Python but do not want to compile protoc
themselves.  To install, simply place this binary somewhere in your PATH.

This binary was built using MinGW, but the output is the same regardless of
the C++ compiler used.

You will still need to download the source code package in order to obtain the
Java or Python runtime libraries.  Get it from:
  https://github.com/google/protobuf/releases/
