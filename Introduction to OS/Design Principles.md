# Introduction to Design Principles

- These principles are used to design an operating system.

- While designing an operating system, three elements are kept in mind

- These elements are abstraction, policy and mechanism

- For example, many OS uses LRU to allocate memory. This concept is a policy,
whereas, system calls used by an OS are the mechanism

## Policy

- Policy refers to the set of rules or a plan that must be followed
- Policies are what will be done
- LRU (Least Recently Used), EDF (Earliest Deadline First) etc.

## Mechanism

- Mechanism refers to the method through which a policy is fulfilled
- Mechanism is how to do something
- For ex. create, open, write, allocate, schedule etc.

## Abstraction

- Abstraction refers to the simplification of h/w complexity
- Abstraction includes OS's abstracted form of h/w resources
- For ex. process, thread, file, socket, memory page etc.

## Design Principles needed to be followed

### Policy and mechanism must be separated

- Mechanism should not dictate over the policy and should support multiple policies

- This way we can introduce new policies without breaking existing ones

### Commonly used cases

- We should have answers to questions such as who are the target users, workload
that will be handled and the applications that will run

- Using these answers we can decide on the abstraction, policies and mechanisms

### Macromanage not micromanage

- OS should only interfere/act when it is needed

- For instance, when a system call is made, OS should do the specified work,
then let the application run its process once the system call is completed
