FROM ghcr.io/foundry-rs/foundry:latest

WORKDIR /app
COPY . .

# Build contracts
RUN forge build

EXPOSE 8545

# Run anvil and deploy scripts on startup, or just anvil
CMD ["anvil", "--host", "0.0.0.0", "--port", "8545"]
