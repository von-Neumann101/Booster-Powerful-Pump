# Booster Powerful Pump

## 中文说明

Booster Powerful Pump 是一个面向 Minecraft Forge 1.20.1 的 Create 附属模组。

当前模组新增一个 Create 兼容方块：

- `booster:powerful_mechanical_pump`
- 英文名：Powerful Mechanical Pump
- 中文名：强力机械泵

强力机械泵继承 Create 原版机械泵的基础行为，接入 Create 原版流体管网。它拥有更高的基础应力消耗，并通过配置倍率提高写入 Create 流体网络的 pressure，从而提升实际流体吞吐量。

### 环境要求

- Minecraft `1.20.1`
- Forge `47.1.33`
- Create `6.0.8`
- Java `17`
- Mod ID：`booster`

### 构建

在项目根目录运行：

```powershell
.\gradlew.bat build
```

构建产物位置：

```text
build/libs/booster-1.20.1-0.1.0.jar
```

### 开发环境运行

```powershell
.\gradlew.bat runClient
```

### 配置

服务端配置文件：

```text
booster-server.toml
```

主要配置项：

- `powerfulPumpStressImpact`：默认 `16.0`
- `powerfulPumpPressureMultiplier`：默认 `8.0`

注意：已经创建过的世界会保留自己的 `serverconfig/booster-server.toml`。如果修改了默认值，旧世界需要手动修改对应世界目录下的配置文件，并重启世界或服务器。

### 当前功能范围

- 新增强力机械泵方块、物品和 BlockEntity。
- 复用 Create 原版机械泵和流体管网逻辑。
- 提高基础应力消耗。
- 提高写入 Create 流体网络的 pressure。

## English

Booster Powerful Pump is a Create addon mod for Minecraft Forge 1.20.1.

This mod currently adds one Create-compatible block:

- `booster:powerful_mechanical_pump`
- English name: Powerful Mechanical Pump
- Chinese name: 强力机械泵

The Powerful Mechanical Pump extends Create's Mechanical Pump behavior and integrates with Create's existing fluid pipe network. It has a higher base stress impact and uses a configurable pressure multiplier to increase the pressure written into Create's fluid network, improving actual fluid throughput.

### Requirements

- Minecraft `1.20.1`
- Forge `47.1.33`
- Create `6.0.8`
- Java `17`
- Mod ID: `booster`

### Build

Run from the project root:

```powershell
.\gradlew.bat build
```

The built jar is written to:

```text
build/libs/booster-1.20.1-0.1.0.jar
```

### Development Client

```powershell
.\gradlew.bat runClient
```

### Configuration

Server config file:

```text
booster-server.toml
```

Important keys:

- `powerfulPumpStressImpact`: default `16.0`
- `powerfulPumpPressureMultiplier`: default `8.0`

Existing worlds keep their own `serverconfig/booster-server.toml`. If you change defaults after a world has already been created, edit that world's config file and restart the world or server.

### Current Scope

- Adds the Powerful Mechanical Pump block, item, and BlockEntity.
- Reuses Create's original Mechanical Pump and fluid network logic.
- Increases base stress impact.
- Increases pressure written into Create's fluid network.
- 
