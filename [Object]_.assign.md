# [合并object key生成新的object]
 
> 
    _.assign(object, [sources])

Arguments
object (Object): The destination object.
[sources] (…Object): The source objects.
Returns
(Object): Returns object.

```
function Foo() {
  this.c = 3;
}

function Bar() {
  this.e = 5;
}

Foo.prototype.d = 4;
Bar.prototype.f = 6;

_.assign({ 'a': 1 }, new Foo, new Bar);
// → { 'a': 1, 'c': 3, 'e': 5 }
```
