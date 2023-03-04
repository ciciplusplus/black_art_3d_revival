# Ported source code from book "Black Art of 3D Game Programming"

Book https://www.amazon.com/Black-Art-Game-Programming-High-Speed/dp/1571690042

The code from the book was ported to MacOS using SDL library.

## 🤔 How to use

⚠️ You'll need an original CD-ROM provided with the book

1. Checkout the repository
2. Copy contents of SOURCE/MSC folder from the disk
3. Run `git apply --reject --whitespace=fix patch.diff`
4. Enjoy

## 🛠️ Project structure and build instructions

Each ported chapter contains HostApp folder with Xcode project targeted last demo from the chapter.

You'll need to have SDL 2.x installed in the system in order to build.
It was tested with version `2.26.2`.

The projects expectes SDL to be installed with Homebrew:

```
brew install sdl2
```

## 🗒️ TODO

- [ ] Update projects to use version independent SDL path
- [ ] Port to other platforms (Linux, Windows)
- [ ] Create muliple targets per demos (currently only last demo from each chapter is targeted)
- [ ] Port missing chapters (e.g. the one with music and sound!)

## 🙇 Acknowledgments

- [Andre LaMothe twitter](https://twitter.com/nurvenetworks) (Author of the book!)
- [Cicoparser project](https://github.com/gabonator/Education/tree/master/2021/CicoParser) (HostApp is originally from there)
- [SDL library](https://www.libsdl.org/)
