

Knowledge Sharing

Written by Nina Chen and Mark Barolak

Edited by Riona MacNamara

Your organization understands your problem domain better than some random personon the internet; your organization should be able to answer most of its own questions.

To achieve that, you need both experts who know the answers to thosequestions and mechanisms to distribute their knowledge, which is what we’ll explorein this chapter. These mechanisms range from the utterly simple (Ask questions;

Write down what you know) to the much more structured, such as tutorials andclasses. Most importantly, however, your organization needs a culture of learning, andthat requires creating the psychological safety that permits people to admit to a lackof knowledge.

Challenges to Learning

Sharing expertise across an organization is not an easy task. Without a strong cultureof learning, challenges can emerge. Google has experienced a number of these challenges,especially as the company has scaled:

Lack of psychological safety

An environment in which people are afraid to take risks or make mistakes infront of others because they fear being punished for it. This often manifests as aculture of fear or a tendency to avoid transparency.

Information islands

Knowledge fragmentation that occurs in different parts of an organization thatdon’t communicate with one another or use shared resources. In such an431 In other words, rather than developing a single global maximum, we have a bunch of local maxima.environment, each group develops its own way of doing things.1 This often leadsto the following:

Information fragmentation

Each island has an incomplete picture of the bigger whole.

Information duplication

Each island has reinvented its own way of doing something.

Information skew

Each island has its own ways of doing the same thing, and these might ormight not conflict.

Single point of failure (SPOF)

A bottleneck that occurs when critical information is available from only a singleperson. This is related to bus factor, which is discussed in more detail in Chapter2.

SPOFs can arise out of good intentions: it can be easy to fall into a habit of “Letme take care of that for you.” But this approach optimizes for short-term efficiency(“It’s faster for me to do it”) at the cost of poor long-term scalability (theteam never learns how to do whatever it is that needs to be done). This mindsetalso tends to lead to all-or-nothing expertise.

All-or-nothing expertise

A group of people that is split between people who know “everything” and novices,with little middle ground. This problem often reinforces itself if expertsalways do everything themselves and don’t take the time to develop new expertsthrough mentoring or documentation. In this scenario, knowledge and responsibilitiescontinue to accumulate on those who already have expertise, and newteam members or novices are left to fend for themselves and ramp up moreslowly.

Parroting

Mimicry without understanding. This is typically characterized by mindlesslycopying patterns or code without understanding their purpose, often under theassumption that said code is needed for unknown reasons.

Haunted graveyards

Places, often in code, that people avoid touching or changing because they areafraid that something might go wrong. Unlike the aforementioned parroting,haunted graveyards are characterized by people avoiding action because of fearand superstition.44 | Chapter 3: Knowledge Sharing2 David Lorge Parnas, Software Engineering: Multi-person Development of Multi-version Programs (Heidelberg:

Springer-Verlag Berlin, 2011).

In the rest of this chapter, we dive into strategies that Google’s engineering organizationshave found to be successful in addressing these challenges.

Philosophy

Software engineering can be defined as the multiperson development of multiversionprograms.2 People are at the core of software engineering: code is an important outputbut only a small part of building a product. Crucially, code does not emerge spontaneouslyout of nothing, and neither does expertise. Every expert was once a novice:an organization’s success depends on growing and investing in its people.

Personalized, one-to-one advice from an expert is always invaluable. Different teammembers have different areas of expertise, and so the best teammate to ask for anygiven question will vary. But if the expert goes on vacation or switches teams, theteam can be left in the lurch. And although one person might be able to provide personalizedhelp for one-to-many, this doesn’t scale and is limited to small numbers of“many.”

Documented knowledge, on the other hand, can better scale not just to the team butto the entire organization. Mechanisms such as a team wiki enable many authors toshare their expertise with a larger group. But even though written documentation ismore scalable than one-to-one conversations, that scalability comes with some tradeoffs:it might be more generalized and less applicable to individual learners’ situations,and it comes with the added maintenance cost required to keep informationrelevant and up to date over time.

Tribal knowledge exists in the gap between what individual team members know andwhat is documented. Human experts know these things that aren’t written down. Ifwe document that knowledge and maintain it, it is now available not only to somebodywith direct one-to-one access to the expert today, but to anybody who can findand view the documentation.

So in a magical world in which everything is always perfectly and immediately documented,we wouldn’t need to consult a person any more, right? Not quite. Writtenknowledge has scaling advantages, but so does targeted human help. A human expertcan synthesize their expanse of knowledge. They can assess what information is applicableto the individual’s use case, determine whether the documentation is still relevant,and know where to find it. Or, if they don’t know where to find the answers,they might know who does.

Philosophy | 45

Tribal and written knowledge complement each other. Even a perfectly expert teamwith perfect documentation needs to communicate with one another, coordinate withother teams, and adapt their strategies over time. No single knowledge-sharingapproach is the correct solution for all types of learning, and the particulars of a goodmix will likely vary based on your organization. Institutional knowledge evolves overtime, and the knowledge-sharing methods that work best for your organization willlikely change as it grows. Train, focus on learning and growth, and build your ownstable of experts: there is no such thing as too much engineering expertise.

Setting the Stage: Psychological Safety

Psychological safety is critical to promoting a learning environment.

To learn, you must first acknowledge that there are things you don’t understand. Weshould welcome such honesty rather than punish it. (Google does this pretty well, butsometimes engineers are reluctant to admit they don’t understand something.)

An enormous part of learning is being able to try things and feeling safe to fail. In ahealthy environment, people feel comfortable asking questions, being wrong, andlearning new things. This is a baseline expectation for all Google teams; indeed, ourresearch has shown that psychological safety is the most important part of an effectiveteam.

Mentorship

