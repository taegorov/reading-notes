### Link Home:
[Home](README.md)

# Reading Notes Code 401: Prep: Readings

## How to Solve Programming Problems

The author recommends a 'measure twice cut once' approach to problem solving in coding. Understand the problem thoroughly before attempting to solve it.

#### Steps for problem solving, *most of your time will be spent on steps 1-3*:


> 1. Read the problem completely twice.

- You might want to do this even more than twice! You should be able to explain the problem well to someone else. Don't move on to the next step until you can

> 2. Solve the problem manually with 3 sets of sample data.

- Don't automate until you can do this. The author recommends doing the following steps if you were given the word "Zebra" and asked to reverse it:

> Write “Zebra” down.
> Start a new word, and put “a” as the first letter.  (Why –> because it is the last letter, we want to start here)
> Put “r” down as the 2nd letter.  (Why –> because it is the next letter backwards from the last letter we copied)
> Put “b” down as the 3rd letter.  (Why –> same as above)

> 3. Optimize the manual steps.

- Optimize the above steps for reversing the string "Zebra". The author recommends something like the following:

> Write “Zebra” down.
> Start at the last letter in the word and create a new empty word.
> Append the current letter to the new word
> If there is a previous letter, make the previous letter the current letter and start back at 3.

- This is starting to look an awful lot like code!!

> 4. Write the manual steps as comments or pseudo-code.

- This step is sometimes optional if you did steps 1-3 in a really thorough manner. However, the author recommends for beginners to do this step regardless

- We've done this in 201 and 301 -- add comments as very thorough to-do's with syntax as close to code as possible

> 5. Replace the comments or pseudo-code with real code.

- If you're struggling on this step, go back to steps 1-3/4

> 6. Optimize the real code.

- Ultimately optional


## Pretend Your Time is Worth $1,000/Hour
(and You’ll Become 100x More Productive)

> “Pretend your time is worth $1,000/hr. Would you spend five of them doing extra work for free? Would you waste one on being angry?” - Niklas Göke

The article starts with the above quote

> They spend hours watching low-quality television and social media when they should be productive and effective.See, many people could be making a fortune (if they used their time well)…but instead, they give away their time in unproductive ways that leave them broke, unhappy, and stuck.

I'm not sure if I agree with this sentiment. In my opinion, it's almost 'victim-blaming' (for lack of a better term) people who just want to unwind after a busy and productive day. I can appreciate the mentality, but I feel like people can abuse this thought process to explain away people who are poor/unsuccessful because they choose to watch some TV after a 12 hour workday (when in reality, there are other health/socioeconomic factors to consider). I acknowledge that the author will elaborate on this point further, however.

*Staying busy vs. staying focused*: I can get behind this 100%. 

> If you let people know your time is free and low-valued, people will treat it as such. But if you teach people that your time is expensive, important, and valuable, then people will respond in kind.

This seems particularly true in the professional sphere. I've utilized this mentality in the past, and it hugely benefitted my sales career since it quickly established rapport and professionalism. The author has experienced this too, and they write:

> No one responded to me. I rarely was invited to write. I think people could see how little I valued myself, and didn’t want to promote my message. I don’t even blame them... You probably need to say “no” more.

However, I will add the caveat that this could be priviliged thinking. The author mentions saying "no" to many high-paying opportunities because they're not the right fit, and quotes Warren Buffet to back this claim. Not everyone has this luxury. I feel like this article would be more powerful if people in less-privileged positions were at least addressed.


## How to Think like a Programmer

> “Everyone in this country should learn to program a computer, because it teaches you to think.” — Steve Jobs

The author points to this 'standard' method for problem solving, which is not useful for coding (and life in general):

> 1. Try a solution.
> 2. If that doesn’t work, try another one.
> 3. If that doesn’t work, repeat step 2 until you luck out.

The author recommends having a problem-solving **framework**.

"Problem-solving skills are almost unanimously the most important qualification that employers look for….more than programming languages proficiency, debugging, and system design."

Problem-solving steps:

1. Understand

Understand exactly what is being asked, and problems will be much simpler if you know exactly what's being asked of you. Write it down, doodle it, explain it to your wife/dog/friend, etc.

2. Plan

Write down the exact steps you will take to tackle the problem. Don't just start coding right away. A great way of framing this step is with the following quote:

> “Given input X, what are the steps necessary to return output Y?”

3. Divide

Don't tackle the main, larger problem all at once. Break it down into bite-size chunks. Solve those chunks one at a time, then "connect the dots." 

4. Stuck?

If you can't solve one of the bite-size chunks: debug, reassess, research.

--- 

You will only get better at this with **practice**.


## The 5 Whys
(Getting to the Root of a Problem Quickly)

Developed by the founder of Toyota Industries (still used by the company today), so it's probably pretty effective!

The quickest, and most overly-simplified explanation of what the 5Y technique is, is "...when a problem occurs, you drill down to its root cause by asking "Why?" five times" ([source](https://www.mindtools.com/pages/article/newTMC_5W.htm))

The steps are as follows:

1. Assemble a Team

These people should be familiar with the problem.

2. Define the Problem

This should simply (in one sentence?) explain the issue.

3. Ask the First "Why?"

This can be one obvious explanation, or several possible explanations. Answers should be quick phrases such as "number of goals is too high."

4. Ask "Why?" Four More Times

These should build upon the Why in step 3.

5. Know when to Stop

Eventually, the root cause is found and asking "why" doesn't generate useful responses. At this point, a "counter-measure" should be clear.

6. Address the Root Cause(s)

Decide on counter-measures.

7. Monitor Your Measures

Keep an eye on your counter-measures and see if the problem goes away.

5 Why Diagram:
![5YDiagram](https://www.mindtools.com/media/Diagrams/5_Whys_Figure_1_Single_Lane.jpg)

5 Why Diagram, multiple lanes:
![multi-lane](https://www.mindtools.com/media/Diagrams/5_Whys_Figure_2_multiple_lanes.jpg)


## What the Heck is an Event Loop Anyway?

JavaScript is a single-threaded programming langauge (one 'call stack') which means it can pretty much only do one thing at a time. When code runs, this is the default process in which it occurs:

![callstack](https://i.ytimg.com/vi/2ZH_1d8TYVg/maxresdefault.jpg)

It is relatively easy to exceed the maximum call size. When things are slow, we call that "blocking" (network requests, image processing, etc.). Our code gets stuck if the stack is blocked. 

The solution is **asynchronous callbacks**. Run some code, give it a callback, then run that chunk of code later.

Web API's do the timeout timer for us, rather than JS directly. When the web API is done with the timeout, it pushes the task to the task queue, and the task queue pushes the first thing in the event loop onto the stack. Here's what it looks like:

![callstack2](https://miro.medium.com/max/1600/1*iHhUyO4DliDwa6x_cO5E3A.gif)


## The Super Mario Effect

This video was deleted from Youtube and from Mark Rober's TED page, so I wasn't able to view it. I do love me some Mark Rober though!