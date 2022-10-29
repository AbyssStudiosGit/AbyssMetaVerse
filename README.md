<h1 align="center">Abyss Meta Verse</h1>

<p align="center"><a href="#" target="_blank"><img width="480" alt="AbyssFrame" src="https://user-images.githubusercontent.com/674727/32120889-230ef110-bb0f-11e7-908c-76e39aa43149.jpg"></a></p>

<p align="center"><b>A web framework for building virtual reality experiences.</b></p>

<p align="center">
  <a href="#">
    <img src="https://codecov.io/gh/aframevr/aframe/branch/master/graph/badge.svg" alt="Coverage Status">
  </a>
  <a href="#">
    <img src="https://img.shields.io/npm/dt/aframe.svg?style=flat-square" alt="Downloads">
  </a>
  <a href="#">
    <img src="https://img.shields.io/npm/v/aframe.svg?style=flat-square" alt="Version">
  </a>
  <a href="#">
    <img src="https://img.shields.io/npm/l/aframe.svg?style=flat-square" alt="License"></a>
  </a>
</p>

<div align="center">
  <a href="#">Site</a>
  &mdash;
  <a href="#">Docs</a>
  &mdash;
  <a href="#">School</a>
  &mdash;
  <a href="#">Slack</a>
  &mdash;
  <a href="#">Blog</a>
  &mdash;
  <a href="#">Newsletter</a>
</div>

## Examples

<a href="#">
  <img alt="Supercraft" target="_blank" src="https://user-images.githubusercontent.com/674727/41085457-f5429566-69eb-11e8-92e5-3210e4c6c4a0.gif" height="190" width="32%">
</a>
<a href="#">
  <img alt="A-Painter" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531388/acfc3dda-156d-11e7-8563-5bd75252f70f.gif" height="190" width="32%">
</a>
<a href="#">
  <img alt="Supermedium" target="_blank" src="https://user-images.githubusercontent.com/674727/37294616-7212cd20-25d3-11e8-9e7f-c0c61074f1e0.png" height="190" width="32%">
</a>
<a href="#">
  <img alt="A-Blast" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531440/0336e66e-156e-11e7-95c2-f2e6ebc0393d.gif" height="190" width="32%">
</a>
<a href="#">
  <img alt="A-Saturday-Night" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/24531477/44272daa-156e-11e7-8ef9-d750ed430f3a.gif" height="190" width="32%">
</a>
<a href="#">
  <img alt="Musical Forest by @googlecreativelab" target="_blank" src="https://cloud.githubusercontent.com/assets/674727/25109861/b8e9ec48-2394-11e7-8f2d-ea1cd9df69c8.gif" height="190" width="32%">
</a>