At Google, we try to set the tone as soon as a “Noogler” (new Googler) engineer joinsthe company. One important way of building psychological safety is to assign Nooglersa mentor—someone who is not their team member, manager, or tech lead—whose responsibilities explicitly include answering questions and helping the Nooglerramp up. Having an officially assigned mentor to ask for help makes it easier for thenewcomer and means that they don’t need to worry about taking up too much oftheir coworkers’ time.

A mentor is a volunteer who has been at Google for more than a year and who isavailable to advise on anything from using Google infrastructure to navigating Googleculture. Crucially, the mentor is there to be a safety net to talk to if the menteedoesn’t know whom else to ask for advice. This mentor is not on the same team as thementee, which can make the mentee feel more comfortable about asking for help intricky situations.

Mentorship formalizes and facilitates learning, but learning itself is an ongoing process.

There will always be opportunities for coworkers to learn from one another,whether it’s a new employee joining the organization or an experienced engineerlearning a new technology. With a healthy team, teammates will be open not just to46 | Chapter 3: Knowledge Sharinganswering but also to asking questions: showing that they don’t know something andlearning from one another.

Psychological Safety in Large Groups

Asking a nearby teammate for help is easier than approaching a large group of mostlystrangers. But as we’ve seen, one-to-one solutions don’t scale well. Group solutionsare more scalable, but they are also scarier. It can be intimidating for novices to forma question and ask it of a large group, knowing that their question might be archivedfor many years. The need for psychological safety is amplified in large groups. Everymember of the group has a role to play in creating and maintaining a safe environmentthat ensures that newcomers are confident asking questions and up-andcomingexperts feel empowered to help those newcomers without the fear of havingtheir answers attacked by established experts.

The most important way to achieve this safe and welcoming environment is for groupinteractions to be cooperative, not adversarial. Table 3-1 lists some examples of recommendedpatterns (and their corresponding antipatterns) of group interactions.

Table 3-1. Group interaction patterns

Recommended patterns (cooperative) Antipatterns (adversarial)

Basic questions or mistakes are guided in the properdirection

Basic questions or mistakes are picked on, and the personasking the question is chastised

Explanations are given with the intent of helping the personasking the question learn

Explanations are given with the intent of showing off one’sown knowledge

Responses are kind, patient, and helpful Responses are condescending, snarky, and unconstructive

Interactions are shared discussions for finding solutions Interactions are arguments with “winners” and “losers”

These antipatterns can emerge unintentionally: someone might be trying to be helpfulbut is accidentally condescending and unwelcoming. We find the Recurse Center’ssocial rules to be helpful here:

No feigned surprise (“What?! I can’t believe you don’t know what the stack is!”)

Feigned surprise is a barrier to psychological safety and makes members of thegroup afraid of admitting to a lack of knowledge.

No “well-actuallys”

Pedantic corrections that tend to be about grandstanding rather than precision.

No back-seat driving

Interrupting an existing discussion to offer opinions without committing to theconversation.

Setting the Stage: Psychological Safety | 473 Impostor syndrome is not uncommon among high achievers, and Googlers are no exception—in fact, amajority of this book’s authors have impostor syndrome. We acknowledge that fear of failure can be difficultfor those with impostor syndrome and can reinforce an inclination to avoid branching out.4 See “How to ask good questions.”

No subtle “-isms” (“It’s so easy my grandmother could do it!”)

Small expressions of bias (racism, ageism, homophobia) that can make individualsfeel unwelcome, disrespected, or unsafe.

Growing Your Knowledge

Knowledge sharing starts with yourself. It is important to recognize that you alwayshave something to learn. The following guidelines allow you to augment your ownpersonal knowledge.

Ask Questions

If you take away only a single thing from this chapter, it is this: always be learning;always be asking questions.

We tell Nooglers that ramping up can take around six months. This extended periodis necessary to ramp up on Google’s large, complex infrastructure, but it also reinforcesthe idea that learning is an ongoing, iterative process. One of the biggest mistakesthat beginners make is not to ask for help when they’re stuck. You might be temptedto struggle through it alone or feel fearful that your questions are “too simple.” “I justneed to try harder before I ask anyone for help,” you think. Don’t fall into this trap!

Your coworkers are often the best source of information: leverage this valuableresource.

There is no magical day when you suddenly always know exactly what to do in everysituation—there’s always more to learn. Engineers who have been at Google for yearsstill have areas in which they don’t feel like they know what they are doing, and that’s

OK! Don’t be afraid to say “I don’t know what that is; could you explain it?” Embracenot knowing things as an area of opportunity rather than one to fear.3

It doesn’t matter whether you’re new to a team or a senior leader: you should alwaysbe in an environment in which there’s something to learn. If not, you stagnate (andshould find a new environment).

It’s especially critical for those in leadership roles to model this behavior: it’s importantnot to mistakenly equate “seniority” with “knowing everything.” In fact, the moreyou know, the more you know you don’t know. Openly asking questions4 or expressinggaps in knowledge reinforces that it’s OK for others to do the same.48 | Chapter 3: Knowledge Sharing

On the receiving end, patience and kindness when answering questions fosters anenvironment in which people feel safe looking for help. Making it easier to overcomethe initial hesitation to ask a question sets the tone early: reach out to solicit questions,and make it easy for even “trivial” questions to get an answer. Although engineerscould probably figure out tribal knowledge on their own, they’re not here towork in a vacuum. Targeted help allows engineers to be productive faster, which inturn makes their entire team more productive.

Understand Context

Learning is not just about understanding new things; it also includes developing anunderstanding of the decisions behind the design and implementation of existingthings. Suppose that your team inherits a legacy codebase for a critical piece of infrastructurethat has existed for many years. The original authors are long gone, and thecode is difficult to understand. It can be tempting to rewrite from scratch rather thanspend time learning the existing code. But instead of thinking “I don’t get it” and endingyour thoughts there, dive deeper: what questions should you be asking?

