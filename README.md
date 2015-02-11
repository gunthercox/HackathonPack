Hackathon Pack
--------------
Hackathons are difficult and by reading this you can learn what a hackathon is,
how they work, and what you can expect to find when hacking at one.

This guide is set up in a question and answer format, and is designed to give an
answer to most questions you will have about hackathons. We currently have
answers to the following questions, and are interested in adding more.

**[General](#general)**

- [What is a hackathon?](#what-is-a-hackathon)
- [Where can I find hackathons?](#where-can-i-find-hackathons)

**Team building**

- Do I need a team?
- What if I want to fly solo?
- What makes a good team?
- How do I find additional members?

**Getting there**

- Can't I just drive myself?
- I'm broke, how can I possibly go?

**[The day before](#the-day-before)**

- [What should I pack?](#what-should-i-pack)

**The day of**

- What is the typical schedule?
- Who are companies that sponsor hackathons?
- What is swag / what is given out?

**[Creating the hack](#creating-the-hack)**

- [Where should I put my code?](#where-should-i-put-my-code)
- [What should I watch out for?](#what-should-i-watch-out-for)
- [Someone committed passwords! How can I remove them?](#removing-sensitive-information)

General
=======

What is a hackathon?
--------------------
> "The word "hackathon" is a portmanteau of the words "hack" and "marathon",
> where "hack" is used in the sense of playful, exploratory programming, not its
> alternate meaning as a reference to computer crime." A hackathon is a time and
> a place for you to make something. Doesn’t matter if it’s a web app, a mobile
> app, a desktop app, or something in between.

> -- [HackRPI website][hackrpi] and [Wikipedia][wikipedia-hackathon]

Where can I find hackathons?
----------------------------
There are many hackathons running every weekend, but unfortunately they are not
all in one place. For students in universities in the United States,
[Major League Hacking (MLH)][mlh] provides information on hackathons based on
where they fall within university semesters. In order to attend a MLH-sponsered
hackathon, you must be a student who is either attending a university, or
sometimes a student in a secondary school such as a high school.

For those looking for hackathons outside of the United States, or hackathons
that are not directly associated with universities,
[Hacker League][hacker-league] also sponsors hackathons hosted in both the
United States and internationally. Hacker Leauge also provides information on
hackathons hosted during the summer and hackathons not directly associated with
a university, but instead associated with an external company or cause.

The day before
==============
The day before the hackathon, you should make sure that you have done the following.

1. Create an account on ChallengePost
2. Print a few copies of your resume
3. Pack your bag

In preparation for a hackathon, you should attendees create an account on
[ChallengePost][challengepost]. ChallengePost is where MLH tells hackathons
to handle submissions and many hosts will handle their judging through this
website.

What should I pack?
-------------------
- **A laptop** that you can hack on (*many hackathons provide extra laptops in
the hardware you can borrow*).
- **Power cables and adapters** for your laptop and any devices you may be
bringing.
- **An ethernet cable** - Wireless access points may become unavailable due the
the number of people connecting to them. Be sure to bring an ethernet cable to
connect to the internet with.
- **A large backpack** that can store all of the devices you are bringing as
well as any swag that you accumulate throughout the hackathon.
- Hygiene items (toothbrush, toothpaste, deodorant, etc.)
- **Comfortable clothing**, you never know what it is going to be like in the
hacking spaces.
- **A pocket folder** with about 10 to 20 copies of your resume.
- **A flash drive** to share files in case sharing them wirelessly isn't an
option.
- **Head phones or earbuds**, the hacking arena can get rather noisey. If your
project ends up using sound in any way it may be a challenge to hear it on your
laptop's speakers. These may also be usefull if you just decide you want to
listen to mucic.

Many of the sponsors who go to hackathons are actively recruiting new employees
or interns. A hackathon can be a great way to get an internship with a company
or get a job and start your career.

Creating the hack
=================
When you're at the hackathon, you will get the chance to meet with sponsors and
learn about what APIs, development tools, and hardware kits they are providing.

Where should I put my code?
---------------------------
This document lives on [GitHub][github], which is a web-based Git hosting
service. There are many other code sharing services out there, like
[Bitbucket][bitbucket] from Atlassian and [CodePlex][codeplex] from Microsoft.
For a hackathon, your team should decide if the project you create will be open
source or private. Most Git hosting services are free for open source projects,
but GitHub requires a paid plan for private projects and CodePlex does not allow
them. Bitbucket allows you to create private projects for free, which allows
enough people for a standard hackathon team.

GitHub also provides [a student developer pack][github-education] that provides
students with free private repositories. The student developer pack also
includes a list of other services that are available to students, many of which
can be useful during hackathons.

What should I watch out for?
----------------------------
If it is your first time at a hackathon, and even if you have been to many
hackathons before, it is useful to know what to watch out for when creating your
hack. We encourage those who have been at hackathons to improve this section (or
the entire guide) with quick tips for those starting out.

1. **Keep it small** - The larger the hack, the longer it is going to take.
You're not there to make a startup, you're there to make a hack.
2. **Make it look good** - You're going to be presenting your hack to others,
polish it up and make it visually appealing.
3. **Look at the sponsors** - Many sponsors will provide hardware or APIs that
you can use, and some even provide the prizes.
4. **Have a plan** - Don't go into a hackathon blind, have an idea of what you
are interested in creating.

Removing sensitive information
------------------------------
You've been creating your hack that uses an impressive third-party API, and you
notice that your API keys are sitting out in the open in your public repository.
Accidents happen, but make sure to remove the keys as soon as possible and more
importantly: generate new ones.

You should never commit keys, passwords, or any other private data to your
repository. Even if it is private, you should still avoid doing it as removal
requires rewriting history and still leaves you in a tough spot.

The first thing you should do when you discover that sensitive information has
been committed to your repository is **invalidate the key or change the
password**. This will ensure that even if someone was able to record the
sensitive information, they will not be able to use it.

Once you have generated new keys and changed your passwords, you should remove
the information from the past commits. Git allows you to rewrite history, along
with most other source control systems, and GitHub provides
[an excellent guide][github-sensitive-data] on removing sensitive information
from your repositories. If the change was recently committed or the repository
does not have many commits, which is typical for a hackathon, you can quickly
remove the information by [amending the commit][amending-commits] after deleting
it.

In order to prevent committing sensitive information, it is best if you put the
sensitive information in a configuration file that is excluded from version
control by a `.gitignore` file. You can distribute the excluded files to your
teammates outside of the repository, and this will prevent anyone from
committing the information.

[amending-commits]: http://stackoverflow.com/q/179123/359284
[bitbucket]: https://bitbucket.org/
[challengepost]: https://challengepost.com
[codeplex]: https://www.codeplex.com/
[github]: https://github.com
[github-education]: https://education.github.com/
[github-sensitive-data]: https://help.github.com/articles/remove-sensitive-data/
[hacker-league]: https://www.hackerleague.org/hackathons
[hackrpi]: http://www.hackrpi.com/
[mlh]: https://mlh.io/
[wikipedia-hackathon]: https://en.wikipedia.org/wiki/Hackathon
