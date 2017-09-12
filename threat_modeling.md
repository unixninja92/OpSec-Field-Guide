#Threat Modeling
###Designing Security Around *You*

>It does not do to leave a live dragon out of your calculations, if you live near him.
>
>J.R.R. Tolkien

#####Give It to Me Straight
So, you may be wondering, 'What is threat modeling, and why is it important?'

To keep things brief, Threat Modeling is one of many approaches to visualizing a scenario so that we can make better decisions with regard to security.

Specifically, it involves making note of all of the things you want to protect, and then imagining all the ways they can be at risk.
Thus the name.
We are analyzing ***threats*** to ***model*** a scenario.
Get it?

 Throughout these tutorials we will be emphasizing this approach, as we believe it is simple, thorough, and versatile.

#####How it Works
In its simplest form, a threat model consists of only two steps:

1. Identifying what you want to protect
2. Determining who (or what) might threaten those things

Moving forward, we will refer to the things we are trying to protect as **assets** and the people or groups trying to get them as **adversaries**.
We promise, that's the only jargon you'll have to remember to make this work!

So, rather than go into some dry, rambling, textbook definitions, let's jump right in and see how this works with an example:

#####Case Study: The Commute

As we have already mentioned, part of what makes the threat modeling approach so robust is its versatility.
While these tutorials will generally focus on information security, one can threat model anything that needs to be secured.

Because, at this point, we may not know enough about information security to threat model around that, let's instead threat model for something almost all of us can relate to: Commuting to work.

######Some Background information

The situation is this: You are getting ready for work.
You are going to drive your car to work.
The weather is nice, and you're in good health.

Despite this good fortune, driving is risky business. So together, we are going to threat model your daily commute, and figure out where the risks lie.

######Determining what's most important

Let's recall the first step of threat modeling:

>1. Identifying what you want to protect

Remember that we call the things we want to protect **assets**.

What might one consider an asset when they are about to step in a car?
A lot of things, sure!
For example:

+ Your life and physical health
+ The safety of others
+ Your reputation at work (don't be late!)
+ Your drivers license
+ The condition of your car

We could easily continue the threat modeling process for each one of these assets, but that's out of the scope of this example.
Instead, we will pick one to focus on.

>+ Your drivers license

Now that's an asset worth protecting!
Being able to drive is the first step towards securing your commute.

With that settled, we continue on to defining adversaries, the bread-and-butter of threat modeling.

######Defining the Adversary

We've got something to fight for now.
But what are we up against in our endeavor to protect ourselves?
That brings us to step two of the threat modeling process:

>2. Determining who (or what) might threaten those things

We call that who/what the **adversary**.

In information security, an adversary might be a manager trying to spy on your internet activity, or a government trying to record a secret meeting.
For our driving example, we want to consider people or groups that could put your license at risk.

Of course, the most likely adversary we will face with regard to hanging on to our license would be law enforcement.

If we stopped there, we wouldn't have created a very robust model at all.
Yes, it's true that we value our license as an asset, and that law enforcement is a potential adversary to that asset, but that doesn't quite analyze the situation very thoroughly.
What we must do now is take a critical look at our adversary.
We will achieve this with a super simple acronym: **CALI**.

+ **C** apabilities - What *CAN* they do?
+ **A** ctions  - What *ARE* they doing?
+ **L** imitations - What *CAN'T* they do?
+ **I** ntentions - What do they *WANT*?

Breaking this down for law enforcement, we could come up with the following example:

+ Capabilities: They can pull you over, arrest you, and testify against you.
+ Actions: Patrolling the streets, setting up speed traps, performing traffic checkpoints.
+ Limitations: They cannot (theoretically) do anything illegal. The limits of their tactics are publicly defined in the law.
+ Intentions: Police may intend to ticket you to meet a quota, to harass you, or simply to stop unsafe driving.

This information provides a much more accurate image for us to design our security practices around.
We can put together our analysis of the assets and adversaries into a simple problem-statement around which we design our security practices:

*While commuting, I intend to protect the status of my drivers license.*
*Law enforcement serves as my primary adversary in this endeavor, because they may intend to fine me in order to meet a quota.*
*To achieve this, they could set up speed traps on the highway to catch me speeding, or use checkpoints to verify my inspection and registration tags.*
*However, they must follow the law to the letter during these processes, which could be helpful to my strategy.*

#####Where do I go from here?

Once you've done this for the assets and adversaries you're done developing your threat model.
Congratulations!

Having a threat model properly established means that the measures you take to secure your assets are much less likely to leave any side of your assets unprotected.
Exactly how to secure those assets is not important at this stage.
So congratulations, you're done!

###FAQ
+ I can come up with a lot of assets and adversaries. Do I really have to do all of this for each one of them?
  + **No, it is up to you to determine how thorough your threat model is.** Not all assets are created equal. You probably care more about securing your Social Security Number number than you do your lolcats.com password. Spend more time analyzing the former.


+ So I just have to do this once and I'm good?
  + **Not really!** While sittign down and doing a thorough, formally thought-out threat model is only necessary on occasion, things are changing all the time, and it's important to be critical of what that means for your situation. Sticking to the driving example, assume midway through your drive one of your headlights burns out. You need to quickly account for this change in situation. How does it affect your level of risk? How can your adversary use it against you?
