# Drosera Safe Wallet Trap Example

This is an example of how to use a Trap to monitor all events emitted from a Safe Wallet. Once an event is detected, the Trap will send an alert to the configured Slack channel.

## Configure dev environment

```bash
curl -L https://foundry.paradigm.xyz | bash && foundryup

# The trap-foundry-template utilizes node modules for dependency management
# install Bun (optional)
curl -fsSL https://bun.sh/install | bash && bun install

# install drosera-cli
curl -L https://app.drosera.io/install | bash && droseraup
```

## Compile the trap
```bash
forge compile
```

## Dry run the trap
```bash
drosera dry-run --block-number <block_number>
```

## Deploy the trap
```bash
drosera apply
```

### Alert Documentation
https://dev.drosera.io/trappers/configuring-alerts
