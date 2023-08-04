# Sacraments: Technology

Thanks to the continuous growth and maturation of the crypto ecosystem, the gaming industry has found a solid place in the world of open blockchains. Cutting edge concepts such as token sales (TGE), NFTs, semi-fungible tokens, staking and layer-2 blockchain architecture all boast the potential to optimize cost efficiency and incentive distribution. A wide range of networks can provide diverse microservices governed by community standards, enabling quick, frequent and reliable delivery of large, complex applications and technology stack evolution. We are currently engaged in the process of tech stack selection for our game prototyping, with the ultimate goal of decentralizing and minimizing transaction costs.

## Architecture&#x20;

The continuous inflation of Ethereum gas fees is a contentious issue. Although Ethereum 2.0 boasts a proof-of-stake system that simplifies cryptographic work, its high volatility is still a major entry barrier for new users. Luckily, Layer-2 blockchain platforms are a great solution for game developers, as they provide gas-free platforms and NFT smart contracts. We adapt Polygon as our Layer 2 blockchain solution and may integrate other solutions in the future when we see fit.&#x20;

## Game Core&#x20;

Frontend: Unity. We have chosen Unity for our frontend game development. Although Unreal boasts better rendering, performance and scalability, its blockchain game tech stack has little to no support. Moreover, Unreal’s pricing model is 5% royalty of overall sales, which may not fit with the blockchain ecosystem. Thus, we have selected Unity, and hope that Unity can provide better multithreading solutions in the near future.

## Gaming Guild x F2P

Free trials are critical marketing components for freemium and paid games alike, yet most blockchain games presently on the market lack free trials due to the limitations of current blockchain technology. To tackle this challenge, we have partnered with a number of gaming guilds from around the world. These organizations will offer seed planets to players so that they may experience Apeiron on a trial basis. The guilds will also provide mentorship, gameplay support, and - most importantly - community! By building a strong community of partner orgs and friendly players, we not only lower the barrier to entry but also ensure we are developing a sustainable ecosystem for the long term.

## **Mix of centralized servers with Blockchain**

To give users the best game experience, we will introduce centralized server clusters to handle most of the game logic. Only assets-related logic will be on-chain.

Centralized server for&#x20;

* Game Logic Validation to avoid cheating in progression&#x20;
* Blockchain data indexing for quick filtering and sorting.&#x20;
* Planet World Generation based on NFT&#x20;
* PVP Matching&#x20;
* Galactic Arena event hosting&#x20;
* Galaxy progression

Decentralized blockchain for&#x20;

* Planet, Apostle, Relic, and Star NFTs&#x20;
* NFT Asset generation and Genes Transform like Chronomerging, Armageddon.&#x20;
* Token earnings and usage (Token recycling mechanic)&#x20;
* Galactic Arena Rewards&#x20;
* Treasury

## **Governance**

Apeiron will give players decision-making power over the flow of the greater narrative, in a fashion similar to that of Dungeons and Dragons. Voting takes place through our decentralized autonomous organization (DAO), where token owners can vote on Galaxy Progression, use of revenue from token issues, game operations, game asset allocation, and token buy-back schemes. In principle, every Apeiros Token holder can become a DAO member and vote on proposals, although membership is optional. DAO implementation will be handled by an external third party such as Snapshot.



## **Server  Architecture**

![](../../.gitbook/assets/server\_architecture-Eng.drawio.png)

1. We will adopt K8s solution to provide high availability and reliable off-chain server.&#x20;
2. Off-chain server security and integrity are as important as on-chain. We will adopt different measures including but not limited to security auditing, Intrusion detection system, VPC, firewall, and continuous backup.&#x20;
3. Different levels of testing including but not limited to unit test, integration test, load test, and stress test, will be carried out to make sure the initial launch of the game will be high quality and less bug-prone. This also applies to future game updates.&#x20;
4. Smart contracts will be kept clean and simple, with upgradable features for bug fixing and improvement. All smart contracts will be audited by Blockchain Security Audit Company.
