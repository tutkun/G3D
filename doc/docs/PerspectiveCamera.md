# PerspectiveCamera

Perspective Camera. Extends from [Node](./Node).

## Constructor

```javascript
new G3D.PerspectiveCamera(scene);
```

### options

| name  | type      | description                                 |
| ----- | --------- | ------------------------------------------- |
| scene | G3D.Scene | the g3d scene you want to put the camera in |

## Properties

| name      | type   | description                                                |
| --------- | ------ | ---------------------------------------------------------- |
| near      | Number | distance between camera and the near plane, default is 1   |
| far       | Number | distance between camera and the far plane, default is 1000 |
| fov       | Number | field of view, default is 90                               |
| viewRatio | Number | view's width / height, default is 1                        |

## Methods

### getViewRay(x, y, flip)

Create a ray from camera position to the mouse-click direction.

#### options

| name | type    | description                                  |
| ---- | ------- | -------------------------------------------- |
| x    | Number  | mouse-click position x value in the canvas   |
| y    | Number  | mouse-click position y value in the canvas   |
| flip | Boolean | whether to flip the y value, default is true |

#### returns

ray: G3D.Ray | null, the created ray