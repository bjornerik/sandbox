Bep's sand box
=============
This is a sand box. The stuff hidden here should work, it should contain some interesting stuff - but it is a sand box, and as so should be considered experimental.

/grails
-------

### /collection-or-not

A small Grails project to test out GORM modelling (Hibernate) 1-many-realationships with and without use of Collection on the 1 side.

Inspired by this blog post: https://mrpaulwoods.wordpress.com/2011/02/07/implementing-burt-beckwiths-gorm-performance-no-collections/

Creation of 1000 then one child gives currently these results with a HSQLDB file-db running on my Dell laptop:

	01445  007%  Creating Japan With Collection
	06158  031%  Adding the first 1000 citizens to Japan With Collection
	02106  010%  Adding one more citizen to Japan With Collection
	00277  001%  Creating Japan Without Collection
	10089  050%  Adding the first 1000 citizens to Japan Without Collection
	00011  000%  Adding one more citizen to Japan Without Collection

On my i7 Ubuntu desktop with 6 gigs of ram and the citizen number set to 10000:

	00463  000%  Creating Japan With Collection
	17292  007%  Adding the first 10000 citizens to Japan With Collection
	11419  005%  Adding one more citizen to Japan With Collection
	00044  000%  Creating Japan Without Collection
	209856  088%  Adding the first 10000 citizens to Japan Without Collection
	00027  000%  Adding one more citizen to Japan Without Collection

