

## ARTICLES 
https://pyxis-studio.com/fr/cqrs-event-sourcing/

https://ookami86.github.io/event-sourcing-in-practice/#event-sourcing-advantages/01-all-advantages.md

https://ookami86.github.io/event-sourcing-in-practice/#further-reading-1.md
https://ookami86.github.io/event-sourcing-in-practice/#further-reading-2.md

https://www.future-processing.pl/blog/cqrs-simple-architecture/

http://danielwhittaker.me/2014/11/15/aggregate-root-cqrs-event-sourcing/

## CONS

https://www.linkedin.com/pulse/ugly-event-sourcing-real-world-production-issues-dennis-doomen/









Tu lis trop le ppt
Ppt trop verbeux
Manque une transition entre cqrs et le monde n tier. Lexplication sur le pk le cqrs est la reponse est un peu trop rapide/succinte


Finalement, quel est le lien entre cqrs et eventsourcing? sont-il disociable?
Manque transtiion entre ES et aggregate
Manque archi global ES avec example a lappui. + montrer avec le meme example que c’est shitty en n-tier. 
ES bonus point pas necessaire.
De maniere general, c’est bcp trop theorique tout ca! Need un exemple concret tout le long.
Idempotency.ordering => on comprends rien, confus.

All Db sucks => typo
The event store => replace “required” by “possible”
Can go wrong? => c’est pas correct. 


=> Grosso modo: avoir un example fil rouge que tu peux utiliser tout au long de la presentaiton. Ne pas hesiter a re-expliquer les trucs techniques comme aggregats, stream, etc. ne pas oublier que les gars n’y connaissent rien!













# 

layout: false
.left-column[
  Summary
  ## N-Tiers
  ## C.Q.R.S.
]
.right-column[
  ## Command & Query Responsibility Segregation
  - What is a Command ?
  - What is a Query ?
  - Why separate them ?
  

  ## Where does it apply
  - In a single object.
  - In a database.
  - System wide scale.


  ## How to do it wrong ...
  - Log shipping
  - Double writes
]



layout: false
.left-column[
  Summary
  ## N-Tiers
  ## C.Q.R.S.
  ## Event Sourcing
]
.right-column[
  ## Store the log, project the state
  - What is an Event ?
  - Aggregates & Streams
  - Event Store
  - Projections


  ## Magic features
  - Super specialized read models
  - Audit for free
  - Business trace for free
  - Time machine 
  - Easy to scale


  ## Can go wrong ?
  - Checkpoints / Idempotency
  - Ordering
  - Eventually consistent / Eventual consistency
  - Split brain
  - Versioning events
]