Consider the principle of “Chesterson’s fence”: before removing or changing something,first understand why it’s there.

In the matter of reforming things, as distinct from deforming them, there is one plainand simple principle; a principle which will probably be called a paradox. There existsin such a case a certain institution or law; let us say, for the sake of simplicity, a fence orgate erected across a road. The more modern type of reformer goes gaily up to it andsays, “I don’t see the use of this; let us clear it away.” To which the more intelligent typeof reformer will do well to answer: “If you don’t see the use of it, I certainly won’t letyou clear it away. Go away and think. Then, when you can come back and tell me thatyou do see the use of it, I may allow you to destroy it.”

This doesn’t mean that code can’t lack clarity or that existing design patterns can’t bewrong, but engineers have a tendency to reach for “this is bad!” far more quickly thanis often warranted, especially for unfamiliar code, languages, or paradigms. Google isnot immune to this. Seek out and understand context, especially for decisions thatseem unusual. After you’ve understood the context and purpose of the code, considerwhether your change still makes sense. If it does, go ahead and make it; if it doesn’t,document your reasoning for future readers.

Many Google style guides explicitly include context to help readers understand therationale behind the style guidelines instead of just memorizing a list of arbitraryrules. More subtly, understanding the rationale behind a given guideline allowsauthors to make informed decisions about when the guideline shouldn’t apply orwhether the guideline needs updating. See Chapter 8.

Growing Your Knowledge | 49

Scaling Your Questions: Ask the Community

Getting one-to-one help is high bandwidth but necessarily limited in scale. And as alearner, it can be difficult to remember every detail. Do your future self a favor: whenyou learn something from a one-to-one discussion, write it down.

Chances are that future newcomers will have the same questions you had. Do them afavor, too, and share what you write down.

Although sharing the answers you receive can be useful, it’s also beneficial to seekhelp not from individuals but from the greater community. In this section, we examinedifferent forms of community-based learning. Each of these approaches—groupchats, mailing lists, and question-and-answer systems—have different trade-offs andcomplement one another. But each of them enables the knowledge seeker to get helpfrom a broader community of peers and experts and also ensures that answers arebroadly available to current and future members of that community.

Group Chats

When you have a question, it can sometimes be difficult to get help from the rightperson. Maybe you’re not sure who knows the answer, or the person you want to askis busy. In these situations, group chats are great, because you can ask your questionto many people at once and have a quick back-and-forth conversation with whoeveris available. As a bonus, other members of the group chat can learn from the questionand answer, and many forms of group chat can be automatically archived andsearched later.

Group chats tend to be devoted either to topics or to teams. Topic-driven group chatsare typically open so that anyone can drop in to ask a question. They tend to attractexperts and can grow quite large, so questions are usually answered quickly. Teamorientedchats, on the other hand, tend to be smaller and restrict membership. As aresult, they might not have the same reach as a topic-driven chat, but their smallersize can feel safer to a newcomer.

Although group chats are great for quick questions, they don’t provide much structure,which can make it difficult to extract meaningful information from a conversationin which you’re not actively involved. As soon as you need to share informationoutside of the group, or make it available to refer back to later, you should write adocument or email a mailing list.

Mailing Lists

Most topics at Google have a topic-users@ or topic-discuss@ Google Groups mailinglist that anyone at the company can join or email. Asking a question on a public mailinglist is a lot like asking a group chat: the question reaches a lot of people who could50 | Chapter 3: Knowledge Sharingpotentially answer it and anyone following the list can learn from the answer. Unlikegroup chats, though, public mailing lists are easy to share with a wider audience: theyare packaged into searchable archives, and email threads provide more structure thangroup chats. At Google, mailing lists are also indexed and can be discovered by

Moma, Google’s intranet search engine.

When you find an answer to a question you asked on a mailing list, it can be temptingto get on with your work. Don’t do it! You never know when someone will needthe same information in the future, so it’s a best practice to post the answer back tothe list.

Mailing lists are not without their trade-offs. They’re well suited for complicatedquestions that require a lot of context, but they’re clumsy for the quick back-andforthexchanges at which group chats excel. A thread about a particular problem isgenerally most useful while it is active. Email archives are immutable, and it can behard to determine whether an answer discovered in an old discussion thread is stillrelevant to a present-day situation. Additionally, the signal-to-noise ratio can belower than other mediums like formal documentation because the problem thatsomeone is having with their specific workflow might not be applicable to you.

Email at Google

Google culture is infamously email-centric and email-heavy. Google engineers receivehundreds of emails (if not more) each day, with varying degrees of actionability. Nooglerscan spend days just setting up email filters to deal with the volume of notificationscoming from groups that they’ve been autosubscribed to; some people just giveup and don’t try to keep up with the flow. Some groups CC large mailing lists ontoevery discussion by default, without trying to target information to those who arelikely to be specifically interested in it; as a result, the signal-to-noise ratio can be areal problem.

Google tends toward email-based workflows by default. This isn’t necessarily becauseemail is a better medium than other communications options—it often isn’t—rather,it’s because that’s what our culture is accustomed to. Keep this in mind as your organizationconsiders what forms of communication to encourage or invest in.

YAQS: Question-and-Answer Platform

YAQS (“Yet Another Question System”) is a Google-internal version of a Stack Overflow–like website, making it easy for Googlers to link to existing or work-in-progresscode as well as discuss confidential information.

Like Stack Overflow, YAQS shares many of the same advantages of mailing lists andadds refinements: answers marked as helpful are promoted in the user interface, and

