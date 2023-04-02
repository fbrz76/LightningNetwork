# WatchTowers

"Watchtowers" are an important component of the Lightning Network, which is a second-layer Bitcoin payment channel network. Their main purpose is to protect users from potential fraud or attacks from their channel partners.

In practice, watchtowers are services that constantly monitor users' payment channels. If a node on the network attempts to send a fraudulent transaction through a channel, the watchtower intervenes immediately, sending an emergency closure transaction to safeguard the funds of the involved users.

Watchtowers are particularly useful for users who cannot constantly monitor their payment channels, such as if they are offline for an extended period of time. In this case, the watchtower continues to monitor the channel for them and intervenes in case of any issues.

It's worth noting that the use of watchtowers is optional. Users can choose not to use them and monitor their payment channels independently. However, for anyone looking to have an extra layer of security on their Lightning Network payment channels, watchtowers are a recommended choice.

To be safe running a node on Lightning Network connect this WatchTower:

<li>Pubkey: 032b32484f7f279638c3fa58f12d4dc255b6d7cbb08bff1f843a8e4ff2b48f79ab
<li>address on clear net: x.xxx.xxx.xxx:xxxx
<li>address on Tor network: 5632omxc6qlrlxvnwkxt4ca2nfdbx332hrloyjlxg4v7ogqs4wipbeqd.onion:9911

first of all edit your <code> lnd.conf</code> file and set
<code> watchtower.active = 1 </code>
stop and restart your lightning node
then use lncli command to add as follow:
<code>lncli wtclient add 032b32484f7f279638c3fa58f12d4dc255b6d7cbb08bff1f843a8e4ff2b48f79ab@5632omxc6qlrlxvnwkxt4ca2nfdbx332hrloyjlxg4v7ogqs4wipbeqd.onion:9911</code> or any other you use software to manage your node. I'll tell about them later.
