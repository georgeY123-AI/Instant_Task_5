 ### Task 5

1. What is the difference between Red-Black Tree and AVL Tree?
2. What is the difference between a Lambda Function, Inline Function, and Anonymous Function?
3. Is `struct` in C the same as `class` in C++? Can I inherit from another `struct` in C? What are the advantages of `class` in C++ over `struct` in C?
4. What is the importance of decorators in Python?
5. What is SQL Injection?
6. What is Extreme Programming?
7. What are DevOps tools, which companies use these tools, and what are the most popular tools used in companies?
8. What are DataOps tools?
9. What are MLOps tools?

### Task 4 Answers

1. **Difference between Red-Black Tree and AVL Tree**

**Red-Black Tree**:
- **Properties**: Each node is colored either red or black. The tree maintains balance through a set of rules involving node colors and rotations.
- **Balancing**: Less strictly balanced compared to AVL trees, allowing faster insertion and deletion operations.
- **Time Complexity**: O(log n) for search, insert, and delete.
- **Use Case**: Preferred in situations where insertions and deletions are more frequent, as it allows for faster modifications.

**AVL Tree**:
- **Properties**: Height-balanced binary search tree where the difference between heights of left and right subtrees cannot be more than one for all nodes.
- **Balancing**: More strictly balanced, resulting in faster lookups but slower insertions and deletions due to more frequent rotations.
- **Time Complexity**: O(log n) for search, insert, and delete.
- **Use Case**: Suitable for read-heavy applications where searches are more frequent than updates.

2. **Difference between Lambda Function, Inline Function, and Anonymous Function**

**Lambda Function**:
- **Definition**: A small, anonymous function defined with the lambda keyword.
- **Use Case**: Typically used for small, throwaway functions without a name.
- **Example in Python**: `lambda x: x + 1`

**Inline Function**:
- **Definition**: A function defined with the `inline` keyword in languages like C++.
- **Use Case**: Suggests to the compiler to insert the function's body where it is called, to reduce function call overhead.
- **Example in C++**:
  ```cpp
  inline int add(int a, int b) {
    return a + b;
  }
  ```

**Anonymous Function**:
- **Definition**: A function without a name, often used in the context of lambda functions.
- **Use Case**: Used for short-term use where defining a full named function would be unnecessary.
- **Example in JavaScript**:
  ```javascript
  const add = function(a, b) {
    return a + b;
  };
  ```

3. **Is `struct` in C the same as `class` in C++? Can I inherit from another `struct` in C? What are the advantages of `class` in C++ over `struct` in C?**

**Struct in C**:
- **Capabilities**: Can hold multiple data types but lacks member functions and other advanced features.
- **Inheritance**: C does not support inheritance for structs.

**Class in C++**:
- **Capabilities**: Can contain data members and member functions, support inheritance, polymorphism, encapsulation, and access specifiers (public, private, protected).
- **Advantages Over C Struct**:
  - Inheritance: Classes can inherit from other classes.
  - Encapsulation: Control access to data using access specifiers.
  - Member Functions: Can have functions that operate on the data members.
  - Polymorphism: Support for function overloading and virtual functions.

4. **What is the importance of decorators in Python?**

**Decorator**:
- **Definition**: A design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure.
- **Use Case**: Used for logging, authorization, instrumentation, caching, etc.
- **Example**:
  ```python
  def my_decorator(func):
      def wrapper():
          print("Something is happening before the function is called.")
          func()
          print("Something is happening after the function is called.")
      return wrapper

  @my_decorator
  def say_hello():
      print("Hello!")

  say_hello()
  ```

5. **What is SQL Injection?**

**SQL Injection**:
- **Definition**: A code injection technique that exploits vulnerabilities in an application's software by inserting malicious SQL statements into an entry field for execution.
- **Impact**: Can lead to unauthorized access to database contents, data modification, and even deletion of data.
- **Prevention**: Use parameterized queries, prepared statements, and proper input validation.

6. **What is Extreme Programming?**

**Extreme Programming (XP)**:
- **Definition**: An agile software development methodology aimed at improving software quality and responsiveness to changing customer requirements.
- **Practices**: Includes practices like pair programming, test-driven development, continuous integration, and frequent releases.
- **Goal**: To improve software quality and adapt to changing requirements efficiently.

7. **What are DevOps tools, which companies use these tools, and what are the most popular tools used in companies?**

**DevOps Tools**:
- **Common Tools**:
  - **Version Control**: Git, GitHub, GitLab
  - **CI/CD**: Jenkins, CircleCI, Travis CI
  - **Configuration Management**: Ansible, Chef, Puppet
  - **Containerization**: Docker, Kubernetes
  - **Monitoring**: Prometheus, Nagios, Grafana
  - **Collaboration**: Slack, Microsoft Teams, Jira
- **Companies**: Most tech companies including Google, Amazon, Facebook, Netflix, and others use DevOps tools to streamline their development and operations processes.

8. **What are DataOps tools?**

**DataOps Tools**:
- **Definition**: Tools used to improve the communication, integration, and automation of data flows between data managers and data consumers across an organization.
- **Common Tools**:
  - **Data Integration**: Apache NiFi, Talend
  - **Data Orchestration**: Apache Airflow, Prefect
  - **Data Quality**: Great Expectations, Deequ
  - **Data Monitoring**: Datadog, Splunk
- **Goal**: To ensure the smooth and efficient handling of data pipelines and data lifecycle management.

9. **What are MLOps tools?**

**MLOps Tools**:
- **Definition**: Tools used to deploy and manage machine learning models in production reliably and efficiently.
- **Common Tools**:
  - **Version Control**: DVC, MLflow
  - **Model Serving**: TensorFlow Serving, TorchServe, Seldon
  - **Monitoring**: Prometheus, Grafana, Neptune.ai
  - **Pipeline Orchestration**: Kubeflow, Airflow
- **Goal**: To streamline the process of deploying, monitoring, and maintaining machine learning models in production environments.
