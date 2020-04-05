# Write External Library

## Step:

### 1. Create External Library:

Source: https://github.com/huubao2309/write_library_external/tree/master/library/lib_math

### 2. Public class for using:

Source: https://github.com/huubao2309/write_library_external/blob/master/library/lib_math/lib/lib_math.dart

```dart
library lib_math;

export 'src/lib_math_base.dart';
export 'src/sin.dart' hide Sqrt;
export 'src/cos.dart';
```

**Note**: `Hide` is a keyword for hiding class that preventing the user uses it.

### 3. Add library at `pubspec.yaml`:

```dart
dependencies:
  lib_math:
    path: ../write_library_external/library/lib_math
```

### 4. Use method of library:

```dart
  var sin = math.Sin().of(90);
  var cos = math.Cos().of(90);
```

