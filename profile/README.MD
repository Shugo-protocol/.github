<div align="center">

```text
   _____ __  ____  _____________ 
  / ___// / / / / / / ____/ __ \
  \__ \/ /_/ / / / / / __/ / / /
 ___/ / __  / /_/ / /_/ / /_/ / 
/____/_/ /_/\____/\____/\____/  
       守 護  /  शु गो
shugo protocolopen-source cryptographic guardrail standards for autonomous agent economies on solana.website • documentation • specification • securitymissionthe agentic economy cannot scale on raw private key delegation. autonomous agents given unconditional custody over hot wallets inevitably fail due to prompt injection, model hallucinations, or poisoned calldata.shugo protocol (守護) engineers zero-custody execution standards for solana. our protocols separate asset ownership from transaction signing authority:custody remains native: vault capital stays in cold human wallets or multisigs.execution is delegated: agents sign transactions using ephemeral keys metered by on-chain policies.invariants are provable: velocity caps, program allowlists, and revocation paths are mathematically verified.protocol stackPlaintext+-----------------------------------------------------------------------------+
|                            APPLICATION LAYER                                |
|         elizaos agents  •  langchain runtimes  •  autonomous bots           |
+-----------------------------------------------------------------------------+
                                       |
                                       v
+-----------------------------------------------------------------------------+
|                           TOOLING & CLIENT LAYER                            |
|             @shugo-protocol/sdk  •  shugo-cli  •  agent-plugins             |
+-----------------------------------------------------------------------------+
                                       |
                                       v
+-----------------------------------------------------------------------------+
|                           PROTOCOL POLICY ENGINE                            |
|        programs/guard (solana anchor)  •  aws kani formal verification      |
|           • epoch velocity meters      • cpi target allowlists              |
|           • atomic revocation hooks    • balance threshold ceilings         |
+-----------------------------------------------------------------------------+
                                       |
                                       v
+-----------------------------------------------------------------------------+
|                             CONSENSUS LAYER                                 |
|       solana core  •  subscriptions & allowances (s&a) native primitives    |
+-----------------------------------------------------------------------------+
organization repositoriesrepositoryscopestatusShugocore protocol monorepo: anchor program, @shugo-protocol/sdk, cli, landing page, and docsactive.githuborganization-level configuration, security disclosure policies, and profile metadataactivecore design principleszero custody: protocols in the shugo ecosystem never hold user funds in custodial intermediary contracts. capital resides in native solana accounts using the foundation's official subscriptions & allowances (s&a) primitives.strict deterministic enforcement: policy enforcement happens on-chain prior to instruction execution via cross-program invocation (cpi) proxies.formal verification first: program accumulators and rollover clocks are mathematically bounded and verified with the aws kani model checker to prevent integer over/underflow and re-entrancy anomalies.frictionless developer integration: agent developers can wrap existing transaction pipelines into guarded delegates with fewer than 5 lines of typescript.quick installationBash# install global developer tooling
npm i -g @shugo-protocol/cli

# or initialize directly into an agent repository
npx shugo init
security & responsible disclosurethe protocol takes a rigorous approach to cryptographic safety:all anchor programs undergo formal verification runs prior to release.to report a vulnerability or potential exploit path, review our disclosure instructions at SECURITY.md or contact security@shugo.com.shugo / 守護 / शुगो • decentralized agent security infrastructure3. Save, exit, and push:Press Ctrl+O, then Enter to save.Press Ctrl+X to exit nano.Run the commit sequence:Bashgit add profile/README.md
git commit -m "docs: initialize organization overview profile"
git push -u origin main
