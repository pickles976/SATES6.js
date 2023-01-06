SATES6.js 
=====

SATES6.js is an ES6 version of the [SAT.js](https://github.com/pboechat/SAT.js)

SAT.js is useful when you want to test collision of two convex polyhedra, but don't want the overhead of a physics engine line Cannon.js or Ammo.js. It can take in geometries in the Three.js format.


## SAT.js

**SAT.js** is a Javascript implementation of the Separating Axis Theorem for convex polygons and polyhedra.

Requires [three.js](http://threejs.org/).

Based on [this article](http://www.geometrictools.com/Documentation/MethodOfSeparatingAxes.pdf).


----------

### Usage

Add three.js and SAT.js to your page:

	*TODO: SHOW USERS HOW YOU CAN IMPORT SATES6.js*

#### Polyhedra

Convert your Three.js geometries to a SAT.js shape object.

    import * as THREE from 'three'
    import { ShapeFromGeometry } from 'SAT.js'

    const box1 = new THREE.BoxGeometry(1, 1, 1)
    const box2 = new THREE.BoxGeometry(2, 2, 2)

    const collider1 = ShapeFromGeometry(box1)
    const collider2 = ShapeFromGeometry(box2)

#### Collision Checking

    import { CheckCollision } from 'SAT.js'
	CheckCollision(collider1, collider2)


----------

### Demo

Examine the SAT algorithm step-by-step [here](http://pedroboechat.com/SAT.js/3D/main.html).

----------

### Video

[![Video](http://www.pedroboechat.com/images/SATjs-video-thumbnail.png)](https://www.youtube.com/watch?v=djKUDMbGMM4)
