# QR-code-Generator
Welcome to the Python QR Code Generator, a simple yet powerful tool for creating QR codes effortlessly. This open-source project enables you to generate QR codes for various purposes, such as sharing URLs, contact information, or any other text-based data.

method 1(for black and white QR code)

import qrcode as qr
img=qr.make("https://github.com/HeenaMaheshwari")
img.save("Heena github.png")



method 2(adding colors)

import qrcode as qr
from PIL import Image
qr=qrcode.QRCode(version=1,error_correction=qrcode.constants.ERROR_CORRECT_H,box_size=10,border=10)
qr.add_data("https://github.com/HeenaMaheshwari")
qr.make(fit=True)
img=qr.make_image(fill_color="orange",back_color="white")
img.save("Heenam github.png")
