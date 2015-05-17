Last Tuesday, I participated in an online panel on the subject of [Build Automation](http://electric-cloud.com/blog/2015/05/continuous-discussions-c9d9-episode-16-recap-build-automation/) as part of Continuous Discussions (#c9d9), a series of community panels about Agile, Continuous Delivery and Devops. Automating the build pipeline has many challenges, including third party dependencies, build version management and especially culture, and panelists discussed real-life experiences addressing these challenges.

Continuous Discussions is a community initiative by [Electric Cloud](http://electric-cloud.com/powering-continuous-delivery/), which powers Continuous Delivery at businesses like SpaceX, Cisco, GE and E*TRADE by automating their build, test and deployment processes.

Below are a few soundbites from my contribution to the panel.

What do build bottlenecks mean for your pipeline?
=================================================

In my experience, bottlenecks are usually related to the architecture of the software more than tools and teams. I think most are not ready to architect software in a way that it can be built, tested and deployed fast and easily.

We need to start breaking things up into very small pieces. That’s the easiest towards removing bottlenecks. Big is bad, small is good. If we want to deliver fast, with no downtime, with ability to rollback when things go wrong and if we want to do that often, we need to architect software in a way that we can deliver what was changed not the whole system at once. Microservices and containers with Docker opened new doors that were closed to most of us until recently.

For a long time we tried to build pipeline around monolithic architecture and now it is time to start building architecture in a way that it supports continues delivery. 

What are some common problems?
==============================

The problem is that there are teams, but there is no personal responsibility. The world changed with Docker and micro services, which made it possible for me to take full responsibility for everything I do, instead of passing it to operations, testers, and other teams. When it is passed on to other teams, the job of DevOps is just to make sure that the repository is built and that the build goes to production. DevOps does not decide what is built or how it’s built; they simply push everything to production. And that’s hard because things go wrong and then people stop taking responsibility. To solve this problem, we need to break down the software into small units.

Many organizations are moving towards micro services. When everything is smaller, deployment can be done daily. As long as your architecture does not prevent it and as long as your teams are capable of completing the job. If you need to rely on someone else for things to be done, then you have a bottleneck.

We need the power to be in the hands of developers. All the other members of the organization should be in support of development. And once we change that culture then things can go more smoothly and run faster.

What do you think about consistency and standardization in the process?
=======================================================================

Standardization would be great if it wouldn't be the biggest innovation killer. Once you standardize, you are stuck with something for many years.

I don’t see anything wrong with people trying new approaches, especially if you break your application into smaller pieces. You can try it out on a tiny part of your system with little code; that isn’t too hard to learn. In any organization I ever worked for, the more standardization, the less changes and innovation were introduced. In my experience, standardization is inversely related to innovation.

Some standardization is important, especially about how to receive communication from outside. But within a team, there is no one better suited to decide how the team should work than the team itself, assuming that the team is a reasonable size.

Regardless of what we are working on, we need to be very tough on contracts about communication between the components. But whatever is going on inside a component I develop is my problem and I can solve it the best way I can as long as no one from the outside is interfering too much.”