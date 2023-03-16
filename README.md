# LightningNetwork
Useful information on some settings so that you can run your node safely


## WatchTower
To be safe running a node on Lightning Network connect this WatchTower:
##### 032b32484f7f279638c3fa58f12d4dc255b6d7cbb08bff1f843a8e4ff2b48f79ab@onj76mblkzh6mpm3nl6ojdczzoi2jvmw2as7m6eybs52gdxqumnoztad.onion:9911

first of all edit your <code> lnd.conf</code> file and set
<code> watchtower.active = 1 </code>
stop and restart your lightning node
then use lncli command to add as follow:
<code>lncli wtclient add 032b32484f7f279638c3fa58f12d4dc255b6d7cbb08bff1f843a8e4ff2b48f79ab@onj76mblkzh6mpm3nl6ojdczzoi2jvmw2as7m6eybs52gdxqumnoztad.onion:9911</code> or any other you use software to manage your node. I'll tell about them later.
