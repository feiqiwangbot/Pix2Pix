Pix2Pix for Unity
=================

This is an attempt to run [pix2pix] (image-to-image translation with deep
neural network) in real time with [Unity]. It contains its own implementation
of an inference engine, so it doesn't require installation of other neural
network frameworks.

[pix2pix]: https://github.com/phillipi/pix2pix
[Unity]: https://unity3d.com

Sketch Pad demo
---------------

![screenshot](https://i.imgur.com/aXYYjes.gif)
![screenshot](https://i.imgur.com/Tb0nYqU.gif)

**Sketch Pad** is a demonstration that resembles the famous [edges2cats] demo
but in real time. You can download a pre-built binary from the [Releases] page.

[Demo video](https://vimeo.com/287778343)

[edges2cats]: https://affinelayer.com/pixsrv/
[Releases]: https://github.com/keijiro/Pix2Pix/releases

System requirements
-------------------

- Unity 2018.1
- Compute shader capability (DX11, Metal, Vulkan, etc.)

Although it's implemented in a platform agnostic fashion, many parts of it are
optimized for NVIDIA GPU architectures. To run the Sketch Pad demo flawlessly,
it's highly recomended to use a Windows system with GeForce GTX 1070 or greater.

How to use other models
-----------------------

This implementation supports the `.pict` weight data format which is used in
Christopher Hesse's [interactive demo]. Pick one of the [pre-trained models],
or you can train your own model with using [pix2pix-tensorflow].

[interactive demo]: https://affinelayer.com/pixsrv/
[pre-trained models]: https://github.com/affinelayer/pix2pix-tensorflow-models
[pix2pix-tensorflow]: https://github.com/affinelayer/pix2pix-tensorflow
