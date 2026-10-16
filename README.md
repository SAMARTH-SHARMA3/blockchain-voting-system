# Smart Voting System Using Blockchain Technology

**A decentralised voting prototype built on Ethereum, with a survey of how people react to the idea of blockchain voting.**

University of East London · BSc (Hons) Computer Science · Dissertation, May 2024 · Samarth Sharma

Supervisor: Dr. Nadeem Qazi

---

## Materials

| | |
|:--|:--|
| **Dissertation** | Available on request |
| **Presentation slides** | Available on request |

To request either, [message me on LinkedIn](https://www.linkedin.com/in/samarth-sharma-120858242/) or [email me](https://mail.google.com/mail/?view=cm&to=samarth841sharma@gmail.com&su=Voting%20dissertation%20request).

---

## The question

Traditional paper ballots and electronic voting machines share a set of problems: limited transparency, difficulty auditing results, and public doubt that votes are counted as cast. This project asks how blockchain technology can be used to build a secure and transparent voting system that addresses them.

The aim was to **design, develop and evaluate a working prototype**, backed by a literature review and a survey of potential users.

## What I did

**Research.** I reviewed how blockchains, consensus mechanisms and smart contracts work, compared centralised and decentralised architectures, and studied electronic voting and its weaknesses. I also looked at Estonia's e-voting and digital identity systems to understand how feasible digital voting is in practice.

**Build.** I developed a hybrid decentralised application (DApp):

| Layer | Technology |
|:--|:--|
| Smart contracts | Solidity on Ethereum, managed with the Truffle Suite |
| Local blockchain for testing | Ganache |
| Front end | React |
| Back end | Node.js with Express |
| Database | MongoDB through Mongoose |
| Authentication | MetaMask wallet connection (Web3) |
| Deployment | IPFS, connecting to a private Ethereum network and a RESTful API |

**Method.** I followed an Agile approach using Kanban, with tasks broken into small units on a board.

## How the prototype works

1. A visitor opens the app and connects their **MetaMask** wallet. Without a connection the app asks them to install MetaMask and reload.
2. Once connected, a menu gives access to candidate registration, voter registration and the voter list.
3. Only the **organiser** of the voting contract can create voters and candidates.
4. Voting is recorded as a transaction on the blockchain. After a vote is cast, the voter's card updates to show **"You Already Voted"**.
5. The interface is responsive, so it works on mobile.

## Survey results

I surveyed 18 respondents (mostly aged 18–25) on their views of current voting systems and of the blockchain approach.

| Question | Result |
|:--|:--|
| How well would a blockchain voting system provide a solution for you? | **83%** said extremely well (33%) or somewhat well (50%); 11% neutral; 5% not very well; 0% not well at all |
| How well do people react to this approach, on a scale of 1 to 10? | Average of **6.3** |

The survey was also used to gauge satisfaction with current systems on factors such as transparency, privacy, reliability, fraud and manipulation.

## Testing

I tested the application manually and with Chrome Developer Tools. A Lighthouse audit scored it **74** for performance, **100** for accessibility, **96** for best practices and **100** for SEO. Performance varied with connection strength and device, mainly because of the time taken to fetch and process data from external services.

## Limitations

- **Small, non-random sample.** The survey reached 18 people, mainly classmates, so it can carry bias and cannot represent voters in general.
- **Testing depth.** Testing was mostly manual. More advanced methods, such as formal analysis of the smart contract, may uncover vulnerabilities.
- **Performance.** Data retrieval was inefficient in poor network conditions, and Ethereum's transaction speed and gas fees limit scale.
- **Scope.** It is a prototype built in a limited timeframe, without access to real election data or stakeholders.

## Future work

Improving scalability and efficiency for large elections, adding more rigorous smart contract security testing, running usability studies with a wider group of voters, and comparing the approach across different governance contexts.

## Tech

`Solidity` · `Ethereum` · `Truffle` · `Ganache` · `React` · `Node.js` · `Express` · `MongoDB` · `MetaMask` · `IPFS`

## Notes

This is academic work submitted to the University of East London.
