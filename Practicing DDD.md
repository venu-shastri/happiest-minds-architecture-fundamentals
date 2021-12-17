#  What is DDD

`Domain Driven Design` is an approach to software development that centers the development on programming a domain model that has a rich understanding of the processes and rules of a domain

-- Martin Fowler

## High Level Understanding of DDD

- Interaction with `Domain Experts`
- Model `Single SubDomain` at a  time
  - Divide and Conquer
- DDD is about Solving Problems and Not Just Coding
- Gives Efficient and Effective Path to Project Success

# Practicing DDD

The  basic philosophy of the primacy of domain terminology can be distributed across three guiding principles

- **Capture the domain model, in domain terms, through interactions with domain experts.**

  > To put it another way, talk to the individuals in the businesses where you're solving problems and try to understand them from their perspective first. This is how you establish the domain's universal language and lay the groundwork for harmonious models.

- **Embed the domain terminology in the code**

  > This includes naming classes, methods, commands, and, most importantly, domain events in the manner that a domain expert would. This is how the domain model is reflected in the code.

- **Protect the domain knowledge from corruption by other domains, technical subdomains, etc.**

  > If you find that your code is talking about two different things—for example, the domain solution and the technical implementation—separate those components to keep the subdomains separate. This strategy tends to produce classes with single responsibilities and a terse, focused vocabulary. Put "translators" at the boundaries between subdomains to keep them from relying on each other's structures unnecessarily, and to prevent the meaning of domain terms from becoming ambiguous.



### Challenges

---

- Team Work
- Meetings!, Meetings!......

### References

---

- Domain Drive Design By Eric Evans , 2003
- Patterns, Principles and Practices Of Domain Driven Design By Scott and Nick Tune 2015
- VirtualDDD Meetup (virtualDDD.com)