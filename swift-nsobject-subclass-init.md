# Swift NSObject subclass init

Swift compiler generates a bridging header. If there are no inits defined, then the default init is inserted.

```text
- (nonnull instancetype)init OBJC_DESIGNATED_INITIALIZER;
```

However, if there are any other initializers defined, they are marked `designated` by default. 

```text
- (nonnull instancetype)initWithDictionary:(NSDictionary<NSString *, id> * _Nonnull)dictionary OBJC_DESIGNATED_INITIALIZER;
```

If only we explicitly mark an initializer `convenience`, it does not mark it designated, which is obvious but I needed to verify 

```text
- (nonnull instancetype)init OBJC_DESIGNATED_INITIALIZER;
- (nonnull instancetype)initWithDictionary:(NSDictionary<NSString *, id> * _Nonnull)dictionary;
```



