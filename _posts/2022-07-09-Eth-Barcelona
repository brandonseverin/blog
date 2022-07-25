---
title: "ethBarcelona 2022"
description: "What happens in Barcelona stays on the blockchain."
toc: true
layout: post
categories: [notes, talks]
---

## Boostrapping an interoperable ecosystem on polkadot -  Alberto Viera
> bit.ly/MoonbeamEthBCN2022

- Polkadot: specialisation and connectivity, there are many best blockchains. You have layer zero which is a blockchain for other blockchains (parachains) - moonbeam is one of those parachains
    - connected security - when projects connect to polkadot they don’t need to worry about security. Plus all blockchains can natively interoperate without a middle man (XCM)
- Moonbeam: Ethereum compatible smart contract parachain on polkadot
- built with substrate. 
- Stack: EVM, Substrate, web3 RPC, unified accounts (Ethereum styled accounts), dev tools and integrations (chainlink, graph etc.)
- Ethereum composability - e.g. sushi, aave, curve
- Tooling dependencies needed
- Composability powered by XCM and GMP protocols
- EVM with expanded features? EVM smart contracts can access substrate features
    - staking precompile - stake tokens to help with the network stability with metals/ledger/trezor 
    - governance unchain
    - ERC20 - precompile: access MVR and GLMR as an ERC20 without the wrapping and wrapping typical with ETH and WETH
    - Batch precompile, batch EVM calls in one single transaction either atomically or not
    - XCM related precompile - liquid staking LIDO : KSM and DOT
- XCM use case - tokens locked in parachain account on origin chain, mints representation in target chain - parachain account isn’t owned by a single entity but is owned by the whole blockchain
- remote execution - trustlessly execute liquid staking
- remote EVM calls - other blockchains can call Moonbeam to do logic via XCM
    - XCM: Polkadot + Moonbeam: do enough developers know substrate. Moonbeam has added a ERC20 interface onto of substrate assets to aid developers and integrations (XC-20 colloquially known)
        - xcDOT support in metamask
- Use moonbeam 


## Managing a DAO treasury for the revolution = Jeff Crypto & Amit Nirgunarthy (internet dollar) Cult DAO

- Charlie Chaplin speech 
    - one of the first movies that he directed and was part of that had sound
- Cult.dao: the manifesto - first rule of cult
- empowers and funds those building and contributing towards our decentralisedd future
    - the guardians
        - top 50 stagers. 
        - They put forward proposals
    - the many
        - they can vote
    - fee taken which takes 0.4% on every transfer
- the treasury contract is renounced 
- Proposal is written to the blockchain
- half of projects funded are marketing/good causes
    - mental health podcast publishing a book :smile:
- Treasury is completely CULT?
- circulation is taken out of supply when cult is staked

## Clean Smart Conract Practices

controversial suggestions: 
- have meaningful name vs weird name e.g. Maker DAO
    - weird name stops copy paste
- test driven development
    - for each line of code you should have multiple tests
    - setter and getter should be separated: don’t use the return value from the setter directly use getter
- Our practises: error message:
    - short messages save barcode size eg: CH_PSCF
        - CH = ClearingHouse : contract filename
        - PSCF : price slippage check fills, the original error message
        - leave a comment above require
    - Oriinaitng from compound:
        - storages are stored within separate files
    - avoid repetitive inputs checks by adding comments
        - pros save gas and also time for reviewers
        - cons: a pitfall i the comment is out-o-date or wrong

## The penological renaissance of art - 

Beatrix Ordovás - collectors are still getting used to digital art, the wallet download and paying in crypto is a huge barrier. They don’t feel comfortable setting everything and how will they display it? Andrés Resinger, his pieces can be both digital and physical


Andrés Resinger - has worked with digital tools for 25 years. The last few years has been working on how to interact the physical with the digital. Originally started to use the computer to compose music as he was classically trained.


## Web3 security in 2022 - Jack Sanford (sherlock), Dima Bourin (Hacken), Minier Jalal (Certik) moderated by Oliver Hörr

- 1.3B dollars lost in 2021
- 2.2B dollars lost so far in 2022
- A lot of the issues are centralisation issues. Projects leave centralisation privilege access open giving super user access to projects
- some of it is code - it is up to developers to understand how to code securely and the best practises
- Bug bounties are becoming more common place
- auditors are starting to have skin in the game, other than just reputation - people are talking but no one is actually doing it yet.
- decentralised insurance - it is normal to get hacked. safe some of your personal money and the protocol’s money - still very far away from it.
- The cost of an audit far outweighs the suffering from a multi million dollar hack
- Do they check if there is a ponzi scheme inside the code or potential rug pull liquidity after deployment? - no.
    - auditors need to improve their reports by a lot
    - auditors aren’t remediators. They recommend things to be fixed. If they aren’t fixed, then it is on you.
    - audits shouldn’t be a one time thing. As long as you hand a contract then you should have another audit

