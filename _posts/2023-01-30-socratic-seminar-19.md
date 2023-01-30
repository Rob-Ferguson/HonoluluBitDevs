---
layout: post
type: socratic
title: "Socratic 19"
meetup: https://www.meetup.com/honolulu-bitdevs/events/290866266
tags: bitdevs, socratic-19, bitcoin, resource
---

# Announcements

- Respect people’s privacy
- [Chatham House rules](https://www.chathamhouse.org/about-us/chatham-house-rule)
- [Join our telegram group](https://t.me/+Uh9gbHO9EHFkZWJh)
- [Follow us on Twitter (@HonoluluBitcoin)](https://twitter.com/HonoluluBitcoin)
- [Donate sats](http://honolulubitdevs.com/donate)
- [8Bit's BTC Jobs board launched](http://btc.jobs/)
- [Self-custody workshop next month](https://www.honolulubitdevs.com/2023-02-16-workshop-self-custody)
- Coinkite giveaway reminder
- Sponsor shoutout
	- Hawaii Technology Development Corporation
	- Entrepreneurs Sandbox

# Geopolitics

- [EU lawmakers vote to impose strict capital requirements on banks holding bitcoin and crypto](https://bitcoinmagazine.com/legal/eu-capital-requirements-banks-holding-crypto)
	- European Union lawmakers have voted to impose strict capital requirements on banks that hold cryptocurrencies
	- Banks would be allowed to hold 2% of capital in bitcoin, but required to have one euro in capital for every euro in cryptocurrency held - in an effort to “prevent instability in the crypto world from spilling over into the financial system,” according to Markus Ferber, economic spokesperson for the EU parliament's European People’s Party
	- Lawmakers cite the chaos in the markets seen over the last few months as further evidence that such regulation is necessary
	- The passed regulation mirrors that suggested by the Bank for International Settlements' Basel Committee, which also suggested the highest possible risk tier weighting for holdings of “unbacked crypto.” Their recommendations placed a 2% limit on tier 1 capital that could be held denominated in unbacked cryptocurrencies (BIS committee recommendation was discussed at last month's BitDevs)

# Market

- Where's the money, Barry?
	- [Gemini's Winklevoss writes open letter to DCG board alleging fraud](https://bitcoinmagazine.com/business/gemini-alleges-dcg-genesis-defrauded-users)
	- [SEC charges Genesis and Gemini for the unregistered offer and sale of crypto asset securities through the Gemini Earn lending program](https://www.sec.gov/news/press-release/2023-7)
	- [Genesis files for Chapter 11 bankruptcy](https://www.coindesk.com/business/2023/01/20/genesis-global-files-for-bankruptcy-protection/)
	- [Genesis already laid off 30% of staff earlier this month](https://www.wsj.com/articles/crypto-lender-genesis-lays-off-30-of-staff-11672939434)
    - Parties affected by Genesis are going to be dragged through lengthy bankruptcy proceedings in an attempt to recoup some of their losses and pay back customers
    - Contagion probably isn't over - Genesis's failure is going to bleed into DCG's other subsidiaries
    - Bitcoin that is held by custodians can be frozen and stolen
    - Besides short-term price volatility, bitcoin that is properly self-custodied in cold storage is entirely unaffected by these incidents

# Technology

- [Bitcoin Genesis block was 14 years ago on January 3, 2009](https://bitcoinmagazine.com/culture/bitcoin-genesis-block-14th-birthday-reflection)
	- 14 years ago today, Satoshi Nakamoto created the first block in the Bitcoin blockchain
	- Message engraved in the block: "Chancellor on brink of the second bailout for banks"
	- The message establishes a sort of manifesto from the start
	- Bitcoin seeks to level the playing field, ensuring property rights to millions worldwide
	- People are losing sight of Bitcoin's original purpose as they leave coins with 3rd-party custodians
	- Proof of Keys Day, also celebrated on January 3, celebrates withdrawing coins to self-custody

- [Bitcoin Core contributor Luke Dashjr loses ~200 BTC after private server compromised and warns users against upgrading Bitcoin Knots](https://unchainedpodcast.com/luke-dashjr-warns-users-about-bitcoin-knots-expiry-after-losing-3-6m-in-hack/)
	- On 1/1/2023, Luke announced his PGP key was compromised and ~200 BTC stolen
    - Luke cautioned against updating to the latest version of Bitcoin Knots signed by his key
	- Most bitcoin hardware wallet users are probably in a more secure position than Luke was for protecting their bitcoin stack

- [BIP 329 merged: standard for wallet label exports and imports between wallets](https://www.nobsbitcoin.com/bip-329-merged/)
	- BIP 329 sets a new standard for backing up various types of wallet labels and import them into other compatible wallets
	- Labels are important for tracking the history of UTXOs across transactions
	- Craig Raw, developer of Sparrow Wallet, proposed the standard

- [James O'Beirne proposes new OP_VAULT soft fork to enable simplified vault/covenant construction](https://jameso.be/vaults.pdf) 
	- [Stephan Livera Podcast #449 with James O’Beirne on OP_Vault](https://overcast.fm/+OBZmwPw60)
	- [Tales From The Crypt Podcast #388: OP_VAULT and Bitcoin Governance with James O’Beirne](https://overcast.fm/+KiHqexa6M)
	- A covenant is a constraint put on how a coin can be spent, above and beyond the traditional requirements of satisfying a one-time unlocking script (e.g., signing a transaction with a private key)
	- Vaults are an especially useful subset of covenant that gives users a time delay to recover funds spent unexpectedly
	- Jame's proposal is constructed specifically for the ideal vault design without the same drawbacks of pre-existing covenant proposals

- [Wizardsardine announces Liana self-custody solution with unique timelock-based recovery mechanisms](https://wizardsardine.com/blog/liana-announcement/)
	- Wizardsardine is a development group known for their work on Revault, an advanced and complex self-custody solution targeted toward organizations
	- Liana is a simpler, lighter self-custody solution that leverages timelocks and recovery keys
	- Timelocked recovery adds a new dimension to leverage in custody setups
	- You could previously configure authentication (who holds the keys) and space (where the keys are located) - now you can configure time (when the keys become available for use)
	- Liana is basically in beta - it's usable today, but the UX isn't prioritized in the initial version

- [Ordinal theory and the debate around "illegitimate" bitcoin transactions](https://read.pourteaux.xyz/p/illegitimate-bitcoin-transactions)
	- [Ordinal Theory Explained: Satoshi Serial Numbers and NFTs on Bitcoin](https://youtu.be/rSS0O2KQpsI)
	- [Ordinals Workshop with Casey Rodarmor](https://youtu.be/MC_haVa6N3I)
	- [Ordinal Theory Handbook](https://docs.ordinals.com/introduction.html)
	- Ordinal theory is the concept of assigning unique, numeric "identities" to individual satoshis and allowing them to be tracked, transferred, and imbued with meaning
	- Arbitrary assets, such as NFTs, security tokens, accounts, or stablecoins can be attached to satoshis using ordinal numbers as stable identifiers
	- Ordinal theory doesn't require a side chain, a separate token, or any changes to Bitcoin
	- Ordinals has resurfaced a debate around what constitutes a "legitimate" use of bitcoin - i.e., should bitcoin be used solely for financial transactions or also for immutable data storage?

# Mining

- [Luxor releases "Hashrate Index 2022 Bitcoin Mining Year in Review"](https://hashrateindex.com/blog/hashrate-index-2022-bitcoin-mining-year-in-review/)
	- 2021 bull market brought a lot of capital into the bitcoin mining industry, which became increasingly institutionalized and intertwined with traditional finance and energy sectors
	- 2022's bear market hit hard - most mining profits gained in the bull market were lost
    - Hashprice hit an all-time low in November
    - New-gen ASICs exited the year at all-time low valuations
    - Many Bitcoin mining stocks fell more than 90%
    - North America's leading hosting providers went bankrupt
    - Acquisitions and asset sales became a prevailing theme 
	- Even with last year's market carnage, Bitcoin’s hashrate grew 41% in 2022 (compared to 2021’s 18% growth)

# Coinkite Giveaway #3

- ["Guess the Nonce" Google Form](https://forms.gle/RmnDxskivwRbnVWy9)
	- Submit guesses ahead of time (only if you plan on attending the meetup)!
	- A specific block will be chosen at the meetup and its nonce will be compared to all submissions - closest guess wins
	- Previous winners are ineligible
	- [Video explaining what a nonce is in relation to bitcoin mining](https://youtu.be/6MgJCGb01jI?t=190)
		- A "nonce" is a "number used only once".
		- Miners are continuously hashing block data when trying to "win" the block lottery. The nonce is an extra field that can be repeatedly modified to produce entirely new hashes without changing the actual transaction data in the block.
		- Miners keep changing the nonce to generate new hashes, ultimately trying to get close enough to the difficulty target.

# Optional Topics

- [CoinCorner releases Bitcoin Best Bits 2022 recap](https://blog.coincorner.com/bitcoin-best-bits-2022-b6059bc928ee)
- Sam Bankman-Fried moves back in with parents
	- [Two FTX executives plead guilty to criminal charges. SBF released on $250M bond and confined to parents' home in California](https://www.nobsbitcoin.com/ftx-founder-sbf-released-on-250m-bond-at-u-s-court-appearance/)
	- [SBF's '$250M bond' incredibly overstated: no money paid, parents' ~$4M house only collateral posted](https://www.nobsbitcoin.com/sbf-bond-overstated/)
	- [Nearly $700M worth of assets linked to SBF & FTX seized by US](https://decrypt.co/119695/feds-seize-about-700m-ftx-sam-bankman-fried-assets)
- [Major bitcoin banking partner 'Silvergate Bank' lost over $700M liquidating debt to cover $8.1B in withdrawals amid bank run](https://www.nobsbitcoin.com/silvergate-bank-bank-run/)
- [El Salvador passes Digital Asset Issuance legislation](https://blog.bitfinex.com/announcements/el-salvadors-historic-digital-asset-securities-law-passes/)
- [Brazilian president signs bill regulating use of bitcoin as payment](https://bitcoinmagazine.com/legal/brazil-enacts-bitcoin-payments-bill)
- [The Kazakhstan mining exodus has flipped bitcoin to clean-energy dominance](https://bitcoinmagazine.com/business/leaving-kazakhstan-bitcoin-mostly-green)
- [Bitcoin miner Core Scientific files for bankruptcy](https://bitcoinmagazine.com/legal/bitcoin-miner-core-scientific-bankruptcy)
- [DOJ shuts down Bitzlato crypto exchange and arrests CEO for facilitating money laundering/criminal activity](https://bitcoinmagazine.com/legal/doj-shuts-down-bitzlato-crypto-exchange)
- [Texan bitcoiners are losing access to Prime Trust-backed services at the end of January due to licensing issues](https://www.nobsbitcoin.com/prime-trust-texas-issues/)
- [New Hampshire commission recommends statewide bitcoin mining energy plan](https://bitcoinmagazine.com/legal/new-hampshire-commission-recommends-bitcoin-mining)
- [Congo’s most famous national park starts mining bitcoin to bring in revenue](https://www.technologyreview.com/2023/01/13/1066820/cryptocurrency-bitcoin-mining-congo-virunga-national-park/)
- [Blockstream raises $125M to expand mining operations](https://www.prweb.com/releases/2023/1/prweb19127332.htm)
- [Strike announces 90-day trial period for Clover point-of-sale system lightning integration](https://bitcoinmagazine.com/business/clover-integrates-bitcoin-lightning-with-strike)
- [Fold launches enterprise API to enable businesses to offer bitcoin reward and card programs](https://foldapp.com/api)
- [Anthony Towns announced a new version of Bitcoin Inquisition](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-December/021275.html)
- ["Swap-in-Potentiam" proposal: non-interactive lightning channel open commitments](https://bitcoinops.org/en/newsletters/2023/01/11/#non-interactive-ln-channel-open-commitments)
- [Integrating statechains with lightning channels can allow for off-chain balancing and improved flexibility](https://bitcoinmagazine.com/technical/statechain-lightning-combined-in-bitcoin)
- [Coinbase pays $50M to NY government and promises to surveil users more](https://www.nobsbitcoin.com/coinbase-pays-50m-to-ny-gov/)
- [Coincorner partners with pouch to bring instant remittance payments to the Philippines utilizing bitcoin's lightning network](https://bitcoinmagazine.com/business/coincorner-pouch-bring-send-globally-to-philippines)
- [Bitcoiners are flocking to Nostr, but what makes it different?](https://bitcoinmagazine.com/technical/what-makes-nostr-a-different-social-platform)
- [LastPass customer vault data stolen in cloud storage breach - data vulnerable to master password bruteforce](https://www.nobsbitcoin.com/lastpass-hacked-sensitive-data-stolen/)