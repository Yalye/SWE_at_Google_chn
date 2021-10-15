## CHAPTER 2

How to Work Well on Teams

Written by Brian Fitzpatrick

Edited by Riona MacNamara

Because this chapter is about the cultural and social aspects of software engineering at Google, it makes sense to begin by focusing on the one variable over which you definitely have control: you.

People are inherently imperfect—we like to say that humans are mostly a collection of intermittent bugs. But before you can understand the bugs in your coworkers, you need to understand the bugs in yourself. We’re going to ask you to think about your own reactions, behaviors, and attitudes—and in return, we hope you gain some real insight into how to become a more efficient and successful software engineer who spends less energy dealing with people-related problems and more time writing great code.

The critical idea in this chapter is that software development is a team endeavor. And to succeed on an engineering team—or in any other creative collaboration—you need to reorganize your behaviors around the core principles of humility, respect, and trust.

Before we get ahead of ourselves, let’s begin by observing how software engineers tend to behave in general.

### Help Me Hide My Code

For the past 20 years, my colleague Ben and I have spoken at many programming conferences. In 2006, we launched Google’s (now deprecated) open source Project Hosting service, and at first, we used to get lots of questions and requests about the product. But around mid-2008, we began to notice a trend in the sort of requests we were getting:    “Can you please give Subversion on Google Code the ability to hide specific branches?”    “Can you make it possible to create open source projects that start out hidden to the world and then are revealed when they’re ready?”    “Hi, I want to rewrite all my code from scratch, can you please wipe all the history?”

Can you spot a common theme to these requests?

The answer is insecurity. People are afraid of others seeing and judging their work in progress. In one sense, insecurity is just a part of human nature—nobody likes to be criticized, especially for things that aren’t finished. Recognizing this theme tipped us off to a more general trend within software development: insecurity is actually a symptom of a larger problem.

### The Genius Myth

Many humans have the instinct to find and worship idols. For software engineers, those might be Linus Torvalds, Guido Van Rossum, Bill Gates—all heroes who changed the world with heroic feats. Linus wrote Linux by himself, right?

Actually, what Linus did was write just the beginnings of a proof-of-concept Unixlike kernel and show it to an email list. That was no small accomplishment, and it was definitely an impressive achievement, but it was just the tip of the iceberg. Linux is hundreds of times bigger than that initial kernel and was developed by thousands of smart people. Linus’ real achievement was to lead these people and coordinate their work; Linux is the shining result not of his original idea, but of the collective labor of the community. (And Unix itself was not entirely written by Ken Thompson and Dennis Ritchie, but by a group of smart people at Bell Labs.)

On that same note, did Guido Van Rossum personally write all of Python? Certainly, he wrote the first version. But hundreds of others were responsible for contributing to subsequent versions, including ideas, features, and bug fixes. Steve Jobs led an entire team that built the Macintosh, and although Bill Gates is known for writing a BASIC interpreter for early home computers, his bigger achievement was building a successful company around MS-DOS. Yet they all became leaders and symbols of the collective achievements of their communities. The Genius Myth is the tendency that we as humans need to ascribe the success of a team to a single person/leader.

And what about Michael Jordan?

It’s the same story. We idolized him, but the fact is that he didn’t win every basketballgame by himself. His true genius was in the way he worked with his team. The team’scoach, Phil Jackson, was extremely clever, and his coaching techniques are legendary. He recognized that one player alone never wins a championship, and so he assembledan entire “dream team” around MJ. This team was a well-oiled machine—at least asimpressive as Michael himself.

So, why do we repeatedly idolize the individual in these stories? Why do people buy products endorsed by celebrities? Why do we want to buy Michelle Obama’s dress or Michael Jordan’s shoes?

Celebrity is a big part of it. Humans have a natural instinct to find leaders and rolemodels, idolize them, and attempt to imitate them. We all need heroes for inspiration,and the programming world has its heroes, too. The phenomenon of “techiecelebrity”has almost spilled over into mythology. We all want to write something world-changing like Linux or design the next brilliant programming language.

