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

#### Bounded Context

---

> A bounded context is a set of tiny services (API, Background Jobs, Serverless Functions, etc) that work together to deliver requirements related to a sub-domain of a large software
> Technically speaking, the Bounded Context in DDD-speak is a specific boundary within your domain that your Glossary from your Ubiquitous Language can only apply – the idea being that different Subdomains may have competing or conflicting definitions of terms
> A Bounded Context is a system that fulfills the goals of the business in the real world.
> Any of our software systems (like a web service or web app) that operate as concrete instances in the Real World are considered Bounded Contexts
> one of the goals of Domain-Driven Designs is to have a one-to-one mapping from a Subdomain to a Bounded Context.

#### Ubiquitous Language

> Words often have different meanings in different contexts
>
> The word “meter” had different meanings in different parts of the organization. In one department, it referred to the connection between the grid and a location. Others understood “meter” as the connection between the grid and the customer, or, of course, a physical meter attached to a house to measure electrical consumption.
>
> Different stakeholders might represent the same business entity in different models. For example, an Advertising Campaign is a complex entity with many rules and invariants for campaign managers; but for sales agents, an Advertising Campaign is merely a data structure that describes a subset of its metadata. Those are two different models, and thus belong to two different Bounded Contexts.
### Challenges

---

- Team Work
- Meetings!, Meetings!......

### References

---

- Domain Drive Design By Eric Evans , 2003
- Patterns, Principles and Practices Of Domain Driven Design By Scott and Nick Tune 2015
- VirtualDDD Meetup (virtualDDD.com)
- https://hackernoon.com/microservices-bounded-context-cohesion-what-do-they-have-in-common-1107b70342b3
- https://vladikk.com/2016/04/05/tackling-complexity-ddd/
- https://hackernoon.com/microservices-bounded-context-cohesion-what-do-they-have-in-common-1107b70342b3
- https://blog.carbonfive.com/2016/10/04/ubiquitous-language-the-joy-of-naming/
- https://blog.carbonfive.com/2016/11/01/bring-clarity-to-your-monolith-with-bounded-contexts
