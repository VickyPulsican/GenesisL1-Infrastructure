<p align="center">
  <img src="images/genesisl1-logo.png" width="140" alt="GenesisL1 Logo">
</p>

<h1 align="center">GenesisL1 Infrastructure</h1>

<p align="center">
Public infrastructure services operated by <b>GenesisL1 Validator – Vicky_Pulsican</b>
</p>

<p align="center">
RPC • REST API • EVM JSON-RPC • WSS • Future Snapshot Service
</p>

---


This repository provides reliable public GenesisL1 infrastructure for developers, validators, wallets, explorers, dApps, and community members.

---

# 🚀 Public Endpoints

## RPC

**Endpoint**

```text
https://rpc.gl1infra.online
```

**Example**

```bash
curl https://rpc.gl1infra.online/status
```

---

## REST API

**Endpoint**

```text
https://api.gl1infra.online
```

**Example**

```bash
curl https://api.gl1infra.online/cosmos/base/tendermint/v1beta1/node_info
```

---

## EVM JSON-RPC

**Endpoint**

```text
https://evm.gl1infra.online
```

**Example**

```bash
curl -X POST https://evm.gl1infra.online \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}'
```

---

## WebSocket (WSS)

**Endpoint**

```text
wss://wss.gl1infra.online
```

**Example**

```bash
wscat -c wss://wss.gl1infra.online \
-x '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}'
```

---

# 📦 Snapshot

**Status**

```text
🚧 Coming Soon
```

A public GenesisL1 snapshot service will be added once it has been fully tested and verified for production use.

---

# 📊 Infrastructure Status

| Service | Endpoint | Status |
|----------|----------|--------|
| RPC | https://rpc.gl1infra.online | ✅ Online |
| REST API | https://api.gl1infra.online | ✅ Online |
| EVM JSON-RPC | https://evm.gl1infra.online | ✅ Online |
| WebSocket (WSS) | wss://wss.gl1infra.online | ✅ Online |
| Snapshot | Coming Soon | 🚧 In Preparation |

---

# 🧪 Health Checks

### RPC

```bash
curl -s https://rpc.gl1infra.online/status | jq '.result.sync_info'
```

### REST API

```bash
curl -s https://api.gl1infra.online/cosmos/base/tendermint/v1beta1/node_info | jq
```

### EVM

```bash
curl -s -X POST https://evm.gl1infra.online \
-H "Content-Type: application/json" \
-d '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}' | jq
```

### WSS

```bash
wscat -c wss://wss.gl1infra.online \
-x '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}'
```

---

# 🛡️ Validator Information

**Validator Name**

```text
Vicky_Pulsican
```

**Identity**

```text
DB008A038B4F1018
```

**Validator Address**

```text
genesisvaloper1hvan9p4ghg6xz26ksgw9vkhghkvxfq0shh60n2
```

---

# 📌 Notes

- All public infrastructure services are hosted on a dedicated infrastructure server.
- The infrastructure server is independent from the validator server.
- Services are monitored and maintained for stability and high availability.
- Additional infrastructure services (such as public snapshots) will be added in future updates.

---

# ❤️ Support

If these public endpoints are useful for your project or development, please consider:

- Using them in your applications
- Reporting any issues
- Sharing feedback or suggestions

Together we can help strengthen the GenesisL1 ecosystem.
