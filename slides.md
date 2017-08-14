title: Backend Technology Comparison
output: slides.html
controls: false

--

# EPPSA
## Backend Technology Comparison

---

### Requirements

* open source
* can be self-hosted
* store data
* get live updates
* no/little backend configuration and code
* can be used by the frontend directly

---

### Contenders

* [MQTT](http://mqtt.org)
* [deepstream.io](http://deepstream.io)
* [Parse](http://parseplatform.org/)
* [Horizon](http://horizon.io)
* [GraphGL](http://graphql.org)

---

### MQTT Pros

* pub/sub system made for live updates
* QoS guarantees
* multiple open source server implementations
* client libraries for many languages
* open standard
* _en vogue_ due to IoT
* our experience

---

### MQTT Cons

* only rudimentary data storage using retained messages
* no support for lists or relations
* limited message order guarantees
* no transactions
* no RPC mechanism

---

### deepstream.io Pros

* "records" for data storage with live update
* "events" for simple live notifications
* support for RPCs
* clients for JS, Android, iOS, C++, PHP
* HTTP API
* supports different databases and caches

---

### deepstream.io Cons

* no C# client
* developed by a (startup) company

---

### Parse Pros

* robust data storage including queries and relations
* "live queries" support live update
* user management and authentication
* lots of client libraries (JS, Android, iOS, Unity etc.)
* updated regularly

---

### Parse Cons

* hosted service discontinued by facebook
* development might lose traction
* live queries only supported by JS, Android and iOS clients
* JS client API feels a bit dated

---

### Horizon Pros

* robust data storage including queries and relations
* "changefeeds" support live update
* user management and authentication
* JS client library with nice API

---

### Horizon Cons

* company closed down
* little community effort
* no clients for Android, iOS, C#

---

### GraphGL Pros

* more robust due to defined schema
* only a protocol
* _en vogue_

---

### GraphGL Cons

* requires a defined schema
* reference implementation is "bring-your-own-data-store"
* live updates (through subscriptions or patch) seem like a work-in-progress
* not all implementations cover the whole spec
