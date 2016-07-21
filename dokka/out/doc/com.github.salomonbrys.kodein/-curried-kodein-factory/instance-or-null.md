[com.github.salomonbrys.kodein](../index.md) / [CurriedKodeinFactory](index.md) / [instanceOrNull](.)

# instanceOrNull

`inline fun <reified T : Any> instanceOrNull(tag: Any? = null): T?`

Gets an instance of `T` for the given tag from a curried factory with an `A` argument, or null if none is found.

Whether the returned object is a new instance at each call or not depends on the binding scope.

### Parameters

`T` - The type of object to retrieve.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.DependencyLoopException` - If the instance construction triggered a dependency loop.

**Return**
An instance, or null if no factory was found.
