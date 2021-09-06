


## Sample App

### 사용법


`<proj>\app\src\main\AndroidManifest.xml` 에서 api key 만 각자의 api key 로 변경해주자.


```xml
...
<meta-data android:name="dev_84ff2c24bba969e74aeae4b56f41cb19a87d71e2" android:value="API KEY" />

```

이제 `gradlew bundle` 을 하면, apk 가 만들어진다. 아래경로에서 확인할 수 있다.

```
<proj>\app\build\outputs\apk\debug\app-debug.apk
```


#### Windows 10


`gradlew build` 를 통해서 제대로 build 가 되는지 확인해 보면 된다.

```
gradlew tasks
...
gradlew build
```

```
c:\android-sdk-sample>gradlew build

> Task :app:compileDebugUnitTestKotlin
w: c:\android-sdk-sample\app\src\test\java\com\test\myapplication\ExampleUnitTest.kt: (15, 25): This expression will be resolved to Int in further releases. Please add explicit convention call

> Task :app:compileReleaseUnitTestKotlin
w: c:\android-sdk-sample\app\src\test\java\com\test\myapplication\ExampleUnitTest.kt: (15, 25): This expression will be resolved to Int in further releases. Please add explicit convention call

> Task :app:lintDebug
Wrote HTML report to file:///D:/a/prog/kotlin/android-sdk-sample/app/build/reports/lint-results-debug.html

Deprecated Gradle features were used in this build, making it incompatible with Gradle 8.0.
Use '--warning-mode all' to show the individual deprecation warnings.
See https://docs.gradle.org/7.0.2/userguide/command_line_interface.html#sec:command_line_warnings

BUILD SUCCESSFUL in 16s
71 actionable tasks: 71 executed
```