# Car In Situ

_Car In Situ_, aka CIS, is physical multiplayers racing car game.

The players drive RC cars using PC gamepad/wheel with a _FPV_ stream.

## Components

_CIS_ have been designed to run using on central unit (e.g. PC) where all player equipements are connected to.

### Common

As hardware, a central unit (e.g. PC) is required with
 - multiple display outputs video card (n players + 1 monitor)
 - multiple capture inputs (n players)

To build the WiFi network used by RC cars, a router is required, we highly recommend [Turris Omnia](https://www.turris.com/en/omnia/overview/) device.

On this station, the _CIS_ game is handled by
 - [CIS server](https://github.com/carinsitu/cis-server)
 - [CIS monitor](https://github.com/carinsitu/cis-monitor)

### Per player

To drive, a gamepad or wheel is required ; tested devices are _Logitech F310_ and _Logitech G920_.

For video feedback, the following is needed:
 - 5.8Ghz analog video receiver, like [ImmersionRC rapidFIRE](https://www.immersionrc.com/fpv-products/rapidfire/)
 - NTSC/PAL capture device, an USB one (take care about Linux compatibility)

And finally, an hacked/improved RC car.

### The hacked/improved RC car

The RC car used to develop _CIS_ is based on [Wl-Toys K989](https://www.wl-toys.com/WLtoys-K989-rc-car-Wltoys-K989-High-speed-128-Full-scale-rc-racing-car-10548.html) 1:28 RC car.

All original electronics is removed and replaced by the _CIS_ [PCB](https://github.com/carinsitu/car-pcb) with its [firmware](https://github.com/carinsitu/car-firmware).

For _FPV_, a camera and a video transmitter is required, the [FXT T82 camera + FX868T VTX]() kit provides quite good results.

### Interactive circuit

To improve the experience, the circuit can have bonus areas, checkpoints and finish line.

To build them, simply use _CIS_ [Gate](https://github.com/carinsitu/gate-firmware) to light the area with a continously sent IR code.
