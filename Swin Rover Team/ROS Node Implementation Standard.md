
### Introduction

This document sets the standard for developing nodes in ROS. The language being used is C++, which allows for greater control of computer hardware at a lower level than the other option (Python). C++ is also better for performance reasons and gives us greater control and flexibility over computer/robotic hardware.

### Convention

I am introducing a convention for our codebase. This helps keep code consistent across the team.

**Class and Struct Names**
- Pascal Case e.g.:
```
class MyClass {};
struct MyStruct {};
```
**Variable Names**
- Camel case for multiple word variables e.g. 
```
int myInt;
std::string myString;
bool b;
```

**Function Names**
- Camel case for function names.
```
void printArray();
void display();
char& getCharacterAt(size_t i);
```

**Pointers and L-Value/R-Value References**
- Pointers and References should be placed after the type, not immediately before the variable/function name e.g. **do**:
```
int* x;
int& y;
int&& z;
```
and don't do:
```
int *x;
int &y;
int &&z;
```

**Indentation**
- TABS! Not spaces.

**Brackets**
- Microsoft Style, brackets on a new/seperate line e.g. **do**: ``````
```
int main(int argc, char** argv)
{
	return 0;
}

```

and don't do:

```
int main(int argc, char** argv) {
	return 0;
}
```

**For Loops**
- Always use the letters i, j and k in that order. For example, if you have nested for loops, use i first, then j in the second for loop and k in the third and final for loop e.g. **do this**:
```
for (size_t i = 0; i < 10; i++)
{
	for (size_t j = 0; j < 10; j++)
	{
		for (size_t k = 0; k < 10; k++)
		{
		
		}
	}
}
```

### ROS Node Implementation Blueprint

Should contain:
- Name for Node
- Basic logging
- More (TBD)

##### BlueprintNode.h

```
// BlueprintNode.h
// Swinburne Rover Team 2025

#pragma once

#include "rclcpp/rclcpp.hpp"

#include <string>

class BlueprintNode : public rclcpp::Node
{
public:
	BlueprintNode(const std::string& nodeName) noexcept;
};
```

##### BlueprintNode.cpp

```
// BlueprintNode.cpp
// Swinburne Rover Team 2025

#include "BlueprintNode.h"

BlueprintNode::BlueprintNode(const std::string& nodeName) noexcept : Node(nodeName)
{
	this->declare_parameter("bp_param", "Blueprint Working!");

	std::string bp_param = this->get_parameter("bp_param").as_string();

	RCLCPP_INFO(this->get_logger(), "%s", bp_param.c_str());
}
```
