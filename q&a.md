Question: If a node sees a text message packet from a node it hasn’t seen before, or hasn’t seen a node info packet in awhile, will it request it?
Answer: Yes, if any packet comes in from a node that isn't in the nodedb with a nodeinfo (user), we send our nodeinfo out with a want response True

Question: Does the nodeinfo ever expire?
Answer: They never expire, however we do send updates to the mesh when any property on User in NodeInfo changes and also every device.node_info_broadcast_secs. It's typically the first thing sent over the mesh after boot

Question: How much electricity does a node use?
Answer: It depends on the type of node and its configuration. RAKs (Wisblock) can idle at just under 20ma, ESP32 often uses 10x more energy.

Question: What Meshtastic clients and tools are available to use?
Answer: The main clients used to connect to Meshtastic nodes are the [Android app](https://meshtastic.org/docs/category/android-app), 
[iOS app](https://meshtastic.org/docs/category/apple-apps), and [Web client](https://meshtastic.org/docs/software/web-client). There is a [Network Management Client](https://github.com/meshtastic/network-management-client) that is under development which aims to help manage large, decentralized mesh networks. There is a Meshtastic Python package that serves as a command line interface and Meshtastic python library. More information about the Meshtastic Python package is located [here](https://meshtastic.org/docs/software/python/cli). There is also a C# / .NET 7 based command line interface for Meshtastic, click [here](https://github.com/meshtastic/c-sharp) for more information.  There are also several other [community apps](https://meshtastic.org/docs/software/community) and [integrations](https://meshtastic.org/docs/software/integrations) available.
