# Introduction #

  * Keep the OS functions out of the public OG headers (eg. do not #include <pthread.h>/<windows.h> in a public header file).
    * OS specific headers should always stay out of the public OG headers.
    * If you need those headers, try to move them into the .cpp files or into a header that is only used internally within the library (e.g. a header in the Libraries/Source folder).

  * Try to avoid using the any kind of prefixes unless you have name collisions that can't be solved nicer.
    * Discuss this with team members if you're unsure how to name it.