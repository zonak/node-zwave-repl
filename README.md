# zwave-repl

This is a small REPL script based on `node-openzwave`.

It allows us to issue command to a Z-Wave gateway. It has been tested with a _Aeon Labs Z-Stick S2_.

## Getting Started

Download the code from _GitHub_ and install the dependencies:

```javascript
npm install
```

## Usage

To run the REPL:

```javascript
node index.js
```

There are two globals available:

- **zwave** - the actual _openzwave_ instance that we use to run the commands
- **nodes** - the list of nodes available in the Z-Wave network

For example, here's how we can switch node `4` on:

```javascript
zwave.switchOn(4)
```

or get the details about the same node:

```javascript
nodes[4]
```

For more options checkout the `node-openzwave` project [here](https://github.com/jperkin/node-openzwave).

## Dependencies

This project is based on the great efforts of _Jonathan Perkin_ and his `node-openzwave` project.

## Release History

 * 2013-11-27    v0.0.1    Initial release.