Scaling Your Questions: Ask the Community | 515 https://talksat.withgoogle.com and https://www.youtube.com/GoogleTechTalks, to name a few.users can edit questions and answers so that they remain accurate and useful as codeand facts change. As a result, some mailing lists have been superseded by YAQS,whereas others have evolved into more general discussion lists that are less focusedon problem solving.

Scaling Your Knowledge:

You Always Have Something to Teach

Teaching is not limited to experts, nor is expertise a binary state in which you areeither a novice or an expert. Expertise is a multidimensional vector of what youknow: everyone has varying levels of expertise across different areas. This is one ofthe reasons why diversity is critical to organizational success: different people bringdifferent perspectives and expertise to the table (see Chapter 4). Google engineersteach others in a variety of ways, such as office hours, giving tech talks, teachingclasses, writing documentation, and reviewing code.

Office Hours

Sometimes it’s really important to have a human to talk to, and in those instances,office hours can be a good solution. Office hours are a regularly scheduled (typicallyweekly) event during which one or more people make themselves available to answerquestions about a particular topic. Office hours are almost never the first choice forknowledge sharing: if you have an urgent question, it can be painful to wait for thenext session for an answer; and if you’re hosting office hours, they take up time andneed to be regularly promoted. That said, they do provide a way for people to talk toan expert in person. This is particularly useful if the problem is still ambiguousenough that the engineer doesn’t yet know what questions to ask (such as whenthey’re just starting to design a new service) or whether the problem is about somethingso specialized that there just isn’t documentation on it.

Tech Talks and Classes

Google has a robust culture of both internal and external5 tech talks and classes. OurengEDU (Engineering Education) team focuses on providing Computer Science educationto many audiences, ranging from Google engineers to students around theworld. At a more grassroots level, our g2g (Googler2Googler) program lets Googlers52 | Chapter 3: Knowledge Sharing6 The g2g program is detailed in: Laszlo Bock, Work Rules!: Insights from Inside Google That Will Transform

How You Live and Lead (New York: Twelve Books, 2015). It includes descriptions of different aspects of theprogram as well as how to evaluate impact and recommendations for what to focus on when setting up similarprograms.sign up to give or attend talks and classes from fellow Googlers.6 The program iswildly successful, with thousands of participating Googlers teaching topics from thetechnical (e.g., “Understanding Vectorization in Modern CPUs”) to the just-for-fun(e.g., “Beginner Swing Dance”).

Tech talks typically consist of a speaker presenting directly to an audience. Classes, onthe other hand, can have a lecture component but often center on in-class exercisesand therefore require more active participation from attendees. As a result,instructor-led classes are typically more demanding and expensive to create andmaintain than tech talks and are reserved for the most important or difficult topics.

That said, after a class has been created, it can be scaled relatively easily because manyinstructors can teach a class from the same course materials. We’ve found that classestend to work best when the following circumstances exist:• The topic is complicated enough that it’s a frequent source of misunderstanding.

Classes take a lot of work to create, so they should be developed only whenthey’re addressing specific needs.• The topic is relatively stable. Updating class materials is a lot of work, so if thesubject is rapidly evolving, other forms of sharing knowledge will have a betterbang for the buck.• The topic benefits from having teachers available to answer questions and providepersonalized help. If students can easily learn without directed help, selfservemediums like documentation or recordings are more efficient. A number ofintroductory classes at Google also have self-study versions.• There is enough demand to offer the class regularly. Otherwise, potential learnerswill get the information they need in other ways rather than waiting for the class.

At Google, this is particularly a problem for small, geographically remote offices.

Documentation

Documentation is written knowledge whose primary goal is to help its readers learnsomething. Not all written knowledge is necessarily documentation, although it canbe useful as a paper trail. For example, it’s possible to find an answer to a problem in amailing list thread, but the primary goal of the original question on the thread was toseek answers, and only secondarily to document the discussion for others.

Scaling Your Knowledge: You Always Have Something to Teach | 537 See “The Boy Scout Rule” and Kevlin Henney, 97 Things Every Programmer Should Know (Boston: O’Reilly,2010).8 g3doc stands for “google3 documentation.” google3 is the name of the current incarnation of Google’s monolithicsource repository.

In this section, we focus on spotting opportunities for contributing to and creatingformal documentation, from small things like fixing a typo to larger efforts such asdocumenting tribal knowledge.

For a more comprehensive discussion of documentation, see

Chapter 10.

Updating documentation

The first time you learn something is the best time to see ways that the existing documentationand training materials can be improved. By the time you’ve absorbed andunderstood a new process or system, you might have forgotten what was difficult orwhat simple steps were missing from the “Getting Started” documentation. At thisstage, if you find a mistake or omission in the documentation, fix it! Leave the campgroundcleaner than you found it,7 and try to update the documents yourself, evenwhen that documentation is owned by a different part of the organization.

At Google, engineers feel empowered to update documentation regardless of whoowns it—and we often do—even if the fix is as small as correcting a typo. This level ofcommunity upkeep increased notably with the introduction of g3doc,8 which made itmuch easier for Googlers to find a documentation owner to review their suggestion.

It also leaves an auditable trail of change history no different than that for code.

Creating documentation

As your proficiency grows, write your own documentation and update existing docs.

For example, if you set up a new development flow, document the steps. You can thenmake it easier for others to follow in your path by pointing them to your document.

Even better, make it easier for people to find the document themselves. Anysufficiently undiscoverable or unsearchable documentation might as well not exist.

This is another area in which g3doc shines because the documentation is predictablylocated right next to the source code, as opposed to off in an (unfindable) documentor webpage somewhere.

Finally, make sure there’s a mechanism for feedback. If there’s no easy and direct wayfor readers to indicate that documentation is outdated or inaccurate, they are likelynot to bother telling anyone, and the next newcomer will come across the same prob‐54 | Chapter 3: Knowledge Sharinglem. People are more willing to contribute changes if they feel that someone willactually notice and consider their suggestions. At Google, you can file a documentationbug directly from the document itself.

