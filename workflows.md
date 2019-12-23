# Creating Plasma Workflows

Plasma workflows are YAML files which can be used to define and edit
your ML workflows with ease. These workflows are used to specify 
the order in which components are executed and the parameters which
are passed to each component.

Sample Plasma Workflow 

```
name: Test Pipeline
description: Sanity check for plasma
version: 0.1
workflow:
    component-1:
       send-message:
           message: Component 1 Executed
    component-2:
       test:
           message: Component 2 Executed

