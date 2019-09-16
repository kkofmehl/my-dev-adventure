# What's New In C#8

Jason Bock

https://www.github.com/JasonBock/WhatsNewInCCharp8

https://www.github.com/JasonBock/Presentations

## History

C# was initially a response to Java

.NET Full 4.8 is the last version to ship (10 years of LTE)

Currently, installing the "Preview" version of Visual Studio, the Visual Studio Installer is doing a good job of isolating the instances (little worry about breaking the environment)

### Patterns

- Enhancement of the "switch" function but specifically for type/sub types

## New Features

### Nullable Reference Types:

- Compiler feature must be opted-in to at the Project File level
    - `<Nullable>enabled</Nullable>`
	- `#nullable disable` (can be added to any class file to disabled the nullable checking for that file)
	- `!.`  (Dammit Operator) (Null Forgiving Operator)

### Enhanced `using`

- Removes the "block" part of using
- Everything under the declaration of the Discard using object is in the using
- Not sure about this one….

### Asynchronous Disable
- `IAsyncDisposable`

### Asynchronous Streams  (Asyncronous foreach)
- "I know I'm getting a stream of data, I just don't know if I'm going to get all of them, or how long it will take to get them all"
- `await foreach (){}`

### Ranges and Indexes  (check out the source code for better details here…)

#### Operators
- `..`
- `x..x` 
- `x..`
- `..^x`  
- `^x`
- `Range()`
- `Index()`
- rangeCopy
- rangeSlice

### Default Interface Members

- Implementations in the interface?
- Yucky!

### Null Coalescing Assignments

- `??`  Assign to another method if a value is null
- I could see this coming in handy...

### Verbatim Interpolation Strings

- `$@` or `@$` Order doesn't matter

### Static Local Functions

- Make a local function static, but it cannot capture local variables from the surrounding function





