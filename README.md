# unison-libs
sample Unison language repo

### `either` branch
```haskell
type Either a b
(Either.>>=) : Either a b -> (b -> Either a c) -> Either a c
Either.either : (a -> c) -> (b -> c) -> Either a b -> c
Either.fromLeft : a -> Either a b -> a
Either.fromRight : b -> Either a b -> b
Either.isLeft : Either a b -> Boolean
Either.isRight : Either a b -> Boolean
Either.leftToOptional : Either a b -> Optional a
Either.rightToOptional : Either a b -> Optional b
```
