# Asymmetric Key Generator

This simple tool can be used to generate an Ed25519 PKCS#8 and RSA key pairs (private and public key).

There's two methods to run the tool, you can either download or build from source code.

## Download
Prebuild apps can be found in [Releases](https://github.com/binance/asymmetric-key-generator/releases).

To verify the package's integrity, download both the app and the checksum file to the same directory:

```shell
-rw-r--r--@  1 john  staff   156M 18 Nov 17:02 AsymmetricKeyGenerator-0.5.0-universal.dmg
-rw-r--r--@  1 john  staff   102B 18 Nov 19:01 AsymmetricKeyGenerator-0.5.0-universal.dmg.CHECKSUM
```

Then run sha256 checksum:

```shell
sha256sum -c AsymmetricKeyGenerator-0.5.0-universal.dmg.CHECKSUM
```

If it passes the integrity check, it'll return `AsymmetricKeyGenerator-0.5.0-universal.dmg: OK`

## Build from source code

Obtain the source code locally and go through the following steps:

```javascript

// install dependencies
npm install

// start the app for development
npm start

// or package to an installable app
npm run dist

```

## How to use

1. Open the app;

2. Choose the key type; Recommend to keep the default value (`Ed25519`), then click the button `Generate Key Pair`;

3. Below on the left column is the `Private Key`, which should be stored in a secure location on your local disk (by using the `Save` button) and must never be shared with anyone;

4. The `Public Key` is visible on the right column, and can be shared with other stakeholders.