Deep down, many engineers secretly wish to be seen as geniuses. This fantasy goes something like this:
• You are struck by an awesome new concept.
• You vanish into your cave for weeks or months, slaving away at a perfect implementationof your idea.
• You then “unleash” your software on the world, shocking everyone with yourgenius.
• Your peers are astonished by your cleverness.
• People line up to use your software.
• Fame and fortune follow naturally.

But hold on: time for a reality check. You’re probably not a genius.

No offense, of course—we’re sure that you’re a very intelligent person. But do you realize how rare actual geniuses really are? Sure, you write code, and that’s a tricky skill. But even if you are a genius, it turns out that that’s not enough. Geniuses still make mistakes, and having brilliant ideas and elite programming skills doesn’t guarantee that your software will be a hit. Worse, you might find yourself solving only analytical problems and not human problems. Being a genius is most definitely not an excuse for being a jerk: anyone—genius or not—with poor social skills tends to be a poor teammate. The vast majority of the work at Google (and at most companies!)doesn’t require genius-level intellect, but 100% of the work requires a minimal level of social skills. What will make or break your career, especially at a company like Google, is how well you collaborate with others.

It turns out that this Genius Myth is just another manifestation of our insecurity.

Many programmers are afraid to share work they’ve only just started because it means peers will see their mistakes and know the author of the code is not a genius.

The Genius Myth | 29

To quote a friend:

I know I get SERIOUSLY insecure about people looking before something is done.

Like they are going to seriously judge me and think I’m an idiot.

This is an extremely common feeling among programmers, and the natural reactionis to hide in a cave, work, work, work, and then polish, polish, polish, sure that no one will see your goof-ups and that you’ll still have a chance to unveil your masterpiece when you’re done. Hide away until your code is perfect.

Another common motivation for hiding your work is the fear that another programmer might take your idea and run with it before you get around to working on it. Bykeeping it secret, you control the idea.

We know what you’re probably thinking now: so what? Shouldn’t people be allowedto work however they want?

Actually, no. In this case, we assert that you’re doing it wrong, and it is a big deal.

Here’s why.

Hiding Considered Harmful

If you spend all of your time working alone, you’re increasing the risk of unnecessaryfailure and cheating your potential for growth. Even though software development isdeeply intellectual work that can require deep concentration and alone time, youmust play that off against the value (and need!) for collaboration and review.

First of all, how do you even know whether you’re on the right track?

Imagine you’re a bicycle-design enthusiast, and one day you get a brilliant idea for acompletely new way to design a gear shifter. You order parts and proceed to spendweeks holed up in your garage trying to build a prototype. When your neighbor—also a bike advocate—asks you what’s up, you decide not to talk about it. You don’twant anyone to know about your project until it’s absolutely perfect. Another fewmonths go by and you’re having trouble making your prototype work correctly. Butbecause you’re working in secrecy, it’s impossible to solicit advice from your mechanicallyinclined friends.

Then, one day your neighbor pulls his bike out of his garage with a radical new gearshiftingmechanism. Turns out he’s been building something very similar to yourinvention, but with the help of some friends down at the bike shop. At this point,you’re exasperated. You show him your work. He points out that your design hadsome simple flaws—ones that might have been fixed in the first week if you hadshown him. There are a number of lessons to learn here.30 | Chapter 2: How to Work Well on Teams2 Literally, if you are, in fact, a bike designer.3 I should note that sometimes it’s dangerous to get too much feedback too early in the process if you’re stillunsure of your general direction or goal.

Early Detection

If you keep your great idea hidden from the world and refuse to show anyone anythinguntil the implementation is polished, you’re taking a huge gamble. It’s easy tomake fundamental design mistakes early on. You risk reinventing wheels.2 And youforfeit the benefits of collaboration, too: notice how much faster your neighbormoved by working with others? This is why people dip their toes in the water beforejumping in the deep end: you need to make sure that you’re working on the rightthing, you’re doing it correctly, and it hasn’t been done before. The chances of anearly misstep are high. The more feedback you solicit early on, the more you lowerthis risk.3 Remember the tried-and-true mantra of “Fail early, fail fast, fail often.”

