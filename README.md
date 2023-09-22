# myqr
## QR Code scanner for login hotspot MikroTik

### Cara pakai

1. Tambahkan button di login.html  atau gnakan nav jika tidak menggunakan tombol.
```html
<button onclick="window.location='https://ajiedev-net.rf.gd/dnet_qr/';">QR Code</button>
```
2. Tambahkan script berikut di MikroTik via Terminal.
```
/ip hotspot walled-garden ip

add action=accept comment="Mikhmon QR Code Scanner" disabled=no dst-host=ajiedev-net.rf.gd


