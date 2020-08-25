# .crypto

Crypto Registry Naming Service (CNS) is a naming service implemented using Ethereum Smart Contract Platform.
Each name inside CNS has a format of a domain name in `.crypto` top level domain space. Like `example.crypto`.

CNS's goal is to be an alternative to classical domain names system (DNS) by fixing its core downsides:

* Censorship Resistance
* Ensure permanent ownership of the domain by the owner
* Decentralized registration
* Decentralized access

## Documentation:

### Pre-requirements

.crypto domain names registry is based on the following technologies:

Required to resolve a domain:

* [JSON](https://www.json.org/json-en.html) - standard data interchange format in web
* [SHA-3](https://en.wikipedia.org/wiki/SHA-3) - modern secure cryptographic hashing algorithm
* [Solidity ABI](https://solidity.readthedocs.io/en/v0.6.11/abi-spec.html) - function call parameters encoding/decoding algorithm
* [Ethereum JSON RPC](https://eth.wiki/json-rpc/API) - access Ethereum blockchain data via JSON RPC interface

Additionally required to manage domain records, transfer domains to other owner address and configure management permission:

* [EIP-721](https://eips.ethereum.org/EIPS/eip-721) - ERC-721 Non-Fungible Token Standard
* [Ethereum Transactions](https://docs.ethhub.io/using-ethereum/transactions/) - executing blockchain transactions

A person reading the documentation is expected to understand the basics of those standards.

### Pages 

* [Architecture](./ARCHITECTURE.md) - detailed overview on CNS design
* [Browser Resolution](./BROWSER_RESOLUTION_HOWTO.md) - Resolving CNS domain in a browser how-to
* [Contributor's Guide](./DEVELOPMENT.md) - Contributor's guide on smart contract source code development and deployment
* [Records Reference](./RECORDS_REFERENCE.md) - A table of all possible records that can be set for CNS domains

## Resolution libraries

Available domain resolution libraries to retrieve crypto registry data:

* [resolution.js](https://github.com/unstoppabledomains/resolution)
* [resolution-swift](https://github.com/unstoppabledomains/resolution-swift)
* [resolution-java](https://github.com/unstoppabledomains/resolution-java)

These libraries are only set to read data from crypto registry making them lightweight and fit for most application that do not require domain management compatibilities.


<div id="deployed-contracts"></div>

## Deployed Smart Contracts addresses

### Mainnet

| Contract Source                                              | Ethereum Addresses                         |
|--------------------------------------------------------------|--------------------------------------------|
| [Registry](./contract/Registry.sol)                          | [0xD1E5b0FF1287aA9f9A268759062E4Ab08b9Dacbe](https://etherscan.io/address/0xD1E5b0FF1287aA9f9A268759062E4Ab08b9Dacbe) |
| [SignatureController](./contracts/SignatureController.sol)   | [0x82EF94294C95aD0930055f31e53A34509227c5f7](https://etherscan.io/address/0x82EF94294C95aD0930055f31e53A34509227c5f7) |
| [MintingController](./contracts/MintingController.sol)       | [0xb0EE56339C3253361730F50c08d3d7817ecD60Ca](https://etherscan.io/address/0xb0EE56339C3253361730F50c08d3d7817ecD60Ca) |
| [WhitelistedMinter](./contracts/WhitelistedMinter.sol)       | [0xB485D89aBA096Fc9F117fA28B80dC8AAC7971049](https://etherscan.io/address/0xB485D89aBA096Fc9F117fA28B80dC8AAC7971049) |
| [URIPrefixController](./contracts/URIPrefixController.sol)   | [0x09B091492759737C03da9dB7eDF1CD6BCC3A9d91](https://etherscan.io/address/0x09B091492759737C03da9dB7eDF1CD6BCC3A9d91) |
| [DomainZoneController](./contracts/DomainZoneController.sol) | [0xeA70777e28E00E81f58b8921fC47F78B8a72eFE7](https://etherscan.io/address/0xeA70777e28E00E81f58b8921fC47F78B8a72eFE7) |
| [Resolver](./contracts/Resolver.sol)                         | [0xb66DcE2DA6afAAa98F2013446dBCB0f4B0ab2842](https://etherscan.io/address/0xb66DcE2DA6afAAa98F2013446dBCB0f4B0ab2842) |
| Resolver **(legacy)**                                        | [0xa1cac442be6673c49f8e74ffc7c4fd746f3cbd0d](https://etherscan.io/address/0xa1cac442be6673c49f8e74ffc7c4fd746f3cbd0d) <br>[0x878bc2f3f717766ab69c0a5f9a6144931e61aed3](https://etherscan.io/address/0x878bc2f3f717766ab69c0a5f9a6144931e61aed3) |
| [ProxyReader](./contracts/ProxyReader.sol)                   |[0x7ea9Ee21077F84339eDa9C80048ec6db678642B1](https://etherscan.io/address/0x7ea9Ee21077F84339eDa9C80048ec6db678642B1) |