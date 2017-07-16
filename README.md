﻿### VisualCode
VisualCode is a developer tool which help to visually compose java code.

Tool converts Java methods to visual blocks which can have multiple input and multiple output ports.
Using Visual Flow editor you connect blocks output and input ports.
Resulting visual flow will be converted to executable Java method.
Resulting method is like any other java method and can be called from ordinary java code.

#### Creating blocks

Let's create simple block.
We start with java static method.

```
	public static double add(double a, double b) {
		return a + b;
	}
```
![ExampleFlow](/docs/images/Simple1CodeView.png)

Next open java source file with ‘Code View’ editor and select Visual View tab.
Now you see visual block.

![ExampleFlow](/docs/images/Simple1CodeViewVisual.png)

#### Creating flow

We start with new java class ExampleFlow and add java stub method.
Next open java file with ‘Flow View’ editor.

![ExampleFlow](/docs/images/Simple1FlowCode.png)

Next select method name and from context menu select ‘Convert to Flow’

![ExampleFlow](/docs/images/Simple1FlowOpenFlow.png)

Resize window to make whole flow visible and you see empty flow.

![ExampleFlow](/docs/images/Simple1FlowEmptyFlow.png)

Rearrange editors to side by side, like this

![ExampleFlow](/docs/images/Simple1FlowSideBySide.png)

Drag ‘add’ block from palette to flow canvas.

![ExampleFlow](/docs/images/Simple1FlowDragNewBlock.png)

Connect flow input port ‘a’ to ‘add’ block input port ‘a’

![ExampleFlow](/docs/images/Simple1FlowStartNewCon.png)

When you drag new connection and your are near enough to target point you will see either green on red glow around the target port. Green means both ports data types are compatible and red means they are not. You should not connect incompatible ports.

![ExampleFlow](/docs/images/Simple1FlowEndNewCon.png)

Connect other ports.

![ExampleFlow](/docs/images/Simple1FlowConnected.png)
#### More complex example

Flow visual view

![ExampleFlow](/docs/images/CalcFlowVisual_15jul2017.png)

Blocks source code

![ExampleFlow](/docs/images/SimpleCodeSource_15jul2017.png)

Block visual view

![ExampleFlow](/docs/images/SimpleCodeVisual_15jul2017.png)

Generated executable code.

![ExampleFlow](/docs/images/CalcFlowGencode.png)





