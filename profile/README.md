<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./logo.png">
    <source media="(prefers-color-scheme: light)" srcset="./logo_light.png">
    <img alt="MadhyaSigma" src="./logo.png" width="480">
  </picture>
</div>

---

We're a technology-first trading operation — we design, build, and run our own algorithmic trading infrastructure end-to-end, and trade our own capital on it. Our approach starts from risk, not returns: every strategy is built to minimize downside first, with income generated as a disciplined outcome of that risk control rather than the goal itself.

The platform is built to run every stage of that process — developing a strategy, deploying it, and operating it live — under proper access control. It's designed to work whether you're a single quant running your own book or a full team of researchers, portfolio managers, and traders operating together.

## Platform capabilities

**Execution**
- Multi-underlying, multi-leg, multi-broker order execution with configurable risk profiles per order
- One-click kill switch, at both the individual strategy and account level
- Unified order-routing layer across multiple broker connections — strategy code is written once and can execute through any connected broker
- A low-latency communication layer between strategies, execution, and brokers, built as core infrastructure rather than an afterthought

**Market data & risk**
- Live option chain with real-time Greeks
- Real-time portfolio risk analytics computed directly off the market, not bolted on after the fact

**Strategy lifecycle**
- Web-based code editor for building strategies directly on the platform
- A no-code strategy builder, with the ability to define custom indicator math and apply it to any asset *(in development)*
- Live per-strategy logs and a control panel for monitoring, managing, and reporting on everything that's running

**Operations & access**
- A paper-trading environment that mirrors live execution exactly, so strategies get proven out before they touch real capital
- Multi-user access with role-based permission levels — portfolio manager, trader, investor — built for running a quant operation solo or as a team

## How it's built

- `trading-core` — the strategy runtime and shared trading library
- `trading-api` — the central API layer strategies and the UI talk to
- `trading-order-service` — multi-broker order distribution and fill sync
- `trading-brokers` — broker-specific execution adapters
- `trading-strategies` — the strategies themselves
- `trading-paper-broker` — the paper-trading simulator
- `trading-ui` — the internal dashboard for monitoring, execution, and risk

Repos are private — this is infrastructure we trade real money on, not open-source tooling.

---

<div align="center">

*Building the system, one trading day at a time.*

</div>
