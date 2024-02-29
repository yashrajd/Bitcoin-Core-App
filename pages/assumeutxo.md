---
layout: default
title: 1.2 Navigation
permalink: /assumeutxo/
nav_order: 191
header: true
---

# AssumeUTXO

AssumeUTXO is a proposed mode for bootstrapping new full nodes that allows them to postpone verifying old block chain history until after the user is able to receive recent transactions.[source](https://bitcoinops.org/en/topics/assumeutxo/). This is achieved by obtaining a snapshot (file containing all the coins (UTXOs) as of a certain block height).

At present, assumeUTXO is available in Bitcoin Core 26.0 and above, but limited to signet and lacks a canonical source of snapshots.

{% include picture.html
	image = "/assets/images/onboarding-assumeutxo-load.png"
	retina = "/assets/imagesonboarding-assumeutxo-load@2x.png"
	big = "/assets/images/onboarding-assumeutxo-load.png"
	alt-text = "Desktop app's onboarding screen showing snapshot loading screen"
	width = 800
	height = 700
%}

## Learn more

[Author’s description in Core repo](https://github.com/bitcoin/bitcoin/blob/master/doc/design/assumeutxo.md)
[Bitcoin Optech topic](https://bitcoinops.org/en/topics/assumeutxo/)


## Working files

[GitHub design issue](https://github.com/BitcoinDesign/Bitcoin-Core-App/issues/79)
[Figma file](https://www.figma.com/file/W6hyzypVYuTzZZVE6zdQsW/Bitcoin-Core-App-(Old)-(Yashraj)-(assumeUTXO)?type=design&node-id=7077%3A10150&mode=design&t=PK2aA8lxTBAGu1F0-1)


## Test

### Test design prototype(s)

Check out assumeUTXO designs we're working on: [Figma prototype](https://www.figma.com/proto/W6hyzypVYuTzZZVE6zdQsW/Bitcoin-Core-App-Old-assumeUTXO?type=design&node-id=7077-10150&viewport=-2158%2C-1088%2C0.41&t=ZNMWbKlcyZhJ5vaE-0&scaling=min-zoom&starting-point-node-id=7524%3A3768&show-proto-sidebar=1).
Drop a comment in the Figma file or create issue in GitHub.


### Testing assumeUTXO functionality

**Install/prepare for testing**

a. get the snapshot file (torrent link in [GitHub issue](https://github.com/bitcoin/bitcoin/pull/27596))

b. download the right Bitcoin Core App installer from [here](https://github.com/D33r-Gee/gui-qml/actions/runs/7587665347) (this will be updated as we go along)

c. Run the installer (instructions [here]({{ '/' | relative_url }}))

d. Change network to signet (open bitcoin.conf file and add a line “signet=1” to it)

**Test assumeUTXO**

e. Enable assumeUTXO & load snapshot (go to Settings > UTXO Snapshot)

f. Report results (use table [here](https://docs.google.com/document/d/1Nqs2WUshIK_-3LRQDudsw3mpcUFXb5ndJ-8hXwXfgJ4/edit?usp=sharing))

#### Feedback we are looking for right now

- Did you install it on a phone, tablet or desktop?
- What is the device brand and model?
- Which operating system did you use? 
- Were the download instructions easy to understand?
- How was the initial installation process?