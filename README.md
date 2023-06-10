# My C++ Learnings

AKA These are the reasons to some weird errors/behaviours I encountered

- Why templates declared in header file and defined in a translation unit
  need to be instantiated explicitly
  - https://stackoverflow.com/questions/495021/why-can-templates-only-be-implemented-in-the-header-file
  - https://stackoverflow.com/questions/13269116/template-classes-multiple-file-project-how-to
  - https://stackoverflow.com/questions/3749099/why-should-the-implementation-and-the-declaration-of-a-template-class-be-in-the

- Allocated memory is not zeroed
  - https://stackoverflow.com/questions/47834180/set-an-array-to-zero-with-c11
  - https://stackoverflow.com/questions/9146395/reset-c-int-array-to-zero-the-fastest-way
  - Personally use `for (T &elem : arr) elem = 0;` for resetting and `T arr = {0};` for initialisation
