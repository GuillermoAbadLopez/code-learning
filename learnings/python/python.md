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

## **Youtube list recommended by Joel:**
https://www.youtube.com/playlist?list=PLC0nd42SBTaNuP4iB4L6SJlMaHE71FG6N
- COHESION: Group things as it makes sense, and make lots of functions that do little thing inside each class.

- COUPLING: Minimize coupling, is something is too much coupled with another thing, maybe they should be the same thing, or have inherance

- ABSTRACTION: Use ABC to denote abstraction

- DEPENDENCY INVERION: If various things do somehting, make and abstract class to group them

- SMALL classes, separate things into subgroups that are cohesive, but not everything in a super big group, do splits that make sense.

- CACHE usage, with `@cached_property` for properties or with `@lru_cache()` for functions

- https://realpython.com/python-kwargs-and-args/ `*args` & `**kwarg` for iterating arguments and keyword-arguments as tuples and dictionaries. * also unpacks any iterable and ** unpacks dictionaries:  `def my_function(a, b, *args, **kwargs):` 

- DECORATORS are just functions that recieve functions and return other functions

- DESIGNS PATERNS:
-- STRATEGY:
-- FACTORY:
