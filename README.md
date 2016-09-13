# RemoteDebug Core Protocol Specification
Specification for the RemoteDebug Core Protocol Specification.

## The proposal

This is a proposal to introduce a **core protocol specification** based on common and public API's that today are shared between Webkit and Chromium. These API's already are used and deployed on a broad variety of devices today, and should give new implementors (ex: Microsoft, Mozilla, Facebook) a stable set of API's as an implemetation target to reach parity, while giving existing implementors (Google, Apple) a head-start without pushing additional commitments on their shoulders, as the API's already committed to through their public and non-experimental nature.

## The API starting point

This specification contains a `protocol.json` generated by the [generate-core-protocol script](https://github.com/RemoteDebug/remotedebug-core-spec/blob/master/generate-core-protocol.js) which grabs the WebKit's iOS10 and Chrome's CDP 1.2 protocol.json files, and generated the INTERSECT as the output.

The proposal is to use the output as the starting point for this **core protocol specification**.

## Proposing new APIs and changes

We should adapt a simiar approach to how the [Service Worker specification](https://github.com/w3c/ServiceWorker) came to life, by using GitHub to manage issues, commits and revisions of the specification.

## Protocol & transport

This specification is using [JSON-RPC](http://www.jsonrpc.org/specification) as the underlaying protocol. The preferred transport mechanism is WebSockets, but the protocol specification is agnostic to this.

## Documentation

The current [`protocol.json`](https://github.com/RemoteDebug/remotedebug-core-spec/blob/master/protocol.json) file can be fetched and viewed in tools like A, B, C and D.
