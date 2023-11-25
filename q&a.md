Question: If a node sees a text message packet from a node it hasn’t seen before, or hasn’t seen a node info packet in awhile, will it request it?
Answer: Yes, if any packet comes in from a node that isn't in the nodedb with a nodeinfo (user), we send our nodeinfo out with a want response True

Question: Does the nodeinfo ever expire?
Answer: They never expire, however we do send updates to the mesh when any property on User in NodeInfo changes and also every device.node_info_broadcast_secs. It's typically the first thing sent over the mesh after boot

Question: How much electricity does a node use?
Answer: It depends on the type of node and its configuration. RAKs (Wisblock) can idle at just under 20ma, ESP32 often uses 10x more energy.