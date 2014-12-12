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
 3. Channels (Type: set, K/V: cid/uids, TTL: EVER)
 4. Connectors: 
 5. Connector Queue: (Type: list, K/V: connector_id/messages )
 6. Device bindings

<h3>Test with PHP</h3>

Create PHP project with composer
`mkdir `

