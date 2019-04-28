
## Main Features

* Multiple wallet creation and management in-app
* Intuitive, multisignature security for personal or shared wallets
* Easy spending proposal flow for shared wallets and group payments
* [BIP32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki) Hierarchical deterministic (HD) address generation and wallet backups
* Device-based security: all private keys are stored locally, not in the cloud
* Support for Bitcoin testnet wallets
* Synchronous access across all major mobile and desktop platforms
* Payment protocol (BIP70-BIP73) support: easily-identifiable payment requests and verifiable, secure bitcoin payments
* Support for over 150 currency pricing options and unit denomination in BTC or bits
* Mnemonic (BIP39) support for wallet backups
* Paper wallet sweep support (BIP38)
* Email notifications for payments and transfers
* Push notifications (only available for ios and android versions)
* Customizable wallet naming and background colors
* Multiple languages supported


## Testing in a Browser

> **Note:** This method should only be used for development purposes. When running Mgc-Wallet in a normal browser environment, browser extensions and other malicious code might have access to internal data and private keys.

Clone the repo and open the directory:

```sh
git clone https://github.com/MagnaChain/Mgc-Wallet.git
cd Mgc-Wallet
```

Ensure you have [Node](https://nodejs.org/) installed, then install and start Mgc-Wallet:

```sh
npm run apply:copay
npm run start
```

Visit [`localhost:8100`](http://localhost:8100/) to view the app.

## Unit Tests (Karma and Jasmine)

To run the tests, run:

```
 npm run test
```

## Testing on Real Devices

It's recommended that all final testing be done on a real device – both to assess performance and to enable features that are unavailable to the emulator (e.g. a device camera).


### Public Key for Copay Binaries

Instead of importing the public key from a public server (like gnu's) you can grab it from here:

```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: SKS 1.1.5
Comment: Hostname: pgp.mit.edu

mQMuBFO8l6sRCAD+VYKPjZY7hMCKVC3KWCkcqvSXEfiqx8KIVSp4yKx1blpVHoBYfAj13Lls
XkVMujjRVZZB8tVxl3282T/1T4VNLdHy+HvulWbAmZRAJzTw8xZYkb7L9iFFVvIHk2o31Gbq
7PAvML2MKA556jd0/OjixDR8mLpdAee8la+09RHuWhOYtFJ4nyrVW0nVFApqj1R90eXMcvOj
vSEdVHEmO341RiwayadfGRRwTqlYtsIx0k64+dpGyjA0CnJJLKVKPTzyn3bQEFhrCq41XfJf
AFI928/YVb4Wmbd51wgDv01c2b/gyGXwNFW+Qxj9xIcVgK/EPMn2I5j4eBsnOZy9Gn9vAQDj
SfX26Q6nU1x7ULPjGJ/SefPkYm2swp1Gxfmn78bXFwgA/Q7/QqqARHuUtO3ZP4FgmcxxYYK8
M+/+ROKoUUPA7Hx3cG3eq86Q5Ok7ADGFTurjaOdZmuV42E54t1pKIYvAe3IJLXr06cx3Vb8L
zLtalsQsYh2IebwRTu2wvQpsSJxBoVUzwmosNWiOuIemlTpujUFmP89Wad8MsnQSRBNoK0D7
03ckYjVRJPD+qd788c9JGyTredk0gJzV2dqesMFT+EaLuNUuOktWC+jTGZ5xK9F7EXN0ZfIM
fKDLFxvCL2a9cTCJIVirn1Ur6QHDsw5PBD/U7DDZDkk9Hzl1ep3qk7PVMn/xDzz3MxKRKKd+
d7d7wZA9OE+iKoivcAPeC1yTxQgA8KEaCz2TuS1+M9A+8PzGebKJ1OazwCb+tIGWCXUeJlIh
dRV7W/kre6e4fv0UOxDJHBrIoD1vIGtHguOGSMEnFuVJFDIH2HXXr5oxJkO86RMAig+EbglT
BJbFEfdx8Ruwhw74JzetijGHYRG62u7n8o8iX6RbpTdzt/nq26fs3Ts0SLMHfP26ZVHJOjY6
2dTCrw0q20RC4i9HWHJ0g694YBPYvhp2gYks93tigHbIqB1GhpBmBauuNvXRvNs493Rn40FI
wNMtWZBcQSMch1aEm4j5njDTt4+a6c/v8W2px3u8nFacKBR5FV86WjHEg+HmNx72nvfE/PQW
HEQixfyiObQpQ29wYXkgKHZpc2l0IGNvcGF5LmlvKSA8Y29wYXlAYml0cGF5LmNvbT6IegQT
EQgAIgUCU7yXqwIbAwYLCQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQXNYAphESz6FzCQEA
wcLYPogeVLbG3ZL5Bi/Be7U4ctNgewfKEZSSmec3vBYBAIB2xXhiq5ZER1P033KFT8g5pgY2
fMbk4YsO11Yj2B2m
=tKra
-----END PGP PUBLIC KEY BLOCK-----
```

Save that text to /tmp/key, and then import it as follows:

```
gpg --import /tmp/key
```

(Thanks @pzkpfwVI and @mika-mitzahlen for this section, taken from [Gist](https://gist.github.com/matiu/61c9f529efeeba66c0e2).

## Contributing to this project

Anyone and everyone is welcome to contribute. Please take a moment to
review the [guidelines for contributing](CONTRIBUTING.md).

* [Bug reports](CONTRIBUTING.md#bugs)
* [Feature requests](CONTRIBUTING.md#features)
* [Pull requests](CONTRIBUTING.md#pull-requests)

## Support

Please see [Support requests](CONTRIBUTING.md#support)

## License

Copay is released under the MIT License.
