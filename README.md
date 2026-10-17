![Banner](img/github-header-banner.png)

# 💫 About Me:
I am a **Smart Contract Engineer** focused on designing, testing, and deploying secure, high-performance, and gas-efficient EVM protocols.


# 💻 Tech Stack:
####  Solidity | Foundry | Anvil | OpenZeppelin | The Graph | Next.js | TypeScript | wagmi | viem | GitHub Actions | Git

# 🚀 Featured Projects:
### [Praedium: Compliance-Gated RWA Tokenization](https://github.com/Rafiitarse/praedium)
Tokenize real-world assets on-chain without losing compliance control. A plain ERC-20 has no idea who is allowed to hold it, so Praedium puts a single on-chain eligibility check in front of every balance change (transfer, mint and burn) against an investor registry. Compliance stops being a promise in a PDF and becomes a property of the protocol.

- **Smart contracts:** Solidity 0.8.28 + Foundry, built on OpenZeppelin v5. `RWAToken` overrides only `_update`, the one funnel every balance change passes through, so no entry point can bypass the gate. Backed by a `ComplianceRegistry` (KYC expiry, jurisdiction codes, freeze, one packed storage slot per investor) and an `AssetRegistry` (document hash, metadata URI, valuation, lifecycle status).
- **Design choice:** freeze, don't claw back. Frozen holders keep their balance until legal resolution, and there is deliberately no forced-transfer function. Four separate roles: minter, pauser, compliance officer and asset admin.
- **Indexing:** a The Graph subgraph tracking transfers, investor status, asset lifecycle and platform counters.
- **Frontend:** a role-aware Next.js dApp (wagmi, viem, Reown AppKit) that shows only what the connected wallet can do, and pre-flights every transfer against the registry so a doomed transaction never gets signed.
- **Testing and CI:** Foundry unit, fuzz and invariant suites, with GitHub Actions running format check, build, tests and coverage on every push.
- **Live on Sepolia:** [`0x53Ff...e109`](https://sepolia.etherscan.io/address/0x53FfF7C20B6DBD66234D769d41EC4C1fA698e109)

### [Time-Weighted ETH Staking Vault](https://github.com/Rafiitarse/time-weighted-staking-vault)
A staking protocol that rewards long-term holders instead of short-term capital. Every deposit is tracked as its own `DepositLot`, so the yield multiplier (0% before 6 months, up to 40% at 3+ years) depends on how long that specific lot has been held.

- **Smart contracts:** Solidity 0.8.27 + Foundry, built on OpenZeppelin `ReentrancyGuard`, `Pausable` and `Ownable`. Receipts (`stETH`) are non-transferable to prevent secondary-market exploits.
- **Indexing:** a The Graph subgraph indexing deposit and withdrawal events.
- **Frontend:** a Next.js dApp for depositing, tracking lots and withdrawing.
- **Testing and CI:** Foundry test suite with coverage reporting, and GitHub Actions CI.
- **Live on Sepolia:** [`0x4EbF...b48Bf`](https://sepolia.etherscan.io/address/0x4EbF2EE5753F729F1D8C166BA36783eD35ab48Bf)

# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api?username=Rafiitarse&theme=dark&hide_border=true&include_all_commits=false&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=Rafiitarse&theme=dark&hide_border=true)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=Rafiitarse&theme=dark&hide_border=true&include_all_commits=false&count_private=false&layout=compact)


## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lintararrafii22) [![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/@Arrafiilintar) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:arrafiilintar@gmail.com)


## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=Rafiitarse&theme=radical&no-frame=false&no-bg=false&margin-w=4)


### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=Rafiitarse&limit=5&theme=dark&combine_all_yearly_contributions=true)



<img data-importer="snake" src="https://raw.githubusercontent.com/Rafiitarse/Rafiitarse/snake-output/snake.svg" alt="Snake animation" />

###

<picture data-importer="pacman">
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Rafiitarse/Rafiitarse/pacman-output/pacman-contribution-graph-dark.svg?game=pacman">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Rafiitarse/Rafiitarse/pacman-output/pacman-contribution-graph.svg?game=pacman">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/Rafiitarse/Rafiitarse/pacman-output/pacman-contribution-graph.svg?game=pacman">
</picture>

###
---
[![](https://komarev.com/ghpvc/?username=Rafiitarse&icon=0&color=0)](https://visitcount.itsvg.in)
<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
