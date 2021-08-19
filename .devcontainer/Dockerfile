FROM rust:latest

WORKDIR /opt/rustlings

# install dependencies
COPY Cargo* ./
COPY src/ ./src
COPY README.md .

RUN cargo install --force --path .

# install prerequisites for vscode extension
RUN rustup component add rust-analysis
RUN rustup component add rust-src
RUN rustup component add rls