Early sharing isn’t just about preventing personal missteps and getting your ideas vetted.

It’s also important to strengthen what we call the bus factor of your project.

The Bus Factor

Bus factor (noun): the number of people that need to get hit by a bus before yourproject is completely doomed.

How dispersed is the knowledge and know-how in your project? If you’re the onlyperson who understands how the prototype code works, you might enjoy good jobsecurity—but if you get hit by a bus, the project is toast. If you’re working with a colleague,however, you’ve doubled the bus factor. And if you have a small team designingand prototyping together, things are even better—the project won’t be maroonedwhen a team member disappears. Remember: team members might not literally behit by buses, but other unpredictable life events still happen. Someone might get married,move away, leave the company, or take leave to care for a sick relative. Ensuringthat there is at least good documentation in addition to a primary and a secondaryowner for each area of responsibility helps future-proof your project’s success andincreases your project’s bus factor. Hopefully most engineers recognize that it is betterto be one part of a successful project than the critical part of a failed project.

Beyond the bus factor, there’s the issue of overall pace of progress. It’s easy to forgetthat working alone is often a tough slog, much slower than people want to admit.

How much do you learn when working alone? How fast do you move? Google and

Stack Overflow are great sources of opinions and information, but they’re no substitutefor actual human experience. Working with other people directly increases thecollective wisdom behind the effort. When you become stuck on something absurd,how much time do you waste pulling yourself out of the hole? Think about how

Hiding Considered Harmful | 31different the experience would be if you had a couple of peers to look over yourshoulder and tell you—instantly—how you goofed and how to get past the problem.

This is exactly why teams sit together (or do pair programming) in software engineeringcompanies. Programming is hard. Software engineering is even harder. Youneed that second pair of eyes.

Pace of Progress

Here’s another analogy. Think about how you work with your compiler. When you sitdown to write a large piece of software, do you spend days writing 10,000 lines ofcode, and then, after writing that final, perfect line, press the “compile” button for thevery first time? Of course you don’t. Can you imagine what sort of disaster wouldresult? Programmers work best in tight feedback loops: write a new function, compile.

Add a test, compile. Refactor some code, compile. This way, we discover and fixtypos and bugs as soon as possible after generating code. We want the compiler at ourside for every little step; some environments can even compile our code as we type.

This is how we keep code quality high and make sure our software is evolving correctly,bit by bit. The current DevOps philosophy toward tech productivity is explicitabout these sorts of goals: get feedback as early as possible, test as early as possible,and think about security and production environments as early as possible. This is allbundled into the idea of “shifting left” in the developer workflow; the earlier we find aproblem, the cheaper it is to fix it.

The same sort of rapid feedback loop is needed not just at the code level, but at thewhole-project level, too. Ambitious projects evolve quickly and must adapt to changingenvironments as they go. Projects run into unpredictable design obstacles orpolitical hazards, or we simply discover that things aren’t working as planned.

Requirements morph unexpectedly. How do you get that feedback loop so that youknow the instant your plans or designs need to change? Answer: by working in ateam. Most engineers know the quote, “Many eyes make all bugs shallow,” but a betterversion might be, “Many eyes make sure your project stays relevant and on track.”

People working in caves awaken to discover that while their original vision might becomplete, the world has changed and their project has become irrelevant.

Case Study: Engineers and Offices

Twenty-five years ago, conventional wisdom stated that for an engineer to be productive,they needed to have their own office with a door that closed. This was supposedlythe only way they could have big, uninterrupted slabs of time to deeplyconcentrate on writing reams of code.32 | Chapter 2: How to Work Well on Teams4 I do, however, acknowledge that serious introverts likely need more peace, quiet, and alone time than mostpeople and might benefit from a quieter environment, if not their own office.

I think that it’s not only unnecessary for most engineers4 to be in a private office, it’sdownright dangerous. Software today is written by teams, not individuals, and a highbandwidth,readily available connection to the rest of your team is even more valuablethan your internet connection. You can have all the uninterrupted time in theworld, but if you’re using it to work on the wrong thing, you’re wasting your time.

