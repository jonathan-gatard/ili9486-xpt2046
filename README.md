# ili9486
Overlay for OrangePiZero screen ili9486 + xpt2046 (3.5inch rpi lcd (a) v3)



"armbian-add-overlay ili9486-xpt2046/screen.dts"

Pin DC : 18
Pin Reset : 2

Works on Amrbian Buster kernel 5.4.43-sunxi

With xinput, get pointer name : "DISPLAY=:0.0 xinput list"
then apply matrix to modify coordinates:
"DISPLAY=:0.0 xinput --set-prop 'ADS7846 Touchscreen' 'Coordinate Transformation Matrix' 0 -1 1 1 0 0 0 0 1"
