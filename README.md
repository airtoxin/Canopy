# Canopy
css components of hexagonal grid system.

[![https://gyazo.com/5ad50294e56d86ca84ed29e6f823d5fd](https://i.gyazo.com/5ad50294e56d86ca84ed29e6f823d5fd.png)](https://gyazo.com/5ad50294e56d86ca84ed29e6f823d5fd)

## Install

### use compiled css file

CURRENTLY, THERE ARE NO FLEXIBILITY OF HEXAGON SIZE 100px FIXED.

Download css file from [Github release page](https://github.com/airtoxin/Canopy/releases) and load it on your html.

```html
<link rel="stylesheet" type="text/css" href="path/to/canopy.css">
```

### use raw less file

Download less file from [Github release page](https://github.com/airtoxin/Canopy/releases). Load canopy less file and less.js.

```html
<link rel="stylesheet/less" type="text/css" href="path/to/canopy/index.less">
<script src="less.js" type="text/javascript"></script>
```

And, change hex size

```javascript
less.modifyVars({hexsize: '10px'})
```

## Hex component

There are 2 grid directions 'row-oriented' and 'column-oriented'.

### row-oriented grid

```html
<div class="canopy-row">
  <div class="hexes">
    <div class="hex">1</div>
    <div class="hex">2</div>
  </div>
  <div class="hexes">
    <div class="hex">3</div>
    <div class="hex">4</div>
  </div>
  <div class="hexes">
    <div class="hex">5</div>
    <div class="hex">6</div>
  </div>
</div>
<style>
  .hex {
    background-color: gray;
  }
</style>
```

[![https://gyazo.com/cc2f38dea3241148ca07ff2bf06a0fb2](https://i.gyazo.com/cc2f38dea3241148ca07ff2bf06a0fb2.png)](https://gyazo.com/cc2f38dea3241148ca07ff2bf06a0fb2)

### column-oriented grid

```html
<div class="canopy-col">
  <div class="hexes">
    <div class="hex">1</div>
    <div class="hex">2</div>
  </div>
  <div class="hexes">
    <div class="hex">3</div>
    <div class="hex">4</div>
  </div>
  <div class="hexes">
    <div class="hex">5</div>
    <div class="hex">6</div>
  </div>
</div>
<style>
  .hex {
    background-color: gray;
  }
</style>
```

[![https://gyazo.com/2bea5bb8f281b0913d032606771dc02b](https://i.gyazo.com/2bea5bb8f281b0913d032606771dc02b.png)](https://gyazo.com/2bea5bb8f281b0913d032606771dc02b)

## Change hexagon size

If you load canopy from less, it can modify hexagon size.

`less.modifyVars({hexsize: '10px'})`

## Example

See [example directory](https://github.com/airtoxin/Canopy/tree/master/example)