Unfortunately, it seems that modern-day tech companies (including Google, in somecases) have swung the pendulum to the exact opposite extreme. Walk into their officesand you’ll often find engineers clustered together in massive rooms—a hundredor more people together—with no walls whatsoever. This “open floor plan” is now atopic of huge debate and, as a result, hostility toward open offices is on the rise. Thetiniest conversation becomes public, and people end up not talking for risk of annoyingdozens of neighbors. This is just as bad as private offices!

We think the middle ground is really the best solution. Group teams of four to eightpeople together in small rooms (or large offices) to make it easy (and nonembarrassing)for spontaneous conversation to happen.

Of course, in any situation, individual engineers still need a way to filter out noise andinterruptions, which is why most teams I’ve seen have developed a way to communicatethat they’re currently busy and that you should limit interruptions. Some of usused to work on a team with a vocal interrupt protocol: if you wanted to talk, youwould say “Breakpoint Mary,” where Mary was the name of the person you wanted totalk to. If Mary was at a point where she could stop, she would swing her chair aroundand listen. If Mary was too busy, she’d just say “ack,” and you’d go on with other thingsuntil she finished with her current head state.

Other teams have tokens or stuffed animals that team members put on their monitorto signify that they should be interrupted only in case of emergency. Still other teamsgive out noise-canceling headphones to engineers to make it easier to deal with backgroundnoise—in fact, in many companies, the very act of wearing headphones is acommon signal that means “don’t disturb me unless it’s really important.” Many engineerstend to go into headphones-only mode when coding, which may be useful forshort spurts but, if used all the time, can be just as bad for collaboration as wallingyourself off in an office.

Don’t misunderstand us—we still think engineers need uninterrupted time to focuson writing code, but we think they need a high-bandwidth, low-friction connection totheir team just as much. If less-knowledgeable people on your team feel that there’s abarrier to asking you a question, it’s a problem: finding the right balance is an art.

Hiding Considered Harmful | 33

In Short, Don’t Hide

So, what “hiding” boils down to is this: working alone is inherently riskier than workingwith others. Even though you might be afraid of someone stealing your idea orthinking you’re not intelligent, you should be much more concerned about wastinghuge swaths of your time toiling away on the wrong thing.

Don’t become another statistic.

It’s All About the Team

So, let’s back up now and put all of these ideas together.

The point we’ve been hammering away at is that, in the realm of programming, lonecraftspeople are extremely rare—and even when they do exist, they don’t performsuperhuman achievements in a vacuum; their world-changing accomplishment isalmost always the result of a spark of inspiration followed by a heroic team effort.

A great team makes brilliant use of its superstars, but the whole is always greater thanthe sum of its parts. But creating a superstar team is fiendishly difficult.

Let’s put this idea into simpler words: software engineering is a team endeavor.

This concept directly contradicts the inner Genius Programmer fantasy so many of ushold, but it’s not enough to be brilliant when you’re alone in your hacker’s lair. You’renot going to change the world or delight millions of computer users by hiding andpreparing your secret invention. You need to work with other people. Share yourvision. Divide the labor. Learn from others. Create a brilliant team.

Consider this: how many pieces of widely used, successful software can you namethat were truly written by a single person? (Some people might say “LaTeX,” but it’shardly “widely used,” unless you consider the number of people writing scientificpapers to be a statistically significant portion of all computer users!)

High-functioning teams are gold and the true key to success. You should be aimingfor this experience however you can.

The Three Pillars of Social Interaction

So, if teamwork is the best route to producing great software, how does one build (orfind) a great team?

To reach collaborative nirvana, you first need to learn and embrace what I call the“three pillars” of social skills. These three principles aren’t just about greasing thewheels of relationships; they’re the foundation on which all healthy interaction andcollaboration are based:34 | Chapter 2: How to Work Well on Teams5 This is incredibly difficult if you’ve been burned in the past by delegating to incompetent people.

Pillar 1: Humility

You are not the center of the universe (nor is your code!). You’re neither omniscientnor infallible. You’re open to self-improvement.