In addition, Googlers can easily leave comments on g3doc pages. Other Googlers cansee and respond to these comments and, because leaving a comment automaticallyfiles a bug for the documentation owner, the reader doesn’t need to figure out who tocontact.

Promoting documentation

Traditionally, encouraging engineers to document their work can be difficult. Writingdocumentation takes time and effort that could be spent on coding, and the benefitsthat result from that work are not immediate and are mostly reaped by others. Asymmetricaltrade-offs like these are good for the organization as a whole given that manypeople can benefit from the time investment of a few, but without good incentives, itcan be challenging to encourage such behavior. We discuss some of these structuralincentives in the section “Incentives and recognition” on page 57.

However, a document author can often directly benefit from writing documentation.

Suppose that team members always ask you for help debugging certain kinds of productionfailures. Documenting your procedures requires an upfront investment oftime, but after that work is done, you can save time in the future by pointing teammembers to the documentation and providing hands-on help only when needed.

Writing documentation also helps your team and organization scale. First, the informationin the documentation becomes canonicalized as a reference: team memberscan refer to the shared document and even update it themselves. Second, the canonicalizationmay spread outside the team. Perhaps some parts of the documentation arenot unique to the team’s configuration and become useful for other teams looking toresolve similar problems.

Scaling Your Knowledge: You Always Have Something to Teach | 559 Laszlo Bock, Work Rules!: Insights from Inside Google That Will Transform How You Live and Lead (New York:

Twelve Books, 2015).10 Ibid.

Code

At a meta level, code is knowledge, so the very act of writing code can be considered aform of knowledge transcription. Although knowledge sharing might not be a directintent of production code, it is often an emergent side effect, which can be facilitatedby code readability and clarity.

Code documentation is one way to share knowledge; clear documentation not onlybenefits consumers of the library, but also future maintainers. Similarly, implementationcomments transmit knowledge across time: you’re writing these commentsexpressly for the sake of future readers (including Future You!). In terms of tradeoffs,code comments are subject to the same downsides as general documentation:they need to be actively maintained or they can quickly become out of date, as anyonewho has ever read a comment that directly contradicts the code can attest.

Code reviews (see Chapter 9) are often a learning opportunity for both author(s) andreviewer(s). For example, a reviewer’s suggestion might introduce the author to a newtesting pattern, or a reviewer might learn of a new library by seeing the author use itin their code. Google standardizes mentoring through code review with the readabilityprocess, as detailed in the case study at the end of this chapter.

Scaling Your Organization’s Knowledge

Ensuring that expertise is appropriately shared across the organization becomes moredifficult as the organization grows. Some things, like culture, are important at everystage of growth, whereas others, like establishing canonical sources of information,might be more beneficial for more mature organizations.

Cultivating a Knowledge-Sharing Culture

Organizational culture is the squishy human thing that many companies treat as anafterthought. But at Google, we believe that focusing on the culture and environmentfirst9 results in better outcomes than focusing on only the output—such as the code—of that environment.

Making major organizational shifts is difficult, and countless books have been writtenon the topic. We don’t pretend to have all the answers, but we can share specific steps

Google has taken to create a culture that promotes learning.

See the book Work Rules!10 for a more in-depth examination of Google’s culture.56 | Chapter 3: Knowledge Sharing

Respect

The bad behavior of just a few individuals can make an entire team or communityunwelcoming. In such an environment, novices learn to take their questions elsewhere,and potential new experts stop trying and don’t have room to grow. In theworst cases, the group reduces to its most toxic members. It can be difficult to recoverfrom this state.

Knowledge sharing can and should be done with kindness and respect. In tech, tolerance—or worse, reverence—of the “brilliant jerk” is both pervasive and harmful, butbeing an expert and being kind are not mutually exclusive. The Leadership section of

Google’s software engineering job ladder outlines this clearly:

Although a measure of technical leadership is expected at higher levels, not all leadershipis directed at technical problems. Leaders improve the quality of the peoplearound them, improve the team’s psychological safety, create a culture of teamworkand collaboration, defuse tensions within the team, set an example of Google’s cultureand values, and make Google a more vibrant and exciting place to work. Jerks are notgood leaders.

This expectation is modeled by senior leadership: Urs Hölzle (Senior Vice Presidentof Technical Infrastructure) and Ben Treynor Sloss (Vice President, Founder of Google

SRE) wrote a regularly cited internal document (“No Jerks”) about why Googlersshould care about respectful behavior at work and what to do about it.

Incentives and recognition

Good culture must be actively nurtured, and encouraging a culture of knowledgesharing requires a commitment to recognizing and rewarding it at a systemic level.

It’s a common mistake for organizations to pay lip service to a set of values whileactively rewarding behavior that does not enforce those values. People react to incentivesover platitudes, and so it’s important to put your money where your mouth is byputting in place a system of compensation and awards.

Google uses a variety of recognition mechanisms, from company-wide standardssuch as performance review and promotion criteria to peer-to-peer awards between

Googlers.

Our software engineering ladder, which we use to calibrate rewards like compensationand promotion across the company, encourages engineers to share knowledge bynoting these expectations explicitly. At more senior levels, the ladder explicitly callsout the importance of wider influence, and this expectation increases as seniorityincreases. At the highest levels, examples of leadership include the following:• Growing future leaders by serving as mentors to junior staff, helping themdevelop both technically and in their Google role

Scaling Your Organization’s Knowledge | 5711 Peer bonuses include a cash award and a certificate as well as being a permanent part of a Googler’s awardrecord in an internal tool called gThanks.• Sustaining and developing the software community at Google via code anddesign reviews, engineering education and development, and expert guidance toothers in the field

