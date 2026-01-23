FROM mcr.microsoft.com/devcontainers/rust:1-bookworm

# Installation de la cible wasm32 et de trunk
RUN rustup target add wasm32-unknown-unknown \
    && cargo install --locked trunk

# Nettoyage du cache pour réduire la taille de l'image
RUN rm -rf /usr/local/cargo/registry