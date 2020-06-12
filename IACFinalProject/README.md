# Summary of project

Your company is creating an Instagram clone called Udagram. Developers pushed the latest version of their code in a zip file located in a public S3 Bucket.

This needs to be done in an automated fashion so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.
We will be deploying the application, along with the necessary supporting software into its matching infrastructure. We will deploy an application (Apache Web Server) and you also pick up code (JavaScript and HTML) from S3 Storage and deploy it in the appropriate folder on the web server.

# Phases of the Project
*  Provide visual aid of the architecture so that that the team is aware of the components
* Create a cloud formation script to materialize the visual aid

# How to run the Cloud formation scripts

### Prerequisites

All the cloudformation scripts are being run from a windows machine. Hence a .bat file has been created as a wrapper to create, update and delete the stack

To create stack:
```bash
./create.bat <stackname> <yamlfile> <jsonparameter>
```
To modify stack:
```bash
./update.bat <stackname> <yamlfile> <jsonparameter>
```

To Delete stack:
```bash
./delete.bat <stackname> 
```

# Files in the repository

* **[Udagram_Architecture.pdf](./Udagram_Architecture.pdf)**:  Architecture diagram of the implementation.
* **[create.bat](./create.bat)**:  Batch wrapper script for creating the stack.
* **[update.bat](./update.bat)**:  Batch wrapper script for creating the stack.
* **[delete.bat](./delete.bat)**:  Batch wrapper script for creating the stack.

* **[final-project-network.yml](./final-project-network.yml)**:  YAML script to create the Network components.
*  **[final-project-server.yml](./final-project-network.yml)**:  YAML script to create the Server components.

* **[final-project-network-parameter.json](./final-project-network-parameter.json)**:  JSON parameter to create the Network components.
*  **[final-project-server-parameter.json](./final-project-server-parameter.json)**:  JSON parameter to create the Server components.



# End result of project
Provide customer a secured application to access the required web services via internet.