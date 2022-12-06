# Reproduction of mixing and matching of kotlin-stdlib 1.8.0 and kotlin-stdlib-jdk7 <1.8.0

## Steps
1. ./gradlew assembleAndroidTest


## Expected
Success

## Actual
Failure

```
FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':app:checkDebugAndroidTestDuplicateClasses'.
> A failure occurred while executing com.android.build.gradle.internal.tasks.CheckDuplicatesRunnable
   > Duplicate class kotlin.internal.jdk7.JDK7PlatformImplementations found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.internal.jdk7.JDK7PlatformImplementations$ReflectSdkVersion found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.DirectoryEntriesReader found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.ExperimentalPathApi found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.FileVisitorBuilder found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.FileVisitorBuilderImpl found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.FileVisitorImpl found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.LinkFollowing found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathNode found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathRelativizer found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathTreeWalk found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathTreeWalk$bfsIterator$1 found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathTreeWalk$dfsIterator$1 found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathTreeWalkKt found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathWalkOption found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathsKt found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathsKt__PathReadWriteKt found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.io.path.PathsKt__PathUtilsKt found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     Duplicate class kotlin.jdk7.AutoCloseableKt found in modules kotlin-stdlib-1.8.0-Beta (org.jetbrains.kotlin:kotlin-stdlib:1.8.0-Beta) and kotlin-stdlib-jdk7-1.7.21 (org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.7.21)
     
     Go to the documentation to learn how to <a href="d.android.com/r/tools/classpath-sync-errors">Fix dependency resolution errors</a>.

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Get more help at https://help.gradle.org
```