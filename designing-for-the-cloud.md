# Designing for the cloud

# Short EN

Migrating a legacy application to the cloud can be challenging. The path to
the 12 factor app is not an easy one to take, but can be incredibly rewarding,
even if you end up not deploying in the cloud.

In this talk I'll show you why cloud-readiness and scalability are just
by-products of good design, and how modern architectures like microservices
can be a very good fit with cloud-friendly architectures.

By the end of the presentation you will be able to:

 - rethink state in your web applications to ease scalability
 - handle files at scale with file storage APIs
 - split your services with message queues
 - handle persistent connections like websocket at scale

# Commentary EN


I've helped quite a few customers going from a legacy setup to a cloud
deployement.  This talk is a recap of the advice I usually give, plus a way to
show that these modifications are not constraints but that they are overall
good design.

HTTP is stateless by its very nature, so a stateful HTTP service is the result
of hidden dependencies to state. Moving to a cloud setup forces you to expose
and manage these dependencies, but that's something you should do anyway.

# History

Internal presentations in several startups (2015 & 2016)
ScaleConf NZ 2016 (Pending)
