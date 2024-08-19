# Introduction

We are attempting to add decred to the [Keystone](https://keyst.one/) hardware
wallet. The people over at Keystone have been very receptive to adding us. This
prop aims to add Keystone support to their hardware and Decrediton.

# Why



# QR Codes

Decrediton has support for Ledger and Trezor hardware wallets over usb. However,
the keystone wallet only gets and receives data over QR Code. This means it isn't
great for use with desktop wallets. In order to ensure the user has a camera to
read data from Keystone we are planning to add support on our side to cryptopower.

# Details

On the keystone side, dcr curently does not exist. This means we need to add it
which is half of the required work.

Along with the hardware wallet, which only signs data, we need a watching only
wallet that can watch the chain and create and send transactions. We will use
cryptopower because it can be on a mobile device which has a camera and can
read data from the Keystone wallet. While crypotpower already has dcr support
of course and works with watching only wallets, it does not yet have the ability
to read qr codes. We will need to add that and a new flow for hardware wallets.

On top of that we will want a buffer for the unexpected, testing, and bug fixes.

# Work

We anticipate costs in the range of **90k USD**.

| Item                                        | How Much       | FTE Weeks |
|---------------------------------------------|---------------:|----------:|
|  Add dcr to Keystone                        | 30k            | 12        |
|  Add qr support to cryptopower              | 15k            | 6         |
|  Add hardware wallet support to cryptopower | 15k            | 6         |
|  Testing                                    | 10k            | 4         |
|  Bug fixes                                  | 10k            | 4         |
|  Discretionary                              | 10k            | 4         |
| **Total**                                   | **90k**        | 36        |