Pillar 2: Respect

You genuinely care about others you work with. You treat them kindly andappreciate their abilities and accomplishments.

Pillar 3: Trust

You believe others are competent and will do the right thing, and you’re OK withletting them drive when appropriate.5

If you perform a root-cause analysis on almost any social conflict, you can ultimatelytrace it back to a lack of humility, respect, and/or trust. That might sound implausibleat first, but give it a try. Think about some nasty or uncomfortable social situationcurrently in your life. At the basest level, is everyone being appropriately humble? Arepeople really respecting one another? Is there mutual trust?

Why Do These Pillars Matter?

When you began this chapter, you probably weren’t planning to sign up for some sortof weekly support group. We empathize. Dealing with social problems can be difficult:people are messy, unpredictable, and often annoying to interface with. Ratherthan putting energy into analyzing social situations and making strategic moves, it’stempting to write off the whole effort. It’s much easier to hang out with a predictablecompiler, isn’t it? Why bother with the social stuff at all?

Here’s a quote from a famous lecture by Richard Hamming:

By taking the trouble to tell jokes to the secretaries and being a little friendly, I gotsuperb secretarial help. For instance, one time for some idiot reason all the reproducingservices at Murray Hill were tied up. Don’t ask me how, but they were. I wantedsomething done. My secretary called up somebody at Holmdel, hopped [into] the companycar, made the hour-long trip down and got it reproduced, and then came back. Itwas a payoff for the times I had made an effort to cheer her up, tell her jokes and befriendly; it was that little extra work that later paid off for me. By realizing you have touse the system and studying how to get the system to do your work, you learn how toadapt the system to your desires.

The moral is this: do not underestimate the power of playing the social game. It’s notabout tricking or manipulating people; it’s about creating relationships to get thingsdone. Relationships always outlast projects. When you’ve got richer relationshipswith your coworkers, they’ll be more willing to go the extra mile when you needthem.

It’s All About the Team | 35

Humility, Respect, and Trust in Practice

All of this preaching about humility, respect, and trust sounds like a sermon. Let’scome out of the clouds and think about how to apply these ideas in real-life situations.

We’re going to examine a list of specific behaviors and examples that you canstart with. Many of them might sound obvious at first, but after you begin thinkingabout them, you’ll notice how often you (and your peers) are guilty of not followingthem—we’ve certainly noticed this about ourselves!

Lose the ego

OK, this is sort of a simpler way of telling someone without enough humility to losetheir ’tude. Nobody wants to work with someone who consistently behaves likethey’re the most important person in the room. Even if you know you’re the wisestperson in the discussion, don’t wave it in people’s faces. For example, do you alwaysfeel like you need to have the first or last word on every subject? Do you feel the needto comment on every detail in a proposal or discussion? Or do you know somebodywho does these things?

Although it’s important to be humble, that doesn’t mean you need to be a doormat;there’s nothing wrong with self-confidence. Just don’t come off like a know-it-all.

Even better, think about going for a “collective” ego, instead; rather than worryingabout whether you’re personally awesome, try to build a sense of team accomplishmentand group pride. For example, the Apache Software Foundation has a long historyof creating communities around software projects. These communities haveincredibly strong identities and reject people who are more concerned with selfpromotion.

Ego manifests itself in many ways, and a lot of the time, it can get in the way of yourproductivity and slow you down. Here’s another great story from Hamming’s lecturethat illustrates this point perfectly (emphasis ours):

John Tukey almost always dressed very casually. He would go into an important officeand it would take a long time before the other fellow realized that this is a first-classman and he had better listen. For a long time, John has had to overcome this kind ofhostility. It’s wasted effort! I didn’t say you should conform; I said, “The appearance ofconforming gets you a long way.” If you chose to assert your ego in any number ofways, “I am going to do it my way,” you pay a small steady price throughout the wholeof your professional career. And this, over a whole lifetime, adds up to an enormousamount of needless trouble. […] By realizing you have to use the system and studyinghow to get the system to do your work, you learn how to adapt the system to yourdesires. Or you can fight it steadily, as a small, undeclared war, for the whole of your life.36 | Chapter 2: How to Work Well on Teams