### what do teams have to do to be secure
- can have an independent security team to check the impacts of the code
- coding securely
- be educated on best coding practises
- audit is the gate
- SDLC framework: secure development lifecycle. At every stage of the development lifecycle you should run the code and asses to see how it goes wrong (5-6 hours). 
- Get the team to maintain proper documentation as you build
    - also helps auditors to do a better job
- Bug bounties is a must thing for every project right now 
- can write outlier detections - i.e. the TVL should never change list this, the transfers should never change like this
    - monitor altering is the next big thing
- smart contracts should have a function that allows teams to pause operations in the event of a hack - it doesn’t go with decentralisation but it saves money. (Dima)


- decentralisation is a joke on bsc and on ethereum - there is decentralisation in the mining pools - the MEV topic isn’t properly addressed
    - the snipers were taking liquidity in cooperation mining pools
- you can have a system that schedules a pause, or have people come to a vote and pause
- people shouldn’t use user experience as an excuse for poor security.


### how does the community participate in the security question 
- having a token makes you into a public company - persuading security is important has taken the wrong route. People 
- don’t expect community will contribute quality information, even for lots of money. Don’t overestimate the power of community when it comes to security research
- Introducing KYC is another element of risk that encompasses the entire project.
- Is it important to community members that a project has a score of 60% vs 80%? There will be a time when the community pushes projects to improve their security rating but we are not there yet

### sandbox environments
- Create a sandbox for projects to test and community to test
- Wallets should have transaction simulations built in - at the moment we focus on signatures, blind signing and smart contracts calls. But it is like we are knocking on the door we see someone’s name on the door but we don’t know if they are inside or if they are a killer. :rofl:

### automatic vs manual audits
- manual audits aren’t going anywhere
- people have developed automatic tools but they still carry out manual audits alongside

### Economic attacks?
- audit reports should be improved but it can’t be done by a single company, should be done by multiple companies that specialise in different types of attacks

### where to next?
- we will fail as a community if my mum has to look at an audit report to use a decentralised bank
    - not know the network they are on
    - not know the wallet they are using
    - not know that there is a smart contract in the back

## Building full sale web3 apps - Ivan on Tech
- got into crypto in 2013
- what is full stack? onchain logic, off chain logic, UI/UX logic  (+ communication between off chain on a onchain stuff)
    - smart contracts
    - backend: nodeJS
- what is the workflow
    - create smart contract, connect to backend (user authentications, sync user activity and assets, sync contract activity), connect to frontend (write SDK and abstractions)
    -  
- Moralis workflow: sync historic and real time events from any contract and any chain
- morals business school? 80 people fully remote, talent.moralis.io

## Fix the money, fix the world - Juan (MakerDAO SES)
> Core unit facilitator at MakerDAO SES

- we’re burning our world down - we need to save our one planet
- It’s all coordination: tools, the power of narratives and money. Narratives are everywhere (religion, capitalism, football, sparartism, the vision of your dao). Money extremely important, allows us to hyper specialise (assign value, fungibility, allows for specialization)
- Money: euros, dollars, pounds? where we are living, take the local currency
    - Money is debt 1. government bonds, the treasury offers the bonds to the federal reserves etc. 
    - what is financing? - oil pharma wars by accepting these currencies we are inadvertently financing this
    - Money that aligns to your values - allow the money to work for you
- Project financing: Good company has assets future cash flows, + DAI —> 
- MetaDAOs: Maker - make MakerDAO into a credit facility at the centre. 
    - spin out metadata that suit propositions to different people e.g. dao supporting coffee farmers in latin america
- Coordination: work, workforce, capital (note that this doesn’t need to be money, could be a ticket get into a party)
    - It’s all governance design: open software, open frameworks, redundancy first
        - change the rules and not the rulers. Set up the framework so anyone can run it. 
        - redundancy first: make your system resilient, minimise single points of failure. get different groups to work on the same things. Every DAO should try and make their own work redundant. Set up the incentives such that anyone can contribute and get compensation.
    - good luck

### Why projects need their own currencies?
- french revolution: separate the church from the state
- crypto: separate the capital from the state
- when you choose a currency that is only backed by projects that you support, you don’t even need to donate. You are creating demand for those particular currencies and backing them in a very direct way. If you choose dollars or euros you are inadvertently supporting how the US governments and the European governments spend their money. 

### DAI competing with CBDCs?
- distribution channels the government basically have the largest by forcing taxing. 
- How do you create a market: you create an army, given them your coins and collect your coins from the rest as tax. 
- We need conscious decisions in how we spend our money.
- Long way to go for UX, e.g. removing private seed phrases

