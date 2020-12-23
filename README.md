# ili9486
Overlay pour OrangePiZero écran ili9486 + xpt2046 (3.5inch rpi lcd (a) v3)



"armbian-add-overlay ili9486-xpt2046/screen.dts"

Pin DC : 18
Pin Reset : 2

Fonctionne sur Amrbian Buster kernel 5.4.43-sunxi

Avec xinput, repérer le nom du pointeur : "DISPLAY=:0.0 xinput list"
puis appliquer la matrice pour transformer les coordonées:
"DISPLAY=:0.0 xinput --set-prop 'ADS7846 Touchscreen' 'Coordinate Transformation Matrix' 0 -1 1 1 0 0 0 0 1"
