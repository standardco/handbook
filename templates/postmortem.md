# Post Mortems

A post mortem is an important part of learning from things that blow up on us. We're human which means things *will* break. That's ok. What we want to do is memorialize these screw ups so we can avoid them in the future. We do that through a post mortem.

## When to create a post Mortem

There's no hard and fast rules for when to create a post mortem. If there's an outage, a release went live that broke the entire website, you rolled out the same bug multiple times are all good use cases for a post mortem.


## The error log

For smaller issues that don't really rise to the level of a post mortem, we have an [error log](https://docs.google.com/spreadsheets/u/1/d/1SIINVUhOUWtXOmwim5KVp0BUsd8s1OInH4cJGCuuHVI/edit#gid=0). Put it there. 

## Ok, get on with it!

Copy and paste the below into a google doc and share with TJ, Jared, and Jonathan:

**Background of Issue**

[specificity is key -- nail down dates / times as accurately as you can. this way we can diagnose outage time]
On Dec 20th at 2:00am EST we install blah blah blah. At 5:00am EST we noticed site slowness. Client contacted us blah blah blah

**Steps taken to fix the issue**

[what exact steps did you take to try and fix the issue. what was the ultimate resolution?]
we did this. then we tried this. and then we did this other thing. we finally had to roll back.

**Current state**

[where are we now? is it fixed?]
we had to roll back to pre dec 20th

**How we'll avoid this in the future**

[probably the most important part of a post mortem. what we'll do next time to avoid this]
next time we'll make sure the EC2 instance is using elastic ip. this will negate any downtime or whatever