See Chapters 5 and 6 for more on leadership.

Job ladder expectations are a top-down way to direct a culture, but culture is alsoformed from the bottom up. At Google, the peer bonus program is one way weembrace the bottom-up culture. Peer bonuses are a monetary award and formal recognitionthat any Googler can bestow on any other Googler for above-and-beyondwork.11 For example, when Ravi sends a peer bonus to Julia for being a top contributorto a mailing list—regularly answering questions that benefit many readers—he ispublicly recognizing her knowledge-sharing work and its impact beyond her team.

Because peer bonuses are employee driven, not management driven, they can have animportant and powerful grassroots effect.

Similar to peer bonuses are kudos: public acknowledgement of contributions (typicallysmaller in impact or effort than those meriting a peer bonus) that boost the visibilityof peer-to-peer contributions.

When a Googler gives another Googler a peer bonus or kudos, they can choose tocopy additional groups or individuals on the award email, boosting recognition of thepeer’s work. It’s also common for the recipient’s manager to forward the award emailto the team to celebrate one another’s achievements.

A system in which people can formally and easily recognize their peers is a powerfultool for encouraging peers to keep doing the awesome things they do. It’s not thebonus that matters: it’s the peer acknowledgement.

Establishing Canonical Sources of Information

Canonical sources of information are centralized, company-wide corpuses of informationthat provide a way to standardize and propagate expert knowledge. Theywork best for information that is relevant to all engineers within the organization,which is otherwise prone to information islands. For example, a guide to setting up a58 | Chapter 3: Knowledge Sharing12 Such as books about software engineering at Google.13 See Chapter 9.14 See Chapter 11.15 Available for multiple languages. Externally available for C++ at https://abseil.io/tips.basic developer workflow should be made canonical, whereas a guide for running alocal Frobber instance is more relevant just to the engineers working on Frobber.

Establishing canonical sources of information requires higher investment than maintainingmore localized information such as team documentation, but it also hasbroader benefits. Providing centralized references for the entire organization makesbroadly required information easier and more predictable to find and counters problemswith information fragmentation that can arise when multiple teams grapplingwith similar problems produce their own—often conflicting—guides.

Because canonical information is highly visible and intended to provide a sharedunderstanding at the organizational level, it’s important that the content is activelymaintained and vetted by subject matter experts. The more complex a topic, the morecritical it is that canonical content has explicit owners. Well-meaning readers mightsee that something is out of date but lack the expertise to make the significant structuralchanges needed to fix it, even if tooling makes it easy to suggest updates.

Creating and maintaining centralized, canonical sources of information is expensiveand time consuming, and not all content needs to be shared at an organizationallevel. When considering how much effort to invest in this resource, consider youraudience. Who benefits from this information? You? Your team? Your product area?

All engineers?

Developer guides

Google has a broad and deep set of official guidance for engineers, including styleguides, official software engineering best practices,12 guides for code review13 and testing,14 and Tips of the Week (TotW).15

The corpus of information is so large that it’s impractical to expect engineers to readit all end to end, much less be able to absorb so much information at once. Instead, ahuman expert already familiar with a guideline can send a link to a fellow engineer,who then can read the reference and learn more. The expert saves time by not needingto personally explain a company-wide practice, and the learner now knows thatthere is a canonical source of trustworthy information that they can access whenevernecessary. Such a process scales knowledge because it enables human experts to recognizeand solve a specific information need by leveraging common, scalableresources.

Scaling Your Organization’s Knowledge | 5916 go/ links are unrelated to the Go language.17 External codelabs are available at https://codelabs.developers.google.com.go/ linksgo/ links (sometimes referred to as goto/ links) are Google’s internal URL shortener.16

Most Google-internal references have at least one internal go/ link. For example, “go/spanner” provides information about Spanner, “go/python” is Google’s Python developerguide. The content can live in any repository (g3doc, Google Drive, Google

Sites, etc.), but having a go/ link that points to it provides a predictable, memorableway to access it. This yields some nice benefits:• go/ links are so short that it’s easy to share them in conversation (“You shouldcheck out go/frobber!”). This is much easier than having to go find a link andthen send a message to all interested parties. Having a low-friction way to sharereferences makes it more likely that that knowledge will be shared in the firstplace.• go/ links provide a permalink to the content, even if the underlying URLchanges. When an owner moves content to a different repository (for example,moving content from a Google doc to g3doc), they can simply update the go/link’s target URL. The go/ link itself remains unchanged.go/ links are so ingrained into Google culture that a virtuous cycle has emerged: a

Googler looking for information about Frobber will likely first check go/frobber. Ifthe go/ link doesn’t point to the Frobber Developer Guide (as expected), the Googlerwill generally configure the link themselves. As a result, Googlers can usually guessthe correct go/ link on the first try.

Codelabs

Google codelabs are guided, hands-on tutorials that teach engineers new concepts orprocesses by combining explanations, working best-practice example code, and codeexercises.17 A canonical collection of codelabs for technologies broadly used across

Google is available at go/codelab. These codelabs go through several rounds of formalreview and testing before publication. Codelabs are an interesting halfway pointbetween static documentation and instructor-led classes, and they share the best andworst features of each. Their hands-on nature makes them more engaging than traditionaldocumentation, but engineers can still access them on demand and completethem on their own; but they are expensive to maintain and are not tailored to thelearner’s specific needs.60 | Chapter 3: Knowledge Sharing

Static analysis

Static analysis tools are a powerful way to share best practices that can be checkedprogrammatically. Every programming language has its own particular static analysistools, but they have the same general purpose: to alert code authors and reviewers toways in which code can be improved to follow style and best practices. Some tools goone step further and offer to automatically apply those improvements to the code.

