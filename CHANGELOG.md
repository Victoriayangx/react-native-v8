Change Log
==========

Version 0.65.1-patch.0
-------------------------------------------------------

 * [*Breaking Change*] Ship `v8-android-jit` by default.

If you use the default v8 variant included in `react-native-v8`, after this version, please change your `android/app/build.gradle`.

```diff
       maven {
           // prebuilt libv8android.so
-           url("$rootDir/../node_modules/v8-android/dist")
+           url("$rootDir/../node_modules/v8-android-jit/dist")
       }
```

 * Upgrade v8-android-* to 9.93.0 (V8 	9.3.345.16)
 
 Please use one of these variants
 - v8-android@~9.93.0
 - v8-android-jit@~9.93.0
 - v8-android-nointl@~9.93.0
 - v8-android-jit-nointl@~9.93.0

Version 0.64.2-patch.0 / 0.64.1-patch.0 / 0.64.0-patch.0
-------------------------------------------------------
Version 0.63.4-patch.1
-------------------------------------------------------

 * Upgrade v8-android-* to 9.88.0 (V8 8.8.278.15)
 
 Please use one of these variants
 - v8-android@~9.88.0
 - v8-android-jit@~9.88.0
 - v8-android-nointl@~9.88.0
 - v8-android-jit-nointl@~9.88.0

Version 0.63.4-patch.0 / 0.63.4-patch.0 / 0.63.2-patch.0 / 0.63.1-patch.0 / 0.63.0-patch.1
-------------------------------------------------------

 * Upgrade v8-android-* to 8.84.0 (V8 8.4.371.19)
 
 Please use one of these variants
 - v8-android@~8.84.0
 - v8-android-jit@~8.84.0
 - v8-android-nointl@~8.84.0
 - v8-android-jit-nointl@~8.84.0


Version 0.62.2-patch.1 / 0.62.1-patch.0 / 0.61.5-patch.3 *(2020-04)*
-------------------------------------------------------

 * Fix incorrect timezone issue [#37](https://github.com/Kudo/react-native-v8/issues/37)
 
 * Upgrade v8-android-* to 8.80.1 (V8 8.0.426.16)
 
 Please use one of these variants
 - v8-android@~8.80.1
 - v8-android-jit@~8.80.1
 - v8-android-nointl@~8.80.1
 - v8-android-jit-nointl@~8.80.1

Version 0.61.4-patch.0 / 0.60.6-patch.1 / 0.59.10-patch.3 *(2019-11-05)*
-------------------------------------------------------

 * Upgrade v8-android to 7.8.0 (V8 7.8.279.17)
 * Add dedicate V8Executor instead of patching JSCExecutor to prevent annoying error like https://github.com/Kudo/react-native-v8/issues/29
 
 Also backport for
 * 0.61.2-patch.0
 * 0.61.1-patch.2
 * 0.61.3-patch.0
 
Version 0.60.5-patch.0 *(2019-08-29)*
-----------------------------

 * Support React Native v0.60.5
 
Version 0.60.4-patch.2 / 0.59.10-patch.2 *(2019-08-29)*
-------------------------------------------------------

 * Fix parsing UTF-8 JS script error
 * Fix JSI crash during convert property numeric names
 
Version 0.60.4-patch.1 *(2019-08-14)*
-----------------------------

 * Add heap memory statistics `global._v8runtime().memory`
 
Version 0.60.4-patch.0 *(2019-07-25)*
-----------------------------

 * Support React Native v0.60.4

Version 0.60.3-patch.0 *(2019-07-16)*
-----------------------------

 * Support React Native v0.60.3

Version 0.60.0-patch.1 *(2019-07-08)*
-----------------------------

 * Fix: Crash or JS exception from V8PointerValue being GCed.


Version 0.60.0-patch.0 *(2019-07-03)*
-----------------------------

 * Release V8 runtime support for React Native.
