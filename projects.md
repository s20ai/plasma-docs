# Plasma Projects

Plasma allows users to create 'projects' to group their code, resources, workflows etc
under a common name.

The directory structure of a plasma project

```
project-directory
	├── .plasma.json
	├── components/
	├── data/
	├── logs/
	├── models/
	└── workflows/
```


## Usage 

Users can create new projects and load existing projects using the Plasma CLI.

### Creating a Plasma Project 

```
plasma project create <project_name>
```

### Loading a Plasma Project

```
plasma project load <project_path>
```


## Directories 


#### .plasma.json

The .plasma.json file is a hidden file which contains project metadata including 
the paths of all project directories.

#### components

The components directory contains all the components used by the workflows in your
project. Projects downloaded through the package-manager are also automatically 
extracted in this directory. All custom components created by the user need to be
stored here too.

#### data

The data directory is used to store temporary file generated during workflow execution.
The user can also store this directory to explicitly store intermediate files created
during workflow execution.

#### logs

The logs directory stores logs from workflow executions. Users can view these log files
in order to debug their workflow.

#### models

The models directory stores all the models generated during workflow executions.

#### workflows 

Users are required to store all of their YAML defined workflows in this directory in order
to enable plasma to find and execute them.


