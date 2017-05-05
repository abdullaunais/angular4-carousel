# Angular4Carousel

Animated angular carousel

###Demo

http://angular4-carousel.bitballoon.com/

## Getting started

`npm i --save-dev angular4-carousel`

Add following lines into your

_module:_

`import { CarouselModule } from 'angular4-carousel';`

`imports: [CarouselModule]`

_component template:_

`<carousel [sources]="imageSources" [config]="config"></carousel>`

_component ts:_

`import { ICarouselConfig, AnimationConfig } from 'angular4-carousel';`

`public imageSources: string[] = [ `<br/>
    `'[img1 src]',`<br/>
    `'[img2 src]',`<br/>
    `'[img3 src]'`<br/>
  `];`<br/>
  ``<br/>
  `public config: ICarouselConfig = {`<br/>
    `verifyBeforeLoad: false,`<br/>
    `log: false,`<br/>
    `animation: true,`<br/>
    `animationType: AnimationConfig.APPEAR,`<br/>
    `autoplay: true,`<br/>
    `autoplayDelay: 500`<br/>
  `};`

## Config

_verifyBeforeLoad_ <br/>
values: false, true <br/>
If true, each image will render to view if and when load.
If false, all images render as soon as carousel init.

_log_: <br/>
values: false, true <br/>
Log to console on image load success or error

_animation:_ <br/>
values: false, true <br/>


_animationType_: <br/>
value: AnimationConfig.APPEAR, AnimationConfig.SLIDE_OVERLAP, AnimationConfig.SLIDE

_autoplay:_<br/>
values: false, true

_autoplayDelay:_ <br/>
values: [number]