Learn to give and take criticism

A few years ago, Joe started a new job as a programmer. After his first week, he reallybegan digging into the codebase. Because he cared about what was going on, hestarted gently questioning other teammates about their contributions. He sent simplecode reviews by email, politely asking about design assumptions or pointing outplaces where logic could be improved. After a couple of weeks, he was summoned tohis director’s office. “What’s the problem?” Joe asked. “Did I do something wrong?”

The director looked concerned: “We’ve had a lot of complaints about your behavior,

Joe. Apparently, you’ve been really harsh toward your teammates, criticizing them leftand right. They’re upset. You need to tone it down.” Joe was utterly baffled. Surely, hethought, his code reviews should have been welcomed and appreciated by his peers.

In this case, however, Joe should have been more sensitive to the team’s widespreadinsecurity and should have used a subtler means to introduce code reviews into theculture—perhaps even something as simple as discussing the idea with the team inadvance and asking team members to try it out for a few weeks.

In a professional software engineering environment, criticism is almost never personal—it’s usually just part of the process of making a better project. The trick is tomake sure you (and those around you) understand the difference between a constructivecriticism of someone’s creative output and a flat-out assault against someone’scharacter. The latter is useless—it’s petty and nearly impossible to act on. Theformer can (and should!) be helpful and give guidance on how to improve. And, mostimportant, it’s imbued with respect: the person giving the constructive criticism genuinelycares about the other person and wants them to improve themselves or theirwork. Learn to respect your peers and give constructive criticism politely. If you trulyrespect someone, you’ll be motivated to choose tactful, helpful phrasing—a skillacquired with much practice. We cover this much more in Chapter 9.

On the other side of the conversation, you need to learn to accept criticism as well.

This means not just being humble about your skills, but trusting that the other personhas your best interests (and those of your project!) at heart and doesn’t actually thinkyou’re an idiot. Programming is a skill like anything else: it improves with practice. Ifa peer pointed out ways in which you could improve your juggling, would you take itas an attack on your character and value as a human being? We hope not. In the sameway, your self-worth shouldn’t be connected to the code you write—or any creativeproject you build. To repeat ourselves: you are not your code. Say that over and over.

You are not what you make. You need to not only believe it yourself, but get yourcoworkers to believe it, too.

For example, if you have an insecure collaborator, here’s what not to say: “Man, youtotally got the control flow wrong on that method there. You should be using thestandard xyzzy code pattern like everyone else.” This feedback is full of antipatterns:you’re telling someone they’re “wrong” (as if the world were black and white),demanding they change something, and accusing them of creating something that

It’s All About the Team | 376 You can find a dozen variants of this legend on the web, attributed to different famous managers.7 By the same token, if you do the same thing over and over and keep failing, it’s not failure, it’s incompetence.goes against what everyone else is doing (making them feel stupid). Your coworkerwill immediately be put on the offense, and their response is bound to be overlyemotional.

A better way to say the same thing might be, “Hey, I’m confused by the control flowin this section here. I wonder if the xyzzy code pattern might make this clearer andeasier to maintain?” Notice how you’re using humility to make the question aboutyou, not them. They’re not wrong; you’re just having trouble understanding the code.

The suggestion is merely offered up as a way to clarify things for poor little you whilepossibly helping the project’s long-term sustainability goals. You’re also not demandinganything—you’re giving your collaborator the ability to peacefully reject the suggestion.

The discussion stays focused on the code itself, not on anyone’s value orcoding skills.

Fail fast and iterate

There’s a well-known urban legend in the business world about a manager whomakes a mistake and loses an impressive $10 million. He dejectedly goes into theoffice the next day and starts packing up his desk, and when he gets the inevitable“the CEO wants to see you in his office” call, he trudges into the CEO’s office and quietlyslides a piece of paper across the desk.“What’s this?” asks the CEO.“My resignation,” says the executive. “I assume you called me in here to fire me.”“Fire you?” responds the CEO, incredulously. “Why would I fire you? I just spent $10million training you!”6