See Chapter 20 for details on static analysis tools and how they’reused at Google.

Setting up static analysis tools requires an upfront investment, but as soon as they arein place, they scale efficiently. When a check for a best practice is added to a tool,every engineer using that tool becomes aware of that best practice. This also frees upengineers to teach other things: the time and effort that would have gone into manuallyteaching the (now automated) best practice can instead be used to teach somethingelse. Static analysis tools augment engineers’ knowledge. They enable anorganization to apply more best practices and apply them more consistently thanwould otherwise be possible.

Staying in the Loop

Some information is critical to do one’s job, such as knowing how to do a typicaldevelopment workflow. Other information, such as updates on popular productivitytools, is less critical but still useful. For this type of knowledge, the formality of theinformation sharing medium depends on the importance of the information beingdelivered. For example, users expect official documentation to be kept up to date, buttypically have no such expectation for newsletter content, which therefore requiresless maintenance and upkeep from the owner.

Newsletters

Google has a number of company-wide newsletters that are sent to all engineers,including EngNews (engineering news), Ownd (Privacy/Security news), and Google’s

Greatest Hits (report of the most interesting outages of the quarter). These are a goodway to communicate information that is of interest to engineers but isn’t mission critical.

For this type of update, we’ve found that newsletters get better engagement whenthey are sent less frequently and contain more useful, interesting content. Otherwise,newsletters can be perceived as spam.

Even though most Google newsletters are sent via email, some are more creative intheir distribution. Testing on the Toilet (testing tips) and Learning on the Loo (produc‐

Scaling Your Organization’s Knowledge | 61tivity tips) are single-page newsletters posted inside toilet stalls. This unique deliverymedium helps the Testing on the Toilet and Learning on the Loo stand out from othernewsletters, and all issues are archived online.

See Chapter 11 for a history of how Testing on the Toilet came to be.

Communities

Googlers like to form cross-organizational communities around various topics toshare knowledge. These open channels make it easier to learn from others outsideyour immediate circle and avoid information islands and duplication. Google Groupsare especially popular: Google has thousands of internal groups with varying levels offormality. Some are dedicated to troubleshooting; others, like the Code Health group,are more for discussion and guidance. Internal Google+ is also popular among Googlersas a source of informal information because people will post interesting technicalbreakdowns or details about projects they are working on.

Readability: Standardized Mentorship

Through Code Review

At Google, “readability” refers to more than just code readability; it is a standardized,

Google-wide mentorship process for disseminating programming language best practices.

Readability covers a wide breadth of expertise, including but not limited to languageidioms, code structure, API design, appropriate use of common libraries,documentation, and test coverage.

