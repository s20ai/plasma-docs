# Plasma component manager

Plasma comes with an in-built component management tool which allows users to
search an online repository of components. These components can also be downloaded 
using the Plasma CLI and then be used in Plasma Workflows.

## Usage

Plasma CLI component operations

plasma component 
	├── list
	├── search
	├── get
	└── describe


#### list
The list operation prints a list of all local components. Both downloaded
and user defined components will be displayed.

```
plasma component list
```

### search
Search allows users to serach for components on plasma's online component
repository.

```
plasma component search <query>
```

### get 
Get allows users to download components from plasma's online component
repository. Downloaded components are automatically extracted and moved to
the projects component directory.

```

plasma component get <component_name>
```
### describe
The Describe operation prints a short description of the component, and its
usage instructions.

```
plasma component describe <component_name>
```

