#### 2.0.0
- Hooks into gradle's incremental compilcation support. This should mean faster build times and less
  inconsistencies when changing the build script without running `clean`. To fully take advantage of
  this you need to use retrolambda `1.4.0+` which is now the default.

#### 1.3.3
- Allow `retrolamba` plugin to be applied before or after `java` and `android`
  plugins

#### 1.3.2
- Fixed for android gradle plugin `0.10.+`

#### 1.3.1
- Removed `compile` property, which didn't work anyway. Use `retrolambdaConfig`
  instead.
- Minor error message improvement.

#### 1.3.0
- Support android instrument tests.

#### 1.2.0
- Support android-library projects.

#### 1.1.1
- Fixed not correctly finding java 8 executable when running from java 6 or 7 on
  windows. (Mart-Bogdan)

#### 1.1
- Fixed bug where java unit tests were not being run through retrolambda
- Allow gradle to be called with java 6 or 7, i.e. Java 8 no longer has to be
  your default java.
- Thank you Mart-Bogdan for starting these fixes.
