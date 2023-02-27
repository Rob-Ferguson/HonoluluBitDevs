---
layout: post
type: socratic
title: "Socratic 20"
meetup: https://www.meetup.com/honolulu-bitdevs/events/291647400/
tags: bitdevs, socratic-20, bitcoin, resource
---

# Announcements

- Respect people’s privacy
- [Chatham House rules](https://www.chathamhouse.org/about-us/chatham-house-rule)
- [Join our telegram group](https://t.me/+Uh9gbHO9EHFkZWJh)
- [Follow us on Twitter (@HonoluluBitcoin)](https://twitter.com/HonoluluBitcoin)
- [Donate sats](http://honolulubitdevs.com/donate)
- Sponsor shoutout
	- Hawaii Technology Development Corporation
	- Entrepreneurs Sandbox

# Geopolitics/Market

- [Mississippi & Missouri lawmakers introduce bills to protect the rights to mine bitcoin and run a node](https://bitcoinmagazine.com/legal/mississippi-missouri-bills-to-protect-bitcoin)
	- Lawmakers from the U.S. states of Mississippi and Missouri have introduced bills that seek to legally protect their citizens’ rights to run a Bitcoin node and to mine BTC
	- The bills also have language prohibiting:
		- Political subdivisions of the state creating requirements which are not in line with other data center requirements, and changing the zoning of bitcoin miners without proper notice
		- Outlawing of discriminatory energy rates directed at bitcoin miners
		- Sound ordinances directed at mining facilities that are not in-line with other sound ordinances within the community
		- Operating nodes or miners being considered the act of money transmitting

- [Wyoming legislature passes bill protecting bitcoin private keys from courts](https://bitcoinmagazine.com/legal/wyoming-legislature-bill-protecting-private-keys)
	- The U.S. state of Wyoming has passed a bill that protects its citizens from having to disclose their private keys
	- The bill states that “No person shall be compelled to produce a private key or make a private key known to any other person in any civil, criminal, administrative, legislative or other proceeding in this state that relates to a digital asset, digital identity or other interest or right to which the private key provides access unless a public key is unavailable or unable to disclose the requisite information with respect to the digital asset, digital identity or other interest or right.”
	- The bill has been approved by the state Senate and House of Representatives and now needs to be signed by the Governor in order to take effect

- [Kraken to discontinue unregistered offer and sale of crypto asset staking-as-a-service program and pay $30 million to settle SEC charges](https://www.sec.gov/news/press-release/2023-25)
	- The SEC has charged Kraken with failing to register the offer and sale of their crypto asset staking-as-a-service program
	- The program allowed investors to transfer crypto assets to Kraken for staking in exchange for advertised annual investment returns
	- The SEC's complaint also alleges that Kraken claimed its staking investment program offered easy-to-use benefits and strategies to obtain regular investment returns, but provided investors with zero insight into its financial condition, among other things
	- SEC Chair Gary Gensler commented, "Today’s action should make clear to the marketplace that staking-as-a-service providers must register and provide full, fair, and truthful disclosure and investor protection."

# Technology

- [Coinkite launches preorders for new bitcoin hardware wallet COLDCARD Q1](https://bitcoinmagazine.com/business/coinkite-new-bitcoin-wallet-coldcard-q1)
	- Coinkite is launching a higher-end, battery-powered COLDCARD, featuring a full QWERTY keyboard, a larger LCD screen, 2 microSD card slots, and a QR code scanner
	- It borrows some core features included in the Mk4: same secure element setup, NFC compatibility, USB virtual disk mode, USB-C connector, etc.
	- The new COLDCARD Q1 is available for pre-sale at $199 with a planned release in Q4 2023

- [Breez's new SDK enables non-custodial "Lightning as a Service" integration for developers](https://medium.com/breez-technology/lightning-for-everyone-in-any-app-lightning-as-a-service-via-the-breez-sdk-41d899057a1d)
	- The open-source Breez SDK enables developers to integrate Lightning and bitcoin payments into their apps with zero learning curve or technical expertise.
	- It’s an end-to-end, non-custodial, drop-in solution powered by [Blockstream's Greenlight](https://blockstream.com/lightning/greenlight/), including a built-in LSP, on-chain interoperability, fiat on-ramps, and other services users and operators need.
	- Key benefits:
		- It's end-to-end: no assembly required
			- Developers can delegate a lot of complexity back to Breez
			- Developers need to add a few abstracted API calls to their apps, and Breez handles all node creation, channel management, etc.
		- It's trustless: no custody
			- All peers maintain custody of their own money at all times
			- Breez SDK users get provisioned their own nodes on-demand via Greenlight
			- Users maintain control of private keys and authorize apps to access the Greenlight node when money needs to move
		- It's frictionless: no KYC/AML
			- Breez SDK enables P2P payments, so developers never have to touch the users' money directly
			- No KYC/AML, money transmitter licenses, or 3rd-party fiat payment processors required
		- It's interoperable: no wallets
			- Users see one balance accessible from any app on any device
			- Various services can be separately authorized to tap into the same Greenlight node
		- It's global: no borders
			- Non-custodial lightning wallets circumvent the regulatory hurdles associated with different geopolitical jurisdictions

- [Voltage announces Flow 2.0: A new LSP focused on just-in-time liquidity](https://voltage.cloud/blog/voltage-announcements/introducing-flow-v2/)
	- The initial version of Flow was released over a year ago and was created as an easy way to purchase persistent channels of a given size to help users get inbound (and outbound) capacity
	- Flow 2.0 is an upgrade to provide liquidity at the exact moment it is needed - a receiver can have zero liquidity and still receive payment via Voltage’s liquidity
	- Flow 2.0 is a noncustodial way to easily receive Lightning payments without thinking about channels
	- By leveraging zero-confirmation channels and preimage hashes, they can determine on the fly if a new channel is required, open it instantly if necessary, and send the payment to the receiver without ever taking custody of funds

- [Strike's API is now publicly available: Businesses and developers can easily use the lightning network for payments](https://www.nobsbitcoin.com/strike-launches-sending-api/)
	- Strike's Sending API documentation is now public
	- Users can leverage the API to send USD payments over lightning network rails
	- No stablecoins - lightning network is used to move value, which is automatically converted to USD on either end
	- "No need to own/spend bitcoin, stomach volatility, encounter taxable events, handle added accounting, or take on any legal/compliance headaches"
	- List of [example applications](https://docs.strike.me/walkthrough/example-apps/) in the documentation

- [BlueWallet is sunsetting LNDhub.io and is no longer supporting custodial Lightning wallets](https://bluewallet.io/sunsetting-lndhub/)
	- Lightning wallets in BlueWallet have historically been custodial by default, leveraging their own [LNDhub](https://bluewallet.io/lndhub/) instance to provide separate accounts for individual BlueWallet users
	- BlueWallet is shutting down their LNDhub instance on April 30th, meaning any users that have sats on BlueWallet's lightning node need to move their funds to a different wallet before that deadline
	- In the interim, BlueWallet LN users can still withdraw sats, but creating new or refilling existing lightning wallets on the LNDHub node is no longer possible
	- LNDHub itself is still a [FOSS project](https://github.com/BlueWallet/LndHub) and users can continue to spin up their own instance as a self-hosted solution
	- BlueWallet users will always be able to connect to their own LNDHub from BlueWallet or other software that supports the LNDHub API spec (i.e., self-hosted LNDHub users are unaffected by this news)
	- A few good alternatives: [Muun](https://muun.com/), [Breez](https://breez.technology/), [Phoenix](https://phoenix.acinq.co/), [Zeus](https://zeusln.app/)

# Mining

- [Fedipool: Fedimint could mitigate bitcoin mining pool concerns](https://www.discreetlog.com/fedipool/)
	- More discussion on [pros and cons](https://github.com/fedimint/fedimint/discussions/1504)
	- The overwhelming majority of bitcoin mining relies on mining pools
	- Mining pool operators custody bitcoin for their users and choose which transactions are included in the blocks they mine
	- Fedimint is an emerging open source protocol that combines bitcoin, lightning, chaumian ecash, and federated custodians (called Guardians) to create community wallets that are easy to use, have strong privacy, reduced custodial risk, cheap and fast payments within the community, and interoperability with all bitcoin wallets
	- The same tech could be used to replace major custodial mining pools:
		- A group of independent miners can choose to create a Fedimint together
		- Rather than a single pool operator constructing blocks and choosing which transactions to include, each Guardian can construct their own blocks, reducing censorship risk
		- Additional miners can join the pool in the future to take advantage of the above, but rather than be a Guardian, they choose which Guardian they want to construct their blocks
	- Key benefits:
		- Rewards can't be seized if at least two miners act honestly
		- Miners receive the privacy benefit of chaumian ecash
		- Miners can withdraw mining rewards using bitcoin or lightning at their leisure
		- Regulatory risk is significantly reduced since Guardians can be easily located in different jurisdictions throughout the world

- [Many ~4MB blocks mined this month as Ordinal inscriptions approach 200k milestone](https://blockchair.com/bitcoin/blocks?s=size(desc)#)
	- Fees have been low enough that inscriptions are relatively economical 
	- It's yet to be seen whether inscriptions will maintain popularity over time, especially as fees go up
	- Still a lot of debate on whether or not inscriptions are a good use of block space, but most have accepted that they're inevitable either way

# Optional Topics

- [Bitcoin Core maintainer Marco Falke steps down](https://www.nobsbitcoin.com/marco-falke-steps-down/)
- [James O'Beirne writes formal BIP for OP_VAULT](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2023-February/021465.html)
- [Codex32: Proposed BIP for offline seed-splitting and recovery scheme](https://bitcoinops.org/en/newsletters/2023/02/22/#proposed-bip-for-codex32-seed-encoding-scheme)
- [Handcrank: A drivechain wannabe with no softfork](https://github.com/supertestnet/handcrank)
- [Flyover: A repayment protocol for fast bitcoin transfers over federated pegs](https://eprint.iacr.org/2023/086)
- [Maravedí: A secure and practical protocol to trade risk for instantaneous finality](https://eprint.iacr.org/2023/183)
- [Fedimint hackathon winners announced](https://www.fedi.xyz/blog/fedimint-hackaton-winners)
- [How many bitcoin confirmations is enough?](https://blog.lopp.net/how-many-bitcoin-confirmations-is-enough/)
- [Ordisrespector is a mempool filter that rejects ordinal transactions](https://minibolt.info/guide/bonus/bitcoin/ordisrespector.html)
- [Muun wallet submarine swaps are quickly expanding the UTXO set](https://twitter.com/mononautical/status/1621663167582437376?s=20)
- [Should we remove the OP_RETURN size limit?](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2023-February/021438.html)
- [Jeremy Rubin steps away from development on bitcoin-related projects](https://twitter.com/JeremyRubin/status/1618806141903069184)
- [Bitcoin + Nostr could redefine social media](https://bitcoinmagazine.com/culture/nostr-and-bitcoin-can-change-social-media)
- [Bitcoin Search: A search engine for bitcoin technical documentation and discussions](https://bitcoinsearch.xyz)
- [Proposal for a serverless version of the BIP78 payjoin protocol](https://bitcoinops.org/en/newsletters/2023/02/01/#serverless-payjoin-proposal)
- [U.K. details plan to regulate bitcoin/cryptocurrency industry](https://bitcoinmagazine.com/legal/u-k-details-plan-to-regulate-bitcoin)
- [UK court rules Craig Wright has no copyright claim on bitcoin](https://bitcoinmagazine.com/legal/court-rules-craig-wright-has-no-bitcoin-copyright)