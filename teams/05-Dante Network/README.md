## Project

Project Name: Dante Network

Start time: 2022.2

## Introduction

![79065cb236bd6d0a18725bd864cc36a](https://user-images.githubusercontent.com/83746881/169981478-dd274207-a0ee-48a5-bdc1-94e46f938766.png)

In this hackathon we have chosen the following tracks:
* [Category 5：cross-chain，Bridge，Layer2，Layer0](https://github.com/xiyu1984/hackathon-2022-summer/blob/main/docs/categories.md#%E7%B1%BB%E5%88%AB-5%E8%B7%A8%E9%93%BEbridgelayer2layer0)
  
  * [Layer0](https://github.com/xiyu1984/hackathon-2022-summer/blob/main/docs/categories.md#layer0)

Dante Network is the middleware of Web3 for collaboration among multiple ecosystems.  In Dante Network, we define and implement a protocol stack for Web3 to realize the interconnection and the interoperability, which will bring innovative experience for Web3, just as an "Internet protocol stack" is for the current Internet. Based on Dante protocol stack, in the future, not only token circulation among multi-chain ecosystems could be easily achieved, but comprehensive information perception and barrier-free interoperability of smart contracts will also be seamlessly feasible. 

Polkadot/Kusama pioneered the ecological paradigm of multi-chain collaboration, where various public chains with different capabilities in the ecosystem can connect and collaborate with each other. We strongly endorse this idea that web3 will be a world of diverse collaborations. The current web3 is a multi-ecological coexistence world, outside of Polkadot, some ecologies are already very famous (e.g. Ethereum, BNB, Solana, Avalanche, Near, etc.), and some have some special capabilities (e.g. Flow, Arweave, Aleo, PlatON, etc.).

Dante Network is very much in line with Polkadot/Kusama's philosophy; in short, Dante Network will help Polkadot expand the boundaries of its eco-applications. More than a cross-ecology Token bridge, Dante Network will provide a common cross-ecology message communication and smart contract invocation infrastructure. This will help users outside the Polkadot ecosystem to access services and resources within the Polkadot ecosystem in their familiar environment, while every participant in the Polkadot ecosystem can enjoy a wider range of services offered by the entire web3 world with Dante Network.

### Product
Contretely, Dante protocol stack is implemented as the following:

* Firstly, Dante protocol stack will be implemented as smart contracts deployed on multi-chains including more than one smart contract platform parachains in the Polkadot ecosystem, through which DApps' in the Polkadot ecosystem can send or receive general messages, to or from contracts deployed on chains outside(EVM chains, Near, Flow, etc.). Besides, smart contracts deployed on different chains can call each other as convenient as they did in the same chain.
* Secondly, we will build off-chain routers called "Adaption nodes" to make the underlying information routing. Anyone can participate in Dante Network by deploying an "Adaption node" with their own private key.
* Thirdly, we will provide SDKs covering multiple technology stacks for DApp developers to make multi-chain interoperations more convenient and easier. The technology stacks will include Rust (ink!, Near, Solana, etc.), Solidity (EVM chains like Ethereum, BNB, Avalanche, etc.), Cadence (Flow), etc.

### Architecture
![image](https://user-images.githubusercontent.com/83746881/174229468-cfbddd60-fb31-4477-bbd8-9f4e99ccc81e.png)

### Details
Details of our project are as below: 
* [Github Organization](https://github.com/dantenetwork)
* [Pitch deck  & white paper](https://github.com/dantenetwork/Pitch-Deck)
* [Video](https://www.youtube.com/watch?v=CYXx4O8Xgcs)

## Plan to Develop

**In Blockchain**
We will complete the most basic functions of the stack, provide a multi-ecological smart contract development SDK for dApp developers to try out, and deploy demos in the test network to demonstrate the capabilities. We will provide both the technology stack of `ink!`(support for most future substrate-based parallel chains) and `solidity` (support for parallel chains with EVM smart contract platforms).

- `Smart contracts`
  - [ ] The implementation of the Message protocol for ink!.
  - [ ] Message communication smart contracts deployed on `shibuya`(AStart Testnet), `Moonbase Alpha`(Moonbeam Testnet), Near Testnet, and some EVM chains.
  - [ ] Basic SQoS Items：Identity traceability as the default choice.
  - [ ] On-chain simulations for some of the underlying algorithms.
- `off-chain routers` 
  - [ ] Message translation between `ink`(Parachain AStar) and `solidity`(some EVM chains) technology stack
  - [ ] Message translation between `ink`(Parachain AStar) and `NEAR Rust`(NEAR) technology stack
  - [ ] Message translation between `solidity`(Parachain Moonbeam) and `NEAR Rust`技术栈间的消息编解码；
  - [ ] Message delivering.
- `Omnichain dApp SDK for Polkadot`
  - [ ] Omnichain dev SDK for `ink`(Parachain AStar) smart contract
  - [ ] Omnichain dev SDK for `solidity`(Parachain Moonbeam) smart contract
- `Demos`(Deployed on Testnet)
  - [ ] Message communication between `ink!` smart contract platform(`shibuya`) in Polkadot and Near or some EVM chains
  - [ ] Smart contracts invocation between `ink!` smart contract platform(`shibuya`) in Polkadot and Near or some EVM chains
  - [ ] Message communication between `solidity` smart contract platform(`Moonbase Alpha`) in Polkadot and Near
  - [ ] Smart contracts invocation between `solidity!` smart contract platform(`shibuya`) in Polkadot and Near or some EVM chains

## Achievement in hackathon

- 6月22日前，在本栏列出黑客松期间最终完成的功能点。
- 把相关代码放在 `src` 目录里，并在本栏列出在黑客松期间打完成的开发工作/功能点。我们将对这些目录/档案作重点技术评审。
- 放一段不长于 **5 分钟** 的产品 DEMO 展示视频, 命名为 `团队目录/docs/demo.mp4`。初审时这视频是可选，demo day 这是计分项。

## Technology Team
Jason(CEO)
* Master degree. Major in software enginering
* Over 10 years of working experience; senior practitioner in blockchain/information security
* Responsible for participating in a number of national information security research projects
* Head of node service provider
* Experienced in operating nodes of many large projects
* Rich experience in blockchain project incubating and operation
* Mail: chengjingxx@gmail.com

Shawn Z (Tech leader)
* Master degree. Major in Information Security
* Expert in privacy computing, blockchain, and artificial intelligence
* Responsible for or participated in a number of national information security research projects
* Worked for a State-owned enterprise (Fortune 500) engaged in the security business for 10+ years
* Full-stack engineer in information security, AI, blockchain, etc
* Hackathon winner as a team tech leader: [Near MetaBuild Hackathon](https://devpost.com/software/universal-trusted-cross-chain-bridge ), [PlatON Dorahacks](https://forum.latticex.foundation/t/topic/5676 )
* [Github](https://github.com/xiyu1984) 
* Mail: xiyuzheng1984@gmail.com

Zack W (Full-stack Dev in web3, core dev in Dante Network)
* Master degree. Major in Computer Science & PM
* EOS, PlatON technical community senior participant (output around 40 technical articles, help EOS and PlatON fix many bugs).
* Technical mentor for EOS 1st Hong Kong Hackathon Live.
* Technical leader of EOS Genesis node ‘eosiomeetone’ which was the largest node in Asia in terms of traffic when the main network was launched, with QPS 8k+.
* Senior full-stack engineer (worked in Qunar, Snowball).
* [Github](https://github.com/wuyahuang).
* [Technical articles](https://github.com/meet-one/documentation) .

George H (Full-stack Dev in web3, core dev in Dante Network)
* Major in Software Engineering
* Senior participant of PlatON technical community ported Chainlink project for PlatON and exported several technical articles.
* Built and maintained Polkadot, Kusama, PlatON, Ethereum2.0, ChainX, and other project nodes
* Crust, Phala project node data center leader, responsible for project operations and maintenance, and the development of operations and maintenance-related tools.
* 10 years as a full-stack engineer in finance, games, education, etc.
* [Github](https://github.com/virgil2019) .
* Mail: hht2015ily@gmail.com

Kay L (Full-stack Dev in web3, core dev in Dante Network)
* Major in Software Engineering
* Development of a State-owned enterprise medical alliance chain, as well as the construction and maintenance of a distributed storage network and related SDK.
* Years of blockchain experience, an active participant in EOS, PlatON, and other communities, publishing technical articles and fixing bugs.
* Participate in EOS node maintenance, and EOS DAPP development.
* [GitHub](https://github.com/kay404) .
* Mail: kay20475@gmail.com

James F (Full-stack Dev in web3, core dev in Dante Network)
* Major in Computer Science
* Over 10 years of working experience in various aspects of computer programming, analysis, development, and testing.
* EOS, Fluence, Nervos technical community participant.
* Full-stack engineer (worked in Go/Rust/C++/Javascript)
* Hackathon winner: [FluenceLabs gitcoin hackathon](https://gitcoin.co/issue/fluencelabs/sovereign-data-hackathon/1/100026738 ), [nervos gitcoin hackathon](https://www.nervos.org/blog/nervos-gitcoin-hackathon-winners-announced ).
* [Github](https://github.com/fsy412) 
