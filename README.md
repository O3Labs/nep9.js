# nep9.js

### Embed NEP9 QR code in your HTML

#### Usage

```html
<script type="text/javascript" src="js/nep9.js"></script>
```

define `div` element with `class=neo-nep9-qr`


##### Asset (*required* for native asset transfer)
The asset you would like a person scanning the QR code to send.  
`data-asset="neo"`  or `data-asset="gas"`  

#### NEP5 script hash (*required* for nep5 token transfer)
The nep5 token you would like a person scanning the QR code to send.  
`data-nep5="ceab719b8baa2310f232ee0d277c061704541cfb"`

##### Address (*required*)
Your valid NEO address.  
`data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb"`  

##### Amount (*optional*)
The amount you would like a person scanning the QR code to send.  
`data-amount="10"`  

##### QR Code width (*optional* default is 200px)
`data-width="200"`

##### QR Code height (*optional* default is 200px)
`data-height="200"`

##### Logo (*optional* default is NEO green logo)
`data-logo="https://o3.network/img/logo-color.png"`

#### Example native asset transfer

10 NEO to AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb
```html
<div class="neo-nep9-qr" data-asset="neo" data-amount="1" data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb"></div>
```


0.5 GAS to AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb
```html
<div class="neo-nep9-qr" data-asset="gas" data-amount="0.5" data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb"></div>
```

Unspecified amount of GAS to AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb (let sender decides)
```html
<div class="neo-nep9-qr" data-asset="gas" data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb"></div>
```


#### Example NEP5 transfer

unspecific amount of ONT to AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb with ONT logo
```html
<div class="neo-nep9-qr" data-nep5="ceab719b8baa2310f232ee0d277c061704541cfb" data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb" data-logo="https://avatars3.githubusercontent.com/u/36180490?s=200&v=4"></div>
```

10 ONT to AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb
```html
<div class="neo-nep9-qr" data-nep5="ceab719b8baa2310f232ee0d277c061704541cfb" data-address="AeNkbJdiMx49kBStQdDih7BzfDwyTNVRfb" data-amount="10" ></div>
```
