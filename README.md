# nep9.js

### Embed NEP9 QR code in your HTML

#### Usage

```html
<script type="text/javascript" src="js/nep9.js"></script>
```

define `div` element with `class=neo-nep9-qr`


##### Asset (*required*)
The asset you would like a person scanning the QR code to send.  
`data-asset="neo"`  or `data-asset="gas"`  

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

#### Example

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