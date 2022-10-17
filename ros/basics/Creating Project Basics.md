# Creating Project Basics

```jsx
catkin_create_pkg <NAME> <DEPENDENCY_PKG1> <DEPENDENCY_PKG2> ...
```

![Untitled](../../docs/ros/basics/Creating%20Project%20Basics/Untitled.png)

- package.xml:
    - What is this package?
    - Who made this package?
    - Where to get this package?
    - Other packages needed?
- CMakeLists.txt
    - Dependencies
    - Message files needed
    - Nodes
    - Services
    - Links
    

When adding new code in /src → add_executable(<NAME OF NODE> src/path.py)

After catkin_make → rosrun <PACKAGE_NAME> <NODE_NAME>

## Messages

```jsx
<MESSAGE_NAME>.msg
```

![Untitled](../../docs/ros/basics/Creating%20Project%20Basics/Untitled%201.png)

## Service files

<aside>
💡 <SERVICE_NAME>.srv

</aside>

![Untitled](../../docs/ros/basics/Creating%20Project%20Basics/Untitled%202.png)

Request

—

Response

## Roslaunch

Run many nodes at the same time

- Make launch folder in package
- <NAME>.launch

![Untitled](../../docs/ros/basics/Creating%20Project%20Basics/Untitled%203.png)

Grouped into multiple namespaces in case of duplicate naming