### DAI is tied to dollar - by using DAI I am supporting the dollar?
- DAI is pegged to the dollar as it is the most commonly used unit of account
- It only takes 24 hours to be pegged to anything else e.g. a basket of assets

## Regen Metalities,  Impact IRL - Lauren Luz (Giveth), Jori Armbruster (EthicHub) James Beck (Metamask/consensys)

- Giveth: donation framework
- ethicHub: lend DAI to farmers, earn 8% stable yield. all the coffee supplied to the event today is from their farmers. 
- consensus: been around since the beginning of ethereal

### what is a mentality?

- James: can have a pejorative sense e.g. people can box you in. Not all degens are stereotypical degens. Regen is in some way reactionary to degen. Create circular economies that don’t need to extract
- Jori: we commit ourselves to use the technology for good. Crypto atm is a confutation of TradFi mentality. You have environmental, social and economical capital.
- Lauren: mentalities are influenced by many different factors, plus they can be dynamic. What if you could seek profit by adding value.
- The technology is neutral - all technology is a site for struggle. Ethereum will be a site for region economics and the 1980s manhattan style capitalism

### what are the roadblocks for the regen meme?
- the idea is that profit is bad and is against altruism.
- we could have better public goods if things would be profitable for people.
- Giveth: when you donate to a verifiable project you get awarded GIVE tokens
    - eventually we want to turn these non-profits into DAOs
        - you could then donate or purchase their actual token

### key barrier for ethicHub?
- user experience for farmers. some of the farmers don’t even know how to read or write.
- people need to understand that your money is your superpower - where you buy things and where you invest is how you can change the world

### metamask ux
- there are so many crypto products that are english only - this is alienating. 
- of the top 25 countries, US, brazil, Philipines, Vietnam, Nigeria (monthly active users)
    - we need to serve these languages
- a16z and gemini “state of crypto” - in english and are serving Americans.
- a lot of what happens in crypto twitter, conferences etc. is insider baseball inhaling our own fumes. ecosystem of 100,000 people.

- we haven’t decided what values our state free money wants to have (state free economics) 
    - money backed by preserved forests
    - dollar based on carbon capture
    - every project doesn’t need a token but every token can have a value
    - celo is trying to back their stable coin with carbon credits.

### how can we ensure that the information/ energy flows?
> do this with this tech, do this with this tech (not even translated in local language)

- celo connect: many people from south america, africa, south east asia
- make it easy for people to access, next step: good support teams to help users.
    - make documentation and support information in different languages
    - setup bounties for documentation translation
- build things for real world users, real world assets not for crypto investors. Build bridges to the real world not other blocchians
- ethicHub has been doing it before DeFi was a thing
- there is a lotto negative sentiment in the industry - these conferences can excite people about what else is there on offer and that people are still building.
    - if people in the non-profit space think all of crypto is a scam then it undermines completely what we are trying to do
    - the community needs to highlight these regenerative projects and good actors in this space.

### frameworks that can help people understand a regen mentality?
- jedi mentality - values in a DAO. 
- when people come into the ecosystem state the values so people can become a part of the movement 
- There isn’t enough an ethic of testing assumption. 
    - crypto has taken on the move fast and break things mentality, test inprod.
    - we need an ethical framework before deploying and testing in prod
    - the more you read the better. 
        - read history of companies, history. don’t just consume crypto material 

### overlap between refi and effective alturism:
- refi is a reaction to defi

## web3 is solarpunk: reimagining public goods - Scott Moore (Gitcoin)

- cyber punk - neuromancer, dystopian high-tech low-life
- cypherpunk - advocate for widespread use for cryptography - privacy to push for social change
- solar punk - we can work together collectively to get this change. sustainable solutions - high-tech and high life

- solar punk is a new beginning
    - it is a coordination problem and  a new coordination paradigm
    - push back on nation states as a means of political coordination
    - reversing trends of increasing institutional power abstracted notions of the self and the collective
- Ostrom (commons management) - 8 core principles
    - local commons can govern resources towards their own ends
- Rochdale (cooperativism)
    - voluntary and open membership 
- escape the tragedy of the commons - relationships are complicated so coordination is complicated.
    - Dunbar’s number 
    - as we lose our sense of connection we also lose our solidarity.
- Paul Samuelson 50s - public goods
    - non-rivalrous vs rivalrous 
- public goods funding matrix
    - market failure, value to community donation/funding amount (no, maybe, yes)
    - kernel project: web3 university
- worry about the shared libraries and the shared code, the shared spaces in which we develop
- web3 is solar punk - it isn’t just a speculative casino
- Tools for progress? - have we imaged a future we want to see?
- How can projects be part of an impact network
    - Impact DAOs
> “we can choose to build a more solar punk future… web3 is solar punk”
