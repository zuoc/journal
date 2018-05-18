# A Letter to /r/python (with some notes about bipolar disorder)

There were a few recent threads that occurred in [/r/python](https://reddit.com/r/python) which greatly disturbed me, because of their general tone towards both me, and a tool that I’ve been toiling on very hard over the past year and a half.

Threads:
- [Why is pipenv the recommended packaging tool by the community and PyPA?](https://www.reddit.com/r/Python/comments/8jd6aq/why_is_pipenv_the_recommended_packaging_tool_by/) (very negative)
- [Pipenv review, after using it in production](https://www.reddit.com/r/Python/comments/8jhtkh/pipenv_review_after_using_it_in_production/) (mostly great!)
- [Kenneth Reitz - Pipenv: The Future of Python Dependency Management - PyCon 2018](https://www.reddit.com/r/Python/comments/8jfmv8/kenneth_reitz_pipenv_the_future_of_python/) (mostly positive, some negativity)

I mention negativity, because it sprung forth from some of these threads in a very aggressive manner, from some very (in these threads) vocal members of the **/r/python** community. It appears I have some haters out there. This is new to me.

One comment, for example, struck me as extremely odd:

> If only these people didn't advertise themselves as the next best thing to sliced bread, collecting undeserved fame, jobs, influence, and as consequence harming very large number of people and technology in general, I wouldn't mind them doing whatever projects they like.

My response to this comment is — first off, my fame, while certainly categorized under “cult of personality” is not necessarily accidental. It’s called *marketing*. I worked very hard at becoming well known within the Python community, and toiled away at it for years. The popularity of [Requests](https://python-requests.org) was accidental, but there were many libraries that existed before it that I had created in an attempt to get GitHub stars. I wanted to be like [Armin Ronacher](https://github.com/mitsuhiko) on GitHub. I succeeded.

Also, for the past 6.5 years, I have not had the most glorious job in the world. I consider myself to have been mildly underpaid, considering what I was responsible for — *the entire deployment experience (including uptime) of Python apps on Heroku, one of the largest deployment platforms in the world*.

Also, “harming a very large number of people”? What? I’ve never harmed a soul with my influence — I use it to build the community up. I’m not \<insert an obvious name here\> from the Social Justice Warrior League. I’m Kenneth — a nice guy who builds nice tools and takes a lot of pictures.

So, this comment is just off the rails, and deeply disturbs me.

Another quote from one thread:

> Pipenv is garbage.

There are a few things I’d like to say:

- Thank you, **/r/python** very much for any and all constructive feedback that was provided on Pipenv and how it does/doesn’t fit into your workflow. Every single comment was read and considered carefully, multiple times — though not responded to. Bandwidth is not available for responses, unfortunately.
- If I came across as crass in any comments, please keep in mind that I was very stressed out with all this negative attention (which is rare for me, the attention is typically quite positive). In addition, I had just started a brand new job, and had a week of little sleep at PyCon. Little Sleep + [Bipolar Type I](https://www.kennethreitz.org/essays/mentalhealtherror-an-exception-occurred) == coming across as dismissive, potentially.
- I’m not perfect. I try my hardest to be the kindest, most approachable and open person in Python — but that comes at a great cost to me — and sometimes I just can’t be that. So, if you had an interaction with me, and it tainted your view of me or my projects, I beg you to reconsider your new view — moods come in waves, and I cannot perform at 100% at all moments. It’s simply not possible.
- I have limited mental bandwidth, and parsing through and individually responding to hundreds of comments filled with personal opinions, often with slightly misaligned views of Python packaging is not within my capacity. I have a lot on my plate, between having a brand new job, managing my freely available web services, keeping up with technology, managing my open source projects, making music, taking photos, learning Kubernetes/Docker, random emails from random people asking random questions, mentorship requests, keynote requests, and orchestrating a new revision of The Hitchhiker’s Guide to Python from O’Reilly. The amount of inbound requests I have incoming is tremendous, and I simply don’t have the bandwidth to respond to all the valid comments and concerns in **/r/python**, so I’m addressing them here, in macro mode.

To those that criticize the project for making too many releases (multiple releases a day) — I’ll say a few things:

- That was a manic period of mine (again, bipolar). I was working on Pipenv for 20+ hours a day for over 4 weeks. Yes, many releases were required. One for each bugfix.
- I’d rather go manic over a codebase than over magic/crystals/the cosmos. This was a very healthy expression for me — I’m sorry if it concerned anyone, but these are the constraints my brain places upon me. I have a severe mental disability, and I’m coping with it very well.
- There was only a period of one month when this occurred, it is not our normal release cadence.
- We just switched the project over to [calver](http://calver.org), with the explicit purpose of preventing me from making more than one release a day — so this shouldn’t be an issue going forward.
- To prevent such things from happening with Requests, I actually revoked my own credentials from PyPI to Requests last year. This has been successful.

Some facts:

- Pipenv is a tool that is widely adopted, and quickly becoming a new workflow standard for many new and experienced Python developers.
- It is, above all else, a workflow tool.
- There is a misnomer that Pipenv is not useful for libraries. That is false. Try using `$ pipenv install -e .` and see what it does when you lock. It augments `setup.py`. I, as a library developer, find that extremely useful.
- Pipenv’s popularity is not because it was written by myself — though that certainly doesn’t hurt. It is because it enforces great practices that most experienced Python developers already employ, but it does them without you having to type any additional commands. *Pipenv is primarily a workflow tool, first and foremost*. That’s why it’s called “Python Dev Workflow for Humans”.
- `Pipfile`/`Pipfile.lock`, the replacement for the true thing that is at play here (`requirements.txt`), will be landing in pip proper in the future, and when that’s the case, you can use it without using Pipenv! In fact, **there’s a huge opportunity here**! Someone — go build a Pipfile -\> pip tool, today! That’ll solve a *huge* use case for a large number of people that don’t want to use Pipenv.
- If you don't like the workflow that Pipenv offers, simply stick with what you love! For example: use pip / virtualenv! Don’t overwhelm me on Reddit with your opinions of how it should be different and your justifications for why. We’re a year and half into this project, with a team of 5 highly time–constrained individuals doing our best to keep up with the *expectations* of an ever-growing audience (170,000 installs this month).
- Packing tools are **hard**. They require a deep understanding of Python infrastructure to build

Of all the work I’ve created, I’m most proud of Pipenv. More than I am of Requests. Pipenv was much more difficult to create, and even harder to maintain. Much. And, it has the potential to shape the future of Python in a way that Requests does not.

So — thank you for your time, and thank you for listening to my thoughts and perspective.

I love you all — even if some of you don't love me anymore.

✨🍰✨

