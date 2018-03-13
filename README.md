# three-js
### 2.1 场景(THREE.Scene):最核心的概念之一,是所有物体,光源和摄像机的容器;

|方法(属性)|描述|
|--|--|
|add(object)|用于在场景中添加对象.使用该方法还可以创建对象组|
|children|用于返回一个场景中所有对象的列表,包括摄像机和光源|
|getObjectByName(name, recursive)|在创建对象的时候可以指定唯一的name,使用该方法可以查找特定的名字.recursive(可选)为false时,在调用者子元素上查找,为true时,在调用者所有后代中查找|
|remove(object)|移除场景中的指定对象|
|travers(function)|该方法可以遍历调用者和调用者所有后代,Function是一个参数,被调用者和每一个后代对象调用Function方法|
|fog|雾化|
|overrideMaterial|使用该属性可以强制场景中的所有物体使用相同的材质|
