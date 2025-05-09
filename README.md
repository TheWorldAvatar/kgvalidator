# The World Avatar (TWA) KG Validator
An agent developed for validating constraints defined using the Shapes Constraint Language (SHACL) to validate restrictions imposed on ontologised data represented in RDF or its variations such as OWL, Turtle and JSON-LD.

## How to run the TWA KG Validator
1. **Build the project using Maven:**
   Run the following maven command to build the code and generate a JAR file:
    ```bash
    mvn clean install -DskipTests
    ```

2. **Navigate to the `target` folder:""
    ```bash
    cd target
    ```

3. **Run the the JAR file:**
    ```bash
    java -jar shacl-validation-agent.jar
    ```

4. **Return to the root project directory:**
    ```bash
    cd ..
    ```
5. **Open the HTML interface:**
   Either double-click the `index.html` or run:
    ```bash
    start index.html
    ```
6. **Load a knowledge graph:**
   In the browser, click the `Choose File` button and select the file `./data/kg.ttl` file.

7. **Load the SHACL constraints:**
   Click the second `Choose File` button and select the file `./data/shacl_constraints.ttl` file.

8. **Validate the knowledge graph:**
   Click the `Validate` button to check whether the knowledge graph satisfies the defined SHACL constraints.

# Authors #
Hanif Seddiqui (mhs62@cam.ac.uk), Feroz Farazi (msff2@cam.ac.uk), 09 May 2025
