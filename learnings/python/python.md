## **First python tutorials:**
https://www.youtube.com/playlist?list=PLpOqH6AE0tNiK7QN6AJo_3nVGQPc8nLdM

## **MIT lectures, what have I learned/need to practice:**
https://ocw.mit.edu/courses/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/
- Pythonic for loops with elements directly

- Specification for functions (at the start comment what it does, and what inputs/outputs has)

- Function scopes/frame/enviorements, global scope vs f scope

- Tuples [Inmutable] vs List [mutable] (alisaing and clonning problems too)

- Recursion functions ( `f(x)= something & f(x-1)` )

- Dictionaries (play with them, understand them)

- Unit testing (functions) -> Regression testing (if you changed something, check again) -> Integration testing (hole system)

- Black box testing (with specification only, it can be math boundries, irrationals, decimals, extremes, etc...) & glass box testing (with code, go through all paths of the code, through code boundaries also)

- Debugg with [try: , except: , assertions &  with prints/raises/returns, etc..]

## **Qilimanjaro leanings:**
- Abstract classes are OP (ABC w @abstractclass)

- `@dataclass` makes your life easier, for example no need for init, you can write the data as attributes directly

- Factoryelements cool too

- Pytest and fixtures are amazing, debug with `set_trace()` or better with debugging run in pytest interface.

- Polymorfism is the provision of a single interface to entities of different types[1] or the use of a single symbol to represent multiple different types https://en.wikipedia.org/wiki/Polymorphism_(computer_science)

## **Youtube list recommended by Joel:**
https://www.youtube.com/playlist?list=PLC0nd42SBTaNuP4iB4L6SJlMaHE71FG6N
- COHESION: Group things as it makes sense, and make lots of functions that do little thing inside each class.

- COUPLING: Minimize coupling, is something is too much coupled with another thing, maybe they should be the same thing, or have inherance

- ABSTRACTION: Use ABC to denote abstraction

- SMALL classes, separate things into subgroups that are cohesive, but not everything in a super big group, do splits that make sense.

- CACHE usage, with `@cached_property` for properties or with `@lru_cache()` for functions

- https://realpython.com/python-kwargs-and-args/ `*args` & `**kwarg` for iterating arguments and keyword-arguments as tuples and dictionaries. * also unpacks any iterable and ** unpacks dictionaries:  `def my_function(a, b, *args, **kwargs):` 

- DECORATORS are just functions that recieve functions and return other functions

- DESIGNS PATERNS: 
    - DECORATOR: Gives an extra functionality to a previous class (wrapps it around with extra things)
    - STRATEGY: Change the behaviour of something (the guts) in runtime depending of input: if car -> build_car_route, if boat -> build_boat rute, ...
    - FACTORY: Change the object you create depending on input: if car -> create car object, if boat -> create car object,...
    - ABSTRACT FACTORY: It implements multiple factory methods at the same time...
    - OBSERVER: 

- DEPENDENCY INJECTION: Takes the creation of the dependacy class outside the dependent class. So basically you have to pass the the dependacy class already instanciated to the dependant class (You INJECT the class you depend on!). Making everything easier to test! (Without this there can not be DEPENDENCY INVERSION) 

- DEPENDENCY INVERION_take1: If various things do somehting, make and abstract class to group them

- DEPENDENCY INVERSION_take2: Higher classes shouldnt depend on lower ones, instead have interfaces for that dependancy, so if you can change the lower ones, but they still fullfull the interface there will be no problem! (I believe this is what we do when we create the abstract classes of PulseShape or PulseDistortion, they are the interfaces so that Pulse or PulseEvent don't depend on the subclasses directly!)
[https://medium.com/ssense-tech/dependency-injection-vs-dependency-inversion-vs-inversion-of-control-lets-set-the-record-straight-5dc818dc32d1#:~:text=The%20Inversion%20of%20Control%20is,dependencies%20to%20an%20application's%20class]