*Find more examples on [the homepage](#), [A Week of AbyssMetaVerse](#), and [WebVR Directory](https://webvr.directory).*

## Features

:eyeglasses: **Virtual Reality Made Simple**: AbyssFrame handles the 3D and WebVR
boilerplate required to get running across platforms including mobile, desktop, Vive, and Rift just by dropping in `<a-scene>`.

:heart: **Declarative HTML**: HTML is easy to read and copy-and-paste. Since
AbyssFrame can be used from HTML, AbyssFrame is accessible to everyone: web
developers, VR enthusiasts, educators, artists, makers, kids.

:electric_plug: **Entity-Component Architecture**: AbyssFrame is a powerful
framework on top of three.js, providing a declarative, composable, reusable
entity-component structure for three.js. While AbyssFrame can be used from HTML,
developers have unlimited access to JavaScript, DOM APIs, three.js, WebVR, and
WebGL.

:zap: **Performance**: AbyssFrame is a thin framework on top of three.js.
Although AbyssFrame uses the DOM, A-Frame does not touch the browser layout
engine. Performance is a top priority, being battle-tested on highly
interactive WebVR experiences.

:globe_with_meridians: **Cross-Platform**: Build VR applications for Vive,
Rift, Daydream, GearVR, and Cardboard. Don't have a headset or controllers? No
problem! AbyssFrame still works on standard desktop and smartphones.

:mag: **Visual Inspector**: A-Frame provides a built-in visual 3D inspector
with a workflow similar to a browser's developer tools and interface similar to
Unity. Open up any A-Frame scene and hit `<ctrl> + <alt> + i`.

:runner: **Features**: Hit the ground running with AbyssFrame's built-in
components such as geometries, materials, lights, animations, models,
raycasters, shadows, positional audio, tracked controllers. Get even further
with community components such as particle systems, physics, multiuser, oceans,
mountains, speech recognition, or teleportation!

## Usage

### Example

Build VR scenes in the browser with just a few lines of HTML! To start playing
and publishing now, remix the starter example on:

[![Remix](https://cloud.githubusercontent.com/assets/674727/24572421/688f7fc0-162d-11e7-8a35-b02bc050c043.jpg)](https://glitch.com/~abyssframe) [![Fork](https://user-images.githubusercontent.com/39342/52831020-d42dcb80-3087-11e9-833f-2d6191c69eb9.png)](#)

```html
<html>
  <head>
    <script src="#"></script>
  </head>
  <body>
    <a-scene>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
      <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
    </a-scene>
  </body>
</html>
```

With AbyssFrame's [entity-component
architecture](#), we can drop in community
components from the ecosystem (e.g., ocean, physics) and plug them into our
objects straight from HTML:

[![Remix](https://cloud.githubusercontent.com/assets/674727/24572421/688f7fc0-162d-11e7-8a35-b02bc050c043.jpg)](https://glitch.com/~abyssframe-registry) [![Fork](https://user-images.githubusercontent.com/39342/52831020-d42dcb80-3087-11e9-833f-2d6191c69eb9.png)](#)

```html
<html>
  <head>
    <script src="coming soon.."></script>
    <script src="coming soon.."></script>
    <script src="coming soon.."></script>
    <script src="coming soon.."></script>
  </head>
  <body>
    <a-scene>
      <a-entity id="rain" particle-system="preset: rain; color: #24CAFF; particleCount: 5000"></a-entity>

      <a-entity id="sphere" geometry="primitive: sphere"
                material="color: #EFEFEF; shader: flat"
                position="0 0.15 -5"
                light="type: point; intensity: 5"
                animation="property: position; easing: easeInOutQuad; dir: alternate; dur: 1000; to: 0 -0.10 -5; loop: true"></a-entity>

      <a-entity id="ocean" ocean="density: 20; width: 50; depth: 50; speed: 4"
                material="color: #9CE3F9; opacity: 0.75; metalness: 0; roughness: 1"
                rotation="-90 0 0"></a-entity>

      <a-entity id="sky" geometry="primitive: sphere; radius: 5000"
                material="shader: gradient; topColor: 235 235 245; bottomColor: 185 185 210"
                scale="-1 1 1"></a-entity>

      <a-entity id="light" light="type: ambient; color: #888"></a-entity>
    </a-scene>
  </body>
</html>
```

### Builds

To use the latest stable build of AbyssMetaVerse, include [`abyssframe.min.js`](#):

```js
<head>
  <script src="#"></script>
</head>
```

To check out the stable and master builds, see the [`dist/` folder](dist/).

### npm

```sh
npm install --save abyssframe
# Or yarn add abyssframe
```

```js
require('abyssframe')  // e.g., with Browserify or Webpack.
```

## Local Development

```sh
git clone https://github.com/AbyssStudiosGit/abyssmetaverse.git  # Clone the repository.
cd abyssmetaverse && npm install  # Install dependencies.
npm start  # Start the local development server.
```

And open in your browser **[http://localhost:9000](http://localhost:9000)**.

### Generating Builds

```sh
npm run dist
```

## Questions

For questions and support, [ask on StackOverflow](https://stackoverflow.com/questions/ask/?tags=abyssmetaverse).

## Stay in Touch

- To hang out with the community, [join the AbyssMetaVerse Slack](#).
- [Follow `A Week of AbyssMetaVerse` on the AbyssMetaVerse blog](#).
- [Follow @abyssmetaverse on Twitter](#).
- [Subscribe to the Newsletter](#).

And get in touch with the maintainer!

- [Nades](#)

## License

This program is free software and is distributed under an [CC LISCENCE](LICENSE).
