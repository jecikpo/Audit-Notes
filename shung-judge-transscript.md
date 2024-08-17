# Shung's judging conversation transscript

The link to the original tweet [Good Luck to the Judge](https://x.com/shunduquar/status/1824480593331015839)

*Edgeworth*: A malicious user can leverage create2 hash collision to steal funds from the contract. They can generate an EOA create2 pair with the same address. After deploying the contract and attracting funds they can use the EOA to rug it.

[Objection!]

*Karma*: An Ethereum address collusion? You need 2**160 effort for that...

[Hold It!]

*Edgeworth*: Due to birthday paradox it is actually more like 2**80 effort. If you ask 23 people their birthday there is 50-50 chance 2 of them has the same birthday.

[Objection!]

*Godot*: What is this nonsene! You cannot make a transaction from an EOA after deploying the contract. Per EIP-3607, transaction from senders with deployed code are rejected at node level.

[Hold It!]

*Mia*: You can instead pre-approve the tokens first with EOA, then deploy the contract, which would inherit the approvals.

[Objection!]

*Godot*: That still doesn't work! You need to study your EIPs. Per EIP-684, you cannot deploy a contract to an account with existing nonce.

[Hold It!]

*Mia*: You can instead deploy an attack contract to do the approvals. Then the contract can selfdestruct. Selfdestructing resets the account nonce, therefore the subsequent create2 deployment will not fail.

*Godot*: Selfdestruct is deprecated.

[Objection!]

*Mia*: You can still selfdestruct during initialization. It is in EIP-6780. Didn't you read your EIPs?

[Hold It!]

*Karma*: Even if that's all possible how are you supposed to check for collisions in 2**80 hashes? You need 100 million exabytes of storage to have a lookup table to check for those collisions.

[Hold It!]

*Edgeworth*: There are various cycle detection algorithms for th--

[Objection!]

*Godot*: What about the cost? Per EIP-3607, you need 10 billion USD to find a collision!

[Take that!]

*Karma*: Exactly! ecmul is a very expensive operation you need to generate addresses.

[Hold It!]

*Mia*: You don't need ecmul to generate addresses. You can generate public keys by adding the generator point to the previous public key. So you only need ecadd. Also we don't need any EOAs!!! Did you forget it old man? We can generate all addressess using create2.

[Hold It!]

*Karma*: But it shouldn't be possible. Even mining contract addresses with / leading zero bytes costs $5000 USD.

[Objection!]

*Edgeworth*: This blog post I found on the internet says it would just cost $1,6 million USD. Bitcoin is already operating at 2**84 hashes a day if we just direct the hashing power of Bitcoin for one day we can find a collision.

[Objection!]

*Godot*: Oh yeah? And if all of humanity came together we can achieve world peace. You are not going to make entire Bitcoin network start looking for create2 collisions just for you.

[Hold It!]

*Edgeworth*: The attacker can instead invest itw own ASICs to reduce the cost of the attack.

[Hold It!]

*Karma*: And what's the hardware cost of that?

*Mia*: According to Moore's law it will cost less than a dollar by 2060!

[Objection!]

*Godot*: A hypothetical exploit that hinges on predicting the future development of the semiconductor industry! You don't actually believe this is a Medium severity, you just want the payment!!

*Mia*: This is a genuine finding, the client even fixed it per the recommendation!

*Karma*: You can't even name which cycle detection algorithm can be used!

*Edgeworth*: It is Pollard's rho algorithm!

*Godot*: Then demonstrate it for a 10 bytes collision, I dare you!

*Mia*: AAAAAAAAA

*Karma*: AAAHAHAAAAAAAA

*Edgeworth*: AAAAAAAAAAAAAAAAA

*Godot*: AAAAAAAAAAAAAAA
