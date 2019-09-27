# ROS2 GitLab CI example project

There are 3 important files here: `.gitlab-ci.yml`, `package.xml`, and `CMakeLists.txt`.

So in `package.xml` you need to add the following lines:
```
<test_depend>ament_lint_auto</test_depend>
<test_depend>ament_lint_common</test_depend>
```

And in `CMakeLists.txt` you need to add the following lines:
```
find_package(ament_lint_auto REQUIRED)
ament_lint_auto_find_test_dependencies()
```
## Travis CI
Right now works, but the approach is too straightforward
Checkout the `.travis.yml` file
