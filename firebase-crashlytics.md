# Firebase Crashlytics

I thought crashlytics work using the uncaught exception handler, but in reality they just intercept the signals. 

```text
SIGABRT, SIGBUS, SIGFPE, SIGILL, SIGSEGV, SIGSYS, SIGTRAP
```



