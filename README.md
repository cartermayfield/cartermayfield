# Hi, I'm Carter Mayfield 👋

CS at **The University of Texas at Austin** ('29). I build production systems that trade real money on live sports markets.

📫 [carter.mayfield.jr@gmail.com](mailto:carter.mayfield.jr@gmail.com) · [LinkedIn](https://www.linkedin.com/in/carter-mayfield-jr-9b7652272)

---

## 🎾 Tennis Ops — algorithmic trading on live tennis markets

Tennis Ops is an end-to-end automated trading system for in-play professional tennis on two regulated exchanges (**Kalshi** and **Polymarket US**). The repo is private because it runs live capital and a proprietary strategy, but I'm happy to walk through any part of it in depth.

- **Six trading bots** (~94,000 lines of Python) autonomously placing, repricing, and canceling orders — **$6,800+ realized profit (+112.3% NAV return) across 2,400+ trades** in the first 1.5 months live
- **Modeling** — a nested Markov-chain win-probability model (Barnett–Clarke) with Bayesian serve-strength priors, plus XGBoost trade selectors retrained weekly by an automated crawl-and-refit pipeline tuned with Optuna
- **Data platform** — 10+ collector daemons running 24/7 (live scores from two independent feeds, order-book depth, trade tape, settlements) writing Parquet datasets, hardened with fail-closed guards and staleness tripwires
- **Research discipline** — 150+ research cycles under preregistration: out-of-sample time splits, match-clustered standard errors, Benjamini–Hochberg corrections, fee-aware executable-fill backtests. **70+ candidate strategies falsified** before one was deployed
- **Validation before capital** — flagship market-making strategy preregistered and validated out-of-sample at **+12.8% stake-weighted ROI (t = 5.0)** before committing money; live stakes sized with fractional Kelly and Monte Carlo capacity simulations
- **Production ops** — live portfolio dashboard (P&L, NAV, clustered t-statistics), automated daily audits of sizing/pricing/selector adherence, one-command restart tooling

---

## 💼 Previously

**DevOps Intern @ SWIVEL, an SWBC Company** (Summer 2026) — Platform engineering on a payments platform: migrated Docker build secrets across 10+ microservice repos, built reusable GitHub Actions for secure image builds, moved production images to a private registry with AWS ECR, and remediated Trivy-flagged container vulnerabilities.

---

## 🛠 Toolbox

**Proficient:** Java · Python · C · Git/GitHub · GitHub Actions (CI/CD) · Docker & Dockerfiles · private container registries · Claude Code · GitHub Copilot

**Familiar:** AWS (CloudFormation, ECR, ECS, EC2) · XGBoost · Trivy container scanning

**Working Knowledge:** XGBoost · PyArrow/Parquet · pandas · NumPy · scikit-learn · Optuna · C#