It’s an extreme story, to be sure, but the CEO in this story understands that firing theexecutive wouldn’t undo the $10 million loss, and it would compound it by losing avaluable executive who he can be very sure won’t make that kind of mistake again.

At Google, one of our favorite mottos is that “Failure is an option.” It’s widely recognizedthat if you’re not failing now and then, you’re not being innovative enough ortaking enough risks. Failure is viewed as a golden opportunity to learn and improvefor the next go-around.7 In fact, Thomas Edison is often quoted as saying, “If I find10,000 ways something won’t work, I haven’t failed. I am not discouraged, becauseevery wrong attempt discarded is another step forward.”

Over in Google X—the division that works on “moonshots” like self-driving cars andinternet access delivered by balloons—failure is deliberately built into its incentivesystem. People come up with outlandish ideas and coworkers are actively encouraged38 | Chapter 2: How to Work Well on Teamsto shoot them down as fast as possible. Individuals are rewarded (and even compete)to see how many ideas they can disprove or invalidate in a fixed period of time. Onlywhen a concept truly cannot be debunked at a whiteboard by all peers does it proceedto early prototype.

Blameless Post-Mortem Culture

The key to learning from your mistakes is to document your failures by performing aroot-cause analysis and writing up a “postmortem,” as it’s called at Google (and manyother companies). Take extra care to make sure the postmortem document isn’t just auseless list of apologies or excuses or finger-pointing—that’s not its purpose. A properpostmortem should always contain an explanation of what was learned and what isgoing to change as a result of the learning experience. Then, make sure that the postmortemis readily accessible and that the team really follows through on the proposedchanges. Properly documenting failures also makes it easier for other people (presentand future) to know what happened and avoid repeating history. Don’t erase yourtracks—light them up like a runway for those who follow you!

A good postmortem should include the following:• A brief summary of the event• A timeline of the event, from discovery through investigation to resolution• The primary cause of the event• Impact and damage assessment• A set of action items (with owners) to fix the problem immediately• A set of action items to prevent the event from happening again• Lessons learned

Learn patience

Years ago, I was writing a tool to convert CVS repositories to Subversion (and later,

Git). Due to the vagaries of CVS, I kept unearthing bizarre bugs. Because my longtimefriend and coworker Karl knew CVS quite intimately, we decided we shouldwork together to fix these bugs.

A problem arose when we began pair programming: I’m a bottom-up engineer who iscontent to dive into the muck and dig my way out by trying a lot of things quicklyand skimming over the details. Karl, however, is a top-down engineer who wants toget the full lay of the land and dive into the implementation of almost every methodon the call stack before proceeding to tackle the bug. This resulted in some epic interpersonalconflicts, disagreements, and the occasional heated argument. It got to the

It’s All About the Team | 39point at which the two of us simply couldn’t pair-program together: it was too frustratingfor us both.

That said, we had a longstanding history of trust and respect for each other. Combinedwith patience, this helped us work out a new method of collaborating. Wewould sit together at the computer, identify the bug, and then split up and attack theproblem from two directions at once (top-down and bottom-up) before coming backtogether with our findings. Our patience and willingness to improvise new workingstyles not only saved the project, but also our friendship.

Be open to influence

The more open you are to influence, the more you are able to influence; the morevulnerable you are, the stronger you appear. These statements sound like bizarre contradictions.

But everyone can think of someone they’ve worked with who is just maddeninglystubborn—no matter how much people try to persuade them, they dig theirheels in even more. What eventually happens to such team members? In our experience,people stop listening to their opinions or objections; instead, they end up “routingaround” them like an obstacle everyone takes for granted. You certainly don’twant to be that person, so keep this idea in your head: it’s OK for someone else tochange your mind. In the opening chapter of this book, we said that engineering isinherently about trade-offs. It’s impossible for you to be right about everything all thetime unless you have an unchanging environment and perfect knowledge, so ofcourse you should change your mind when presented with new evidence. Chooseyour battles carefully: to be heard properly, you first need to listen to others. It’s betterto do this listening before putting a stake in the ground or firmly announcing a decision—if you’re constantly changing your mind, people will think you’re wishy-washy.

