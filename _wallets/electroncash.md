---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

id: electroncash
title: "Electron Cash"
titleshort: "Electron Cash"
compat: "desktop windows mac linux mobile android"
level: 2
platform:
  - desktop:
    name: desktop
    default: &DEFAULT
      text: "walletelectroncash"
      link: "https://electroncash.org"
      source: "https://github.com/Electron-Cash/Electron-Cash"
      screenshot: "electrum.png"
      check:
        control: "checkgoodcontrolfull"
        validation: "checkpassvalidationspvservers"
        transparency: "checkpasstransparencyopensource"
        environment: "checkpassenvironmenttwofactor"
        privacy: "checkpassprivacybasic"
        fees: "checkgoodfeecontrolfull"
      privacycheck:
        privacyaddressreuse: "checkpassprivacyaddressrotation"
        privacydisclosure: "checkfailprivacydisclosurecentralized"
        privacynetwork: "checkpassprivacynetworksupporttorproxy"
    os:
      - name: windows
        <<: *DEFAULT
      - name: mac
        <<: *DEFAULT
      - name: linux
        <<: *DEFAULT
  - mobile:
    name: mobile
    os:
      - name: android
        text: "walletelectroncash"
        link: "https://play.google.com/store/apps/details?id=org.electroncash.wallet"
        source: "https://github.com/Electron-Cash/Electron-Cash"
        screenshot: "electrumandroid.png"
        check:
          control: "checkgoodcontrolfull"
          validation: "checkpassvalidationspvservers"
          transparency: "checkpasstransparencyopensource"
          environment: "checkpassenvironmentmobile"
          privacy: "checkpassprivacybasic"
          fees: "checkgoodfeecontrolfull"
        privacycheck:
          privacyaddressreuse: "checkpassprivacyaddressrotation"
          privacydisclosure: "checkfailprivacydisclosureaccount"
          privacynetwork: "checkfailprivacynetworknosupporttor"
---
