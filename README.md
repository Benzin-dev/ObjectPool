# ObjectPool
Object pooling system using custom class Object - int (number of clones) - List

Create empty object and attach this class to it.

In inspector add new Prefab Amount Lists. Drag prefab of object you want to clone in field Game Object and set it's maximum amount.
You can instantiate this object with command - var clone = ObjectPool.SharedInstance.GetPooledObject(int index).
Don't forget to make it active after initialization - clone.SetActive(true).
And deactivate it in order to re-initialize - clone.SetActive(false).

You can deactivate ALL active pooled objects with command - ObjectPool.SharedInstance.ClearPooledObjects().
