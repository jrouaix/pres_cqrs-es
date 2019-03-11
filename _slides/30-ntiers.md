@title[N-Tiers]
@snap[north] 
## N-Tiers
@snapend

@snap[west splitscreen] 
Front <br /> 
- Present <br />
Back <br />
- Validate <br />
- Execute <br />
Data <br />
- Persist <br />
@snapend

@snap[east splitscreen]
![N-Tiers](_assets/Overview_of_a_three-tier_application_vectorVersion.png)
@snapend


@snap[south-west byline text-06]
Sources : https://en.wikipedia.org/wiki/Multitier_architecture
@snapend

+++
## Some examples
- S.P.A. / Api / Database
- View / Controller / Repository .. Database
- Facade Api / Business Api / Persistance Api .. Database

+++
## FullStack
- What does it mean ?

note: 
- is this because of languages ? Is there a fullheap ?
- is the only way of thinking is in stack ?


+++
## Why it's not enough
- All the calls are directed to the data tiers
- The database, usually a relational one, is hard to scale.
- As the system grows, more and more pressure is added on last tiers : data.

+++
## Read != Write
- Read & Write needs are often not aligned
  * Write : less volumes / transactions
  * Read : more volumes / optional consistancy / aggregations ...

+++
## SOLUTION

- ADD CACHE !
- OR FIND A BETTER DATABASE !

note:
This is the end of the show !

+++
## All databases sucks !
i.e. : not all databases are made equal

+++

![Databases](_assets/DbSkills.png)

