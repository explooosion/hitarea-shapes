# HitAreaShapes

Use [PixiJS](https://www.pixijs.com/) to set transparent shape's [hitArea](https://pixijs.download/dev/docs/PIXI.Sprite.html#hitArea) with multiple polygons. Please install [PhysicsEditor](https://www.codeandweb.com/physicseditor) before starting.

## Prepare

1. Download [PhysicsEditor](https://www.codeandweb.com/physicseditor).

2. Add sprite and use shape tracer.

3. Select `Phaser(P2)` from Exporter menu.

4. Publish image with JSON format.

## Installation

Installation is done using the npm install command:

```sh
npm install hitarea-shapes
```

## Example

Import module and your polygons json file.

```javascript
import HitAreaShapes from 'hitarea-shapes';
import polygons from './my-polygons.json';

const hitAreaShapes = new HitAreaShapes(data)
const sprite = PIXI.Sprite.from('https://pixijs.io/examples/examples/assets/flowerTop.png');

sprite.buttonMode = true;
sprite.interactive = true;

sprite.hitArea = hitAreaShapes;
```

## Credit

- [eXponenta](https://github.com/eXponenta) - [pixi-poly](https://github.com/eXponenta/pixi-poly)

## License

[MIT](http://opensource.org/licenses/MIT)
