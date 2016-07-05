**I Abuse The Term Unit Tests.**

For me a unit test is anything you can run with unit test framework. If you go to Wikipedia you see a massive list of unit test frameworks which cover what would be traditionally called a unit test like a very small piece of code being tested, to integration test, to production tests, to smoke tests everything.

For me if you can run it with a unit test framework it is a unit test. And the key is that once it runs in those frameworks it is something that is repeatable, it is something that can fit into a continuous integration loop, it is something that is replicate able, in a way it is a much better language to communicate between all the parties in a development life cycle.

So the way I look at it is tests are how you should be communicating, unit tests is what you write and I don't particularly care about all the academics about it. A lot of people, especially actually a lot of developers sometimes get quite I would say focused on the fact that a unit test is a very small piece of test. For me, the key definition is unit. So, a unit isn't just a bit of code, a unit is what you are testing. So, sometimes you are testing a little bit of code, sometimes you test a lot of code.

One of the side effects that I see happening with the focus on testing a little bit of code is that you end up creating a lot of mocks. And the mock is basically something that replace or replicates a behavior of the application.

And I don't really like marks, I think mocks can be very dangerous because after a while you start to have to maintain your mocks, your mocks might not represent reality. So the way I look at it is you want to run as much code as possible all the time and it should be fast. So, my benchmark for unit test is milliseconds, anything that runs slower than that is probably doing more than it should be doing at that moment in time. 

So, ideally you want to run as much of your code as possible during your test because it means that the more moving parts you have and this also goes down to the idea that when we measure code covered, we shouldn't be measuring just a bit of code, we should be measuring the overall coverage of the application which basically means that we are touching all sorts of code from all sorts of places. So in fact that is why you don't want the 100%, you want like 5000% which is the topic of another post.