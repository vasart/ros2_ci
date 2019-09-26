# ros2_ci

There are 3 important files here:
`.gitlab-ci.yml`,
`package.xml`,
and
`CMakeLists.txt`.

In package.xml you need to add the following lines:
```
<test_depend>ament_lint_auto</test_depend>
<test_depend>ament_lint_common</test_depend>
```

In `CMakeLists.txt` you need to add the following lines:
```
find_package(ament_lint_auto REQUIRED)
ament_lint_auto_find_test_dependencies()
```

