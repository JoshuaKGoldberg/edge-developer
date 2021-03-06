---
ms.assetid: 1c743e65-ba45-4d85-948c-77b424cf24f8
description: Learn how to use new and old features in Microsoft Edge's F12 developer tools.
title: F12 devtools guide
author: erikadoyle
ms.author: edoyle
ms.date: 02/08/2017
ms.topic: article
ms.prod: microsoft-edge
keywords: edge, web development, html, css, javascript, developer
---

# Meet the Microsoft Edge F12 Dev Tools

> [!TIP]
> **[Test on Microsoft Edge free from any browser](https://developer.microsoft.com/en-us/microsoft-edge/tools/remote/)**:
> We partnered with BrowserStack to get free live and automated testing on Microsoft Edge.

Microsoft Edge introduces great new improvements to F12 developer tools, including some of the most requested features from [UserVoice](https://wpdev.uservoice.com/forums/257854-microsoft-edge-developer).  The new tools are built in TypeScript, and are always running, so no reloads are required. In addition, F12 developer tools documentation is now fully available on [GitHub](https://github.com/MicrosoftEdge/MicrosoftEdge-Documentation). From this point on, the docs will not only be influenced by your feedback, but you're invited to contribute and help shape our documentation.

> [!VIDEO https://channel9.msdn.com/Blogs/One-Dev-Minute/Microsoft-Edge-F12-tools/player]

## The F12 tools at work

There are seven distinct tools, each with their own tab in the F12 tools interface. Here you'll find an image of each tool and a quick summary of what it does, followed by lists of its main features and typical tasks.

> Visit the [Settings](./f12-devtools-guide/settings.md) page for more information about how to adjust Developer Settings in Microsoft Edge.

## The DOM Explorer tool (CTRL+1)

> [!NOTE]
> The **DOM Explorer** tool is now called **Elements** in [Windows Insider](https://insider.windows.com/) preview builds. 

[The DOM Explorer tool](./f12-devtools-guide/dom-explorer.md) shows the structure of your webpage as it's being rendered in the browser and makes it possible to edit your HTML and styles in a live page. You can do this without having to edit and reload your sources, so you can quickly solve display issues or experiment with new ideas.
![Microsoft Edge DOM Explorer](./f12-devtools-guide/media/Edge_DOMExplorer.png)

**Features** in the DOM Explorer tool include:
 - IntelliSense autocompletion suggestions when editing HTML attributes and CSS properties.
 - Drag DOM nodes to rearrange them and edit nodes as HTML.
 - Support for compiled CSS sourcemaps.

**Development and debugging tasks it makes easier:**
 - Determining why an element is not displaying at the right place or right size.
 - Figuring out which CSS styles and media queries are being applied to an element.
 - Testing a series of different colors for an element to see which looks best.

[Learn more about the DOM Explorer tool.](./f12-devtools-guide/dom-explorer.md)

## The Console tool (CTRL+2)
![Microsoft Edge Console Tool](./f12-devtools-guide/media/Edge_Console.png)

The [Console tool](./f12-devtools-guide/console.md) provides a way to interact with your running code:

  - Change variable values or inject code into a live site with the Console's command line.
  - Use the [Console Debugging API](./f12-devtools-guide/console/using-the-console-api.md) to send out debug information.
  - See browser error messages and status codes.

**Features** in the [Console tool](./f12-devtools-guide/console.md) include:

  - Open the Console at the bottom of any other tool with the Console button or ``CTRL + ` ``.
  - [Console Debugging API](./f12-devtools-guide/console/using-the-console-api.md) methods for timing, counting, grouping, and more.
  - IntelliSense autocompletion suggestions on the command line speed up input, reduce typos, and help you discover aspects of JavaScript APIs.

**Development and debugging tasks it makes easier:**

  - Targeting specific iFrames.
  - Timing code execution down to the statement with new timing methods.
  - Changing the value of a variable in running code without reloading.

[Learn more about the Console tool.](./f12-devtools-guide/console.md)

## The Debugger tool (CTRL+3)
![Microsoft Edge Debugger Tool](./f12-devtools-guide/media/Edge_Debugger.png)

You use the [Debugger tool](./f12-devtools-guide/debugger.md) to examine what your code is doing, when it's doing it, and how it's doing it. Pause code in mid-execution, step through it line-by-line, and watch the state of variables and objects at each step.

**Features** in the [Debugger tool](./f12-devtools-guide/debugger.md) include:

  - No-refresh debugging. Set your breakpoints and go without reloading and losing state.
  - Tabbed document interface for easier management of multiple scripts.
  - Breakpoints on standard code, XHR responses, and events.

**Development and debugging tasks it makes easier:**

  - Seeing what led to a function call using the Call stack.
  - Making compressed or minified code more readable using source maps.
  - Monitoring web worker creation and execution.

[Learn more about the Debugger tool.](./f12-devtools-guide/debugger.md)

## The Network tool (CTRL+4)
![Microsoft Edge Network Tool](./f12-devtools-guide/media/Edge_Network_details.png)

The [Network tool](./f12-devtools-guide/network.md) gives you the fine details of any network requests involved in the loading and operation of your webpages.

**Development and debugging tasks it makes easier:**
  - Viewing the amount of bandwidth your page consumes across resources.
  - Debugging AJAX requests by viewing request and response headers and bodies.
  - Identifying network requests that slow the loading of your webpages.

[Learn more about the Network tool.](./f12-devtools-guide/network.md)

## The Performance Tool (CTRL+5)
![Microsoft Edge Performance Tool](./f12-devtools-guide/media/Edge_Performance.png)

The [Performance tool](./f12-devtools-guide/performance.md) helps you dig into what is happening when your page slows down. Using it to profile specific points of slowness shows the operations that are causing them. In Microsoft Edge, the Performance tool combines the previous **UI Responsiveness** and **Profiler** tools to create an end-to-end view of your scripting and painting performance.

Some interesting features are:

  - Identifying the different sources of CPU activity causing UI slowness.
  - Insight into your webpage's frame rate and how much repaints and reflows cost.
  - Setting labels on the timeline to isolate user scenarios.

**Development and debugging tasks it makes easier:**

  - Testing code optimizations.
  - Speeding up your webpages.

[Learn more about the Performance tool.](./f12-devtools-guide/performance.md)

## The Memory tool (CTRL+6)
![Microsoft Edge Memory Tool](./f12-devtools-guide/media/Edge_Memory.png)

When a webpage starts out fast and slows down after you use it for a while, the culprit is usually a memory leak. The [Memory tool](./f12-devtools-guide/memory.md) tracks the memory use of your webpage, helping you identify where memory use is growing, why it's growing, and how to fix it.

Some interesting features are:

  - A timeline to see progressive changes in memory use.
  - Snapshots to examine the details of memory use at specific points.
  - Snapshot comparisons to identify specific points of growth.

**Development and debugging tasks it makes easier:**

  - Identifying detached DOM nodes.
  - Identifying points of memory growth.
  - Measuring the memory use of objects.

[Learn more about the Memory tool.](./f12-devtools-guide/memory.md)

## The Emulation tool (CTRL+7)
![Microsoft Edge Emulation Tool](./f12-devtools-guide/media/Edge_Emulation.png)

The [Emulation tool](./f12-devtools-guide/emulation.md) helps you test how your webpages run on different screen sizes and hardware features, and how they respond to different user agent strings.

Some interesting features are:

  - Emulating different screen sizes and resolutions.
  - GPS simulation.

**Development and debugging tasks it makes easier:**

  - Testing responsive designs on multiple screen types.
  - Testing location-aware features for a mobile site.

[Learn more about the Emulation tool.](./f12-devtools-guide/emulation.md)
