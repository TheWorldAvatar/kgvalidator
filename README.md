# The World Avatar (TWA) KG Validator
An agent developed for validating the conformance of ontologised data (knowledge graph) represented in RDF or its variations such as OWL, Turtle and JSON-LD to constraints defined using the Shapes Constraint Language (SHACL).

---
## How to run the TWA KG Validator
### 1. **Build the project using Maven:**
Assuming that you already have Maven and JDK 11 installed on your computer. Run the following maven command to build the code and generate a JAR file:
```bash
mvn clean install -DskipTests
```

### 2. ** Run the validator**

#### 2.1 **From your code**
Run the JAR file with the knowledge graph file path and SHACL constraints file path:
```bash
java -jar ./target/shacl-validation-agent.jar <knowledge graph file path> <SHACL constraints file path>
```
For example,
```bash
java -jar ./target/shacl-validation-agent.jar ./data/MatPassportChassisCrossbeamKnowledgeGraph.owl ./data/shacl_constraints.ttl
```
Run the above command from within your knowledge graph generation code to check conformance.
Go to **step 7** for validation results.
	
#### 2.2 **Manually**
Run the the JAR file:
```bash
java -jar ./target/shacl-validation-agent.jar
```

### 3. **Open the HTML interface:**
Either double-click the `index.html` or run:
```bash
start index.html
```

### 4. **Load a knowledge graph:**
   In the browser, click the first `Choose File` button and select `./data/MatPassportChassisCrossbeamKnowledgeGraph.owl`.

### 5. **Load the SHACL constraints:**
   Click the second `Choose File` button and select `./data/shacl_constraints.ttl`.

### 6. **Validate the knowledge graph:**
   Click the `Validate` button to check whether the knowledge graph satisfies the defined SHACL constraints.

### 7. **Interpret the Result**
   The validator returns `true` if the knowledge graph conforms to the SHACL constraints. Otherwise, it returns `false` along with an explanation of the violations.

## Authors

---

- **Hanif Seddiqui** (mhs62@cam.ac.uk)  
- **Feroz Farazi** (msff2@cam.ac.uk)  
*Date: 09 May 2025*
