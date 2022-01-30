## abstract base class
*short term: ABCs*
Complements [[duck-typing]] by providing a way to define interfaces when other techniques like `hasattr()` would be clumsy or subtly wrong (e.g. - [[magic method]]s).

ABCs introduce `issubclass()`
You can create your own ABCs with the `abc` module<br>


Python comes with many built-in ABCs:
+ data structures --> in the `collections.abc` module
+ numbers --> in the `numbers` module
+ streams --> in the `io` module
+ import finders and loaders --> in the `importlib.abc` module

