<p align="center">
  <h1 align="center">🗂️ listenerResources</h1>
  <p align="center">
    <strong>Remote config for the Telegram deal monitor: the channel list and the price threshold.</strong>
  </p>
  <p align="center">
    <img src="https://img.shields.io/badge/Content-JSON-f7df1e?style=for-the-badge&logo=json&logoColor=white" alt="Content">
    <img src="https://img.shields.io/badge/Consumed_by-telegramMonitor-26a5e4?style=for-the-badge&logo=telegram&logoColor=white" alt="Consumed_by">
  </p>
</p>

---

## ✨ What Is This?

A one-file config repo. [`telegramMonitor`](https://github.com/pratiks360/telegramMonitor) downloads `channels.json` from this repo's raw URL at runtime, so channels can be added or removed with a commit instead of a redeploy.

## 🗂️ Layout

| File | Contents |
|---|---|
| `channels.json` | Owner name, date, `low_deal_price` threshold, the Telegram `channels` to watch and the keyword `filters` that trigger an alert |

## 🔁 How It's Used

```
raw.githubusercontent.com/pratiks360/listenerResources/main/channels.json  ──►  telegramMonitor
```

Edit `channels.json`, push, and the monitor picks the change up on its next refresh.

## 🔒 Privacy Notes

Public channel handles only — no tokens or personal data belong in this file.

---

<p align="center">
  <sub>Built with ❤️ as config-as-a-repo.</sub>
</p>
