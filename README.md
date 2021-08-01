# MONCoin®: Checkpoints IPFS Helper

This project is designed to make it very easy to help with the distribution of MONCoin® checkpoints via [IPFS](https://ipfs.io). It is designed to run as a service with an in-built IPFS node where the latest checkpoints hash is retrieved, and locally pinned. Any old pins are removed as needed. The more people that run IPFS nodes with the checkpoints file, the faster everyone else can retrieve it.

## Prerequisites

- node >=10
- Optional Open Firewall Ports for faster IPFS discovery
  - 4001/tcp
  - 4002/tcp
  - 4003/tcp

## Install

```sh
git clone https://github.com/Kulteam/MONCoin-Checkpoints-IPFS-Helper
cd MONCoin-Checkpoints-IPFS-Helper
npm install
```

## Usage

### Starting CLI Mode

```bash
npm start
```

### Starting with PM2

```bash
pm2 start index.js --name checkpoints-ipfs
pm2 save
```

### Starting with [forever](https://www.npmjs.com/package/forever)

```bash
forever start index.js
```

## Run tests

```sh
npm test
```

## Author

👤 **Special Thanks to TurtleCoin Developers**

* Twitter: [@_turtlecoin](https://twitter.com/_turtlecoin)

## 📝 License

This project is [GPL-3.0](https://github.com/Kulteam/MONCoin-Checkpoints-IPFS-Helper/blob/master/LICENSE) licensed.
