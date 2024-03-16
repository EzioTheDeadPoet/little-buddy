# Little Buddy

Firmware for the [PineBuds Pro](https://wiki.pine64.org/wiki/PineBuds_Pro).

> **NOTE**: currently lacking functionality found in the factory default firmware (mainly, ANC)

The following button actions are mapped:

| taps   | single bud     | left           | right       |
| ------ | -------------- | -------------- | ----------- |
| single | play/pause     | play/pause     | play/pause  |
| double | next track     | previous track | next track  |
| triple | volume up      | volume up      | volume down |
| quad   | volume down    | ---            | ---         |
| hold   | previous track | toggle anc     | toggle anc  |

## install

Flash both earbuds with

```sh
nix run 'github:hall/little-buddy#flash'
```

> **NOTE**: append `-- -h` to view command help text; if you don't want to use [nix](https://nixos.org/download.html), you can download the latest [release](https://github.com/hall/little-buddy/releases) and use [`bestool`](https://github.com/Ralim/bestool) directly

## languages

The following languages of audio alerts are currently supported:

| name      | translation | code |
| --------- | :---------- | :--- |
| عربى      | Arabic      | ar   |
| বাংলা     | Bengali     | bn   |
| Deutsch  | German      | de   |
| English   | English     | en   |
| Español   | Spanish     | es   |
| Français  | French      | fr   |
| हिंदी     | Hindi       | hi   |
| 日本      | Japanese    | ja   |
| Português | Portuguese  | pl   |
| русский   | Russian     | ru   |
| 中国人    | Chinese     | zh   |

> **NOTE**: as they are autogenerated, new languages are both easy to add and likely to have inconsistencies; feel free to open an issue in either case.

## attribution

Thus far, I've written almost none of this.
Credit goes to the original authors.

### name

The upstream tarball was named "Little Whale" so I combined that with the device name :shrug:

### others

You may also want to check out the [OpenPineBuds](https://github.com/pine64/OpenPineBuds) project which is more established (and likely by better stewards).
This project takes non-trivial inspiration from there.
