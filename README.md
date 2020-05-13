# ToDoApp
Simple To Do App using Blazor WebAssembly

Tested on:
dotnet - 3.1.300-preview-015135
Visual Studio 16.6.0 Preview 6.0

Main idea of this ToDo component is to test the Drag and Drop events with Blazor.

Here are the outstanding issues:

1) When dragging a lot we get a GC_MINOR: (Nursery full). This has to be debugged and fixed. This is probably the most important optimization that should be performed.

2) Make the component not use any javascript at all (only Blazor)
   The only javascript we rely on for now is this:
   ondragstart="event.dataTransfer.setData('', event.target.id);"

3) Make Cards Editable

4) Make Cards Keep and Switch Positions

5) Wrap into own Component

6) Possibly publish to NuGet
