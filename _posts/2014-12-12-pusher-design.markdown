---
layout:     post
title:      "Pusher - Realtime message service"
subtitle:   "Build a realtime message service"
date:       2014-12-12 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>Components</h2>
 1. Connector (Golang)
 2. Hub (PHP)
 3. Message Queue (Beanstalkd)

 Connector <--> Redis <--> Hub

<h3>Connector</h3>
 1. Connect with token
 2. Authenticate client
 3. Update online/offline status of client into Redis

<h3>Redis</h3>
 1. Tokens (Type: string, K/V: token/uid, TTL: 12h)
 2. Users (Type: hash, K/V: uid/{online, nickname, avatar etc.}, TTL: 7d)
 3. ChannelUsers (Type: set, K/V: cid/uids, TTL: EVER)
 4. UserChannels 
 5. Connectors: 
 6. Connector Queue: (Type: list, K/V: connector_id/messages)
 7. Device bindings

<h3>Hub API</h3>
 1. Token
    * NewToken
    * RefreshToken
    * RevokeToken
 2. Push
    * ToUser
    * ToChannel
 3. Channel
    * NewChannel
    * AddMember
    * RemoveMember
    * Members
 4. Fetch Messages
    * UserMessages
    * ChannelMessages
    * UnreceivedMessage
 5. Ack
    * UserAckList: all channels subscribed
    * ChannelAck

<h3>Message Store</h3>
 1. When a message pushed to HUB, it will be stored in db
 2. 