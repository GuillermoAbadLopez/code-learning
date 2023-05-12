**PATCHING PYCON LEARNINGS:**
https://www.youtube.com/watch?v=ww1UsGZV8fQ

6:50 - Target must be importable
-- patch auto-imports the target for you

7:30 - Don't patch where the function is declared, but where it is referenced

8:42 - If you import a function from a module: Use the importing module's name to target the function instead of the imported module. This is because the importing module's lookup table contains the function

9:36 - If you import an entire module: Use the imported module's name to target the function instead of the importing function.

11:12 - Scope tier
-- Context Manager - duration is a partial life of a function
-- Function decorator - duration is the entire life of a function
-- Class decorator - duration is the entire life of all functions inside the class

13:05 - It's recommended to use Context Manager for built-in functions

14:00 - Remember that a decorator creates a MagickMock object. It must be passed as an argument into the tested function.
 
14:39 - Yes, decorators can be stacked. However this is at the expense of DRY.

14:53 - in `setUp`, your patches can be started. You can then stop them all in `addCleanup`  if a test goes bad before `tearDown` happens.