The idea of vulnerability can seem strange, too. If someone admits ignorance of thetopic at hand or the solution to a problem, what sort of credibility will they have in agroup? Vulnerability is a show of weakness, and that destroys trust, right?

Not true. Admitting that you’ve made a mistake or you’re simply out of your leaguecan increase your status over the long run. In fact, the willingness to express vulnerabilityis an outward show of humility, it demonstrates accountability and the willingnessto take responsibility, and it’s a signal that you trust others’ opinions. In return,people end up respecting your honesty and strength. Sometimes, the best thing youcan do is just say, “I don’t know.”

Professional politicians, for example, are notorious for never admitting error or ignorance,even when it’s patently obvious that they’re wrong or unknowledgeable about asubject. This behavior exists primarily because politicians are constantly under attackby their opponents, and it’s why most people don’t believe a word that politicians say.

When you’re writing software, however, you don’t need to be continually on the40 | Chapter 2: How to Work Well on Teamsdefensive—your teammates are collaborators, not competitors. You all have the samegoal.

Being Googley

At Google, we have our own internal version of the principles of “humility, respect,and trust” when it comes to behavior and human interactions.

From the earliest days of our culture, we often referred to actions as being “Googley”or “not Googley.” The word was never explicitly defined; rather, everyone just sort oftook it to mean “don’t be evil” or “do the right thing” or “be good to each other.” Overtime, people also started using the term “Googley” as an informal test for culture-fitwhenever we would interview a candidate for an engineering job, or when writinginternal performance reviews of one another. People would often express opinionsabout others using the term; for example, “the person coded well, but didn’t seem tohave a very Googley attitude.”

Of course, we eventually realized that the term “Googley” was being overloaded withmeaning; worse yet, it could become a source of unconscious bias in hiring or evaluations.

If “Googley” means something different to every employee, we run the risk ofthe term starting to mean “is just like me.” Obviously, that’s not a good test for hiring—we don’t want to hire people “just like me,” but people from a diverse set of backgroundsand with different opinions and experiences. An interviewer’s personaldesire to have a beer with a candidate (or coworker) should never be considered avalid signal about somebody else’s performance or ability to thrive at Google.

Google eventually fixed the problem by explicitly defining a rubric for what we meanby “Googleyness”—a set of attributes and behaviors that we look for that representstrong leadership and exemplify “humility, respect, and trust”:

Thrives in ambiguity

Can deal with conflicting messages or directions, build consensus, and make progressagainst a problem, even when the environment is constantly shifting.

Values feedback

Has humility to both receive and give feedback gracefully and understands howvaluable feedback is for personal (and team) development.

Challenges status quo

Is able to set ambitious goals and pursue them even when there might be resistanceor inertia from others.

Puts the user first

Has empathy and respect for users of Google’s products and pursues actions thatare in their best interests.

It’s All About the Team | 41

Cares about the team

Has empathy and respect for coworkers and actively works to help them withoutbeing asked, improving team cohesion.

Does the right thing

Has a strong sense of ethics about everything they do; willing to make difficult orinconvenient decisions to protect the integrity of the team and product.

Now that we have these best-practice behaviors better defined, we’ve begun to shyaway from using the term “Googley.” It’s always better to be specific about expectations!

Conclusion

The foundation for almost any software endeavor—of almost any size—is a wellfunctioningteam. Although the Genius Myth of the solo software developer still persists,the truth is that no one really goes it alone. For a software organization to standthe test of time, it must have a healthy culture, rooted in humility, trust, and respectthat revolves around the team, rather than the individual. Further, the creative natureof software development requires that people take risks and occasionally fail; for peopleto accept that failure, a healthy team environment must exist.

TL;DRs• Be aware of the trade-offs of working in isolation.• Acknowledge the amount of time that you and your team spend communicatingand in interpersonal conflict. A small investment in understanding personalitiesand working styles of yourself and others can go a long way toward improvingproductivity.• If you want to work effectively with a team or a large organization, be aware ofyour preferred working style and that of others.