Readability started as a one-person effort. In Google’s early days, Craig Silverstein(employee ID #3) would sit down in person with every new hire and do a line-by-line“readability review” of their first major code commit. It was a nitpicky review thatcovered everything from ways the code could be improved to whitespace conventions.

This gave Google’s codebase a uniform appearance but, more important, ittaught best practices, highlighted what shared infrastructure was available, andshowed new hires what it’s like to write code at Google.

Inevitably, Google’s hiring rate grew beyond what one person could keep up with. Somany engineers found the process valuable that they volunteered their own time toscale the program. Today, around 20% of Google engineers are participating in thereadability process at any given time, as either reviewers or code authors.62 | Chapter 3: Knowledge Sharing18 A changelist is a list of files that make up a change in a version control system. A changelist is synonymouswith a changeset.

What Is the Readability Process?

Code review is mandatory at Google. Every changelist (CL)18 requires readabilityapproval, which indicates that someone who has readability certification for that languagehas approved the CL. Certified authors implicitly provide readability approvalof their own CLs; otherwise, one or more qualified reviewers must explicitly givereadability approval for the CL. This requirement was added after Google grew to apoint where it was no longer possible to enforce that every engineer received codereviews that taught best practices to the desired rigor.

See Chapter 9 for an overview of the Google code review processand what Approval means in this context.

Within Google, having readability certification is commonly referred to as “havingreadability” for a language. Engineers with readability have demonstrated that theyconsistently write clear, idiomatic, and maintainable code that exemplifies Google’sbest practices and coding style for a given language. They do this by submitting CLsthrough the readability process, during which a centralized group of readabilityreviewers review the CLs and give feedback on how much it demonstrates the variousareas of mastery. As authors internalize the readability guidelines, they receive fewerand fewer comments on their CLs until they eventually graduate from the processand formally receive readability. Readability brings increased responsibility: engineerswith readability are trusted to continue to apply their knowledge to their owncode and to act as reviewers for other engineers’ code.

Around 1 to 2% of Google engineers are readability reviewers. All reviewers are volunteers,and anyone with readability is welcome to self-nominate to become a readabilityreviewer. Readability reviewers are held to the highest standards because theyare expected not just to have deep language expertise, but also an aptitude for teachingthrough code review. They are expected to treat readability as first and foremost amentoring and cooperative process, not a gatekeeping or adversarial one. Readabilityreviewers and CL authors alike are encouraged to have discussions during the reviewprocess. Reviewers provide relevant citations for their comments so that authors canlearn about the rationales that went into the style guidelines (“Chesterson’s fence”). Ifthe rationale for any given guideline is unclear, authors should ask for clarification(“ask questions”).

Readability: Standardized Mentorship Through Code Review | 6319 As of 2019, just the Google C++ style guide is 40 pages long. The secondary material making up the completecorpus of best practices is many times longer.20 For why Google uses a monorepo, see https://cacm.acm.org/magazines/2016/7/204032-why-google-storesbillionsof-lines-of-code-in-a-single-repository/fulltext. Note also that not all of Google’s code lives within themonorepo; readability as described here applies only to the monorepo because it is a notion of withinrepositoryconsistency.

Readability is deliberately a human-driven process that aims to scale knowledge in astandardized yet personalized way. As a complementary blend of written and tribalknowledge, readability combines the advantages of written documentation, whichcan be accessed with citable references, with the advantages of expert human reviewers,who know which guidelines to cite. Canonical guidelines and language recommendationsare comprehensively documented—which is good!—but the corpus ofinformation is so large19 that it can be overwhelming, especially to newcomers.

Why Have This Process?

Code is read far more than it is written, and this effect is magnified at Google’s scaleand in our (very large) monorepo.20 Any engineer can look at and learn from thewealth of knowledge that is the code of other teams, and powerful tools like Kythemake it easy to find references throughout the entire codebase (see Chapter 17). Animportant feature of documented best practices (see Chapter 8) is that they provideconsistent standards for all Google code to follow. Readability is both an enforcementand propagation mechanism for these standards.

One of the primary advantages of the readability program is that it exposes engineersto more than just their own team’s tribal knowledge. To earn readability in a givenlanguage, engineers must send CLs through a centralized set of readability reviewerswho review code across the entire company. Centralizing the process makes a significanttrade-off: the program is limited to scaling linearly rather than sublinearly withorganization growth, but it makes it easier to enforce consistency, avoid islands, andavoid (often unintentional) drifting from established norms.

The value of codebase-wide consistency cannot be overstated: even with tens of thousandsof engineers writing code over decades, it ensures that code in a given languagewill look similar across the corpus. This enables readers to focus on what the codedoes rather than being distracted by why it looks different than code that they’re usedto. Large-scale change authors (see Chapter 22) can more easily make changes acrossthe entire monorepo, crossing the boundaries of thousands of teams. People canchange teams and be confident that the way that the new team uses a given languageis not drastically different than their previous team.64 | Chapter 3: Knowledge Sharing21 For this reason, code that is known to have a short time span is exempt from readability requirements. Examplesinclude the experimental/ directory (explicitly designated for experimental code and cannot push to production)and the Area 120 program, a workshop for Google’s experimental products.

These benefits come with some costs: readability is a heavyweight process comparedto other mediums like documentation and classes because it is mandatory andenforced by Google tooling (see Chapter 19). These costs are nontrivial and includethe following:• Increased friction for teams that do not have any team members with readability,because they need to find reviewers from outside their team to give readabilityapproval on CLs.• Potential for additional rounds of code review for authors who need readabilityreview.• Scaling disadvantages of being a human-driven process. Limited to scaling linearlyto organization growth because it depends on human reviewers doing specializedcode reviews.

The question, then, is whether the benefits outweigh the costs. There’s also the factorof time: the full effect of the benefits versus the costs are not on the same timescale.

The program makes a deliberate trade-off of increased short-term code-reviewlatency and upfront costs for the long-term payoffs of higher-quality code,repository-wide code consistency, and increased engineer expertise. The longer timescaleof the benefits comes with the expectation that code is written with a potentiallifetime of years, if not decades.21

As with most—or perhaps all—engineering processes, there’s always room forimprovement. Some of the costs can be mitigated with tooling. A number of readabilitycomments address issues that could be detected statically and commented onautomatically by static analysis tooling. As we continue to invest in static analysis,readability reviewers can increasingly focus on higher-order areas, like whether a particularblock of code is understandable by outside readers who are not intimatelyfamiliar with the codebase instead of automatable detections like whether a line hastrailing whitespace.

But aspirations aren’t enough. Readability is a controversial program: some engineerscomplain that it’s an unnecessary bureaucratic hurdle and a poor use of engineertime. Are readability’s trade-offs worthwhile? For the answer, we turned to our trusty

Engineering Productivity Research (EPR) team.

Readability: Standardized Mentorship Through Code Review | 6522 This includes controlling for a variety of factors, including tenure at Google and the fact that CLs for authorswho do not have readability typically need additional rounds of review compared to authors who already havereadability.

The EPR team performed in-depth studies of readability, including but not limited towhether people were hindered by the process, learned anything, or changed theirbehavior after graduating. These studies showed that readability has a net positiveimpact on engineering velocity. CLs by authors with readability take statistically significantlyless time to review and submit than CLs by authors who do not have readability.22 Self-reported engineer satisfaction with their code quality—lacking moreobjective measures for code quality—is higher among engineers who have readabilityversus those who do not. A significant majority of engineers who complete the programreport satisfaction with the process and find it worthwhile. They report learningfrom reviewers and changing their own behavior to avoid readability issues whenwriting and reviewing code.

For an in-depth look at this study and Google’s internal engineeringproductivity research, see Chapter 7.

Google has a very strong culture of code review, and readability is a natural extensionof that culture. Readability grew from the passion of a single engineer to a formalprogram of human experts mentoring all Google engineers. It evolved and changedwith Google’s growth, and it will continue to evolve as Google’s needs change.

Conclusion

Knowledge is in some ways the most important (though intangible) capital of a softwareengineering organization, and sharing of that knowledge is crucial for makingan organization resilient and redundant in the face of change. A culture that promotesopen and honest knowledge sharing distributes that knowledge efficientlyacross the organization and allows that organization to scale over time. In most cases,investments into easier knowledge sharing reap manyfold dividends over the life of acompany.66 | Chapter 3: Knowledge Sharing

TL;DRs• Psychological safety is the foundation for fostering a knowledge-sharingenvironment.• Start small: ask questions and write things down.• Make it easy for people to get the help they need from both human experts anddocumented references.• At a systemic level, encourage and reward those who take time to teach andbroaden their expertise beyond just themselves, their team, or their organization.• There is no silver bullet: empowering a knowledge-sharing culture requires acombination of multiple strategies, and the exact mix that works best for yourorganization will likely change over time.