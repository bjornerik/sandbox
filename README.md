Bep's sandbox
=============
This is a sandbox. The stuff hidden here should work, it should contain some interesting stuff - but it is a sandbox, and as so should be considered experimental.

/grails
-------

### /collection-or-not

A small Grails project to test out GORM modelling (Hibernate) 1-many-realationships with and without use of Collection on the 1 side.

Inspired by this blog post: https://mrpaulwoods.wordpress.com/2011/02/07/implementing-burt-beckwiths-gorm-performance-no-collections/

On my i7 Ubuntu desktop with 6 gigs of ram and the citizen number set to 10000:

	00438  001%  Creating Japan With Collection
	16928  037%  Adding the first 10000 citizens to Japan With Collection
	11202  025%  Adding one more citizen to Japan With Collection
	00050  000%  Creating Japan Without Collection
	15901  035%  Adding the first 10000 citizens to Japan Without Collection
	00061  000%  Adding one more citizen to Japan Without Collection
	00844  002%  Deleting Japan With Collection
	00164  000%  Deleting Japan Without Collection

The interesting line is the "Adding one more ...".

