# NeuralPayRouter

NeuralPayRouter — A Smart Contract Payment Mesh in Solidity

I designed and audited a full build upgradeable Solidity smart contract payment protocol with reentrancy protection, role-based access control, and a 25-test suite.

This neural-net-inspired payment routing system is a network of "nodes" (smart contracts) that intelligently route payments through weighted paths, split funds, and self-optimize fees. 

Advanced Solidity patterns (upgradeable contracts, reentrancy guards, access control)
Security auditing mindset (every known vulnerability addressed + documented)
System design thinking (modular architecture)
Testing discipline (full test suite)

A Solidity protocol where payments travel through a graph of registered "nodes" (like neurons), each taking a small fee and passing funds along. It's original, visually explainable to investors, and shows serious engineering discipline.

Files include: 
contracts/core/NeuralPayRouter.sol — The main 300-line contract (upgradeable, role-based, reentrancy-safe)
contracts/libraries/WeightMath.sol — Fixed-point math with sigmoid & EMA functions
contracts/libraries/PathValidator.sol — Validates payment paths, prevents cycles
contracts/mocks/MaliciousRecipient.sol — An attack contract used to prove reentrancy protection works
test/NeuralPayRouter.test.ts — 25+ tests covering attacks, edge cases, and happy paths
audit/AUDIT_REPORT.md — A profe ssional-style security audit report
scripts/deploy.ts — One-command deployment to Sepolia testnet

In my next Solidity Language Smart Contract project I modify this dApp for use as an employer payroll.
3. The net pay amount is passed to a smart contract 
4. The contract distributes payment in USD, BTC, ETH, or other crypto 
5. It goes directly to the employee's wallet or bank account — no middleman
