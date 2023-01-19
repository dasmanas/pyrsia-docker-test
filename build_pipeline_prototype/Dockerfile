FROM rust:1.66.1-buster
ARG RUST_VERSION
RUN apt-get update; \
    apt-get -y install git-all curl clang llvm libclang-dev jq protobuf-compiler;
RUN rustup default ${RUST_VERSION}; \
    git clone https://github.com/tiainen/pyrsia_build_pipeline_prototype.git;
WORKDIR pyrsia_build_pipeline_prototype