# 光源
光源也是很重要的一部分,没有光源,渲染的场景将不可见.WebGL本身不支持光源,需要自己写WebGL着色程序.在Three.js中封装了多种光源

### three.js中光源列表

|名字|描述|
|--|--|
|THREE.AmbientLight|一个基本光源,该光源的颜色将会叠加到场景现有物体的颜色上|
|THREE.PointLight|点光源,从空间的一点向所有方向发射光线,点光源不能用来创建阴影|
|THREE.SpotLight|有聚光的效果,类似台灯,天花板上的吊灯或者手电筒,这种光源可以投射阴影|
|THREE.DirectionalLight|也成为无限光,从这种光源发出的光线可以看做是平行的,就类似太阳光.这种光源也可以投射阴影|
|THREE.HemisphereLight|特殊的光源,可以通过模拟反光面和光线微弱的天空来创建更自然的室外光线.这个光源不提供与阴影相关的功能|
|THREE.AreaLight|使用该光源可以指定散发光线的平面,而不是一个点.不投射任何阴影|
|THREE.LensFlare|不是一个光源,但是可以为场景中的光源添加镜头光晕效果|

* 基础光源: `THREE.AmbientLight`, `THREE.PointLight`, `THREE.SpotLight`, `THREE.DirectionalLight`
* 特殊光源: `THREE.HemisphereLight`, `THREE.AreaLight`, `THREE.LensFlare`

