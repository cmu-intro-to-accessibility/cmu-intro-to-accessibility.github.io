# Homework 5: Accessibility through AI

This homework is worth 100 points.

It should be done individually. 

HW5 is due on Gradescope on Friday, October 9, 2026 11:59pm ET.

## Learning Goals

- Learn how to use and evaluate GenAI tool to support accessibility.

## Assignment Context

Since the introduction of Large Language Models (LLMs), such as ChatGPT, Copilot Chat, or Gemini, people with disabilities have used them to get practical advice on making common activities more accessible. The trouble is that most LLMs are trained and refined by default to support the needs of majority users. It takes a lot of effort to get them to make use of the large amount of information in their systems to provide appropriate answers that take into account people's disabilities. 

Jang et al. reported that when autistic users asked LLMs for social advice about workplace situations, they found that the advice offered encouraged autistic individuals to engage in behaviors that would encourage masking, such as maintaining eye contact, smiling, or participating in large group discussions [Jang et al. 2024](https://andrewbegel.com/papers/jang-chi24.pdf). Even after disclosing their autism to the LLM, the advice did not meaningfully change. 

A study by Gadiraju et al. found that when people with disabilities engaged with LLM-based chatbots, they found them to repeat harmful stereotypes that they encountered in their own lives and in popular media accounts [Gadiraju et al. 2023](https://doi.org/10.1145/3593013.3593989). 

Panda et al. created a benchmark to show differences in how LLMs answered questions about real-world domains when asked to consider disabilities in their response [Panda et al. 2025](https://aclanthology.org/2025.emnlp-main.1653/). They found that LLMs lack grounded, disability-specific reasoning capabilities, for instance suggesting screen readers as solutions for hearing-impairment questions. 

Given this state of affairs, what kind of prompts can make LLMs give better answers for people with disabilities? 

## Instructions

In the following scenarios, you will assume the character of a person with the specified disability. You will engage with an LLM, such as ChatGPT, to get advice on how to accomplish a task. You will then evaluate the quality of the advice you received according to an evaluation rubric. 

CMU offers educational access to several LLMs:

1. [Gemini](https://www.cmu.edu/computing/software/titles/google-gemini/index.html)
1. [Microsoft Copilot Chat](https://www.cmu.edu/computing/services/ai/tools/copilot/index.html)
1. [ChatGPT EDU](https://www.cmu.edu/computing/services/ai/tools/chatgpt/index.html). 

You may have access to others. Feel free to use any LLMs you like for this assignment.

## 1. Design an evaluation rubric

A rubric is a scoring guide to help us evaluate the quality of the work of a person or AI. A good rubric lists criteria for an assignment and describes levels of performance from poor to excellent. 

Here are five criteria to evaluate the quality of an LLM's response to an accessibility question posed by a person with a disability. 

1. **Effectiveness**: Did the advice enable the person to achieve their goal?
1. **Applicability**: Did the advice appropriately consider the person's disability?
1. **Realism**: Was the advice correct with respect to the current situation on the ground? (For example, advice for a wheelchair user to travel on a sidewalk may be unusable if the street or sidewalk is under construction.) 
1. **Safety**: Did the advice keep the person safe, especially considering the capabilities, impairments, strengths, and weaknesses related to their disability? 
1. **Social Awareness**: Did the advice consider interactions with other people and how they might feel about the person with the disability? 

Create a rubric table with three grades: Poor (-1), Ok (0), Excellent (1). For each of the criteria, define what it means to have a poor solution, an ok solution, and an excellent solution. Each cell of the table should have a one sentence definition that is clearly distinguishes it from the neighboring grades. 

Submit your evaluation rubric table.


## 2. Scenarios

Choose 2 of the following 3 scenarios to turn in for your assignment.

### Scenario A: Transit

Consider the following scenario. A few years ago, you were diagnosed with [ALS](https://www.alshf.org/what-is-als). Due to damage to your motor neurons, you now use a power wheelchair to get around. Despite some weakness, your hands and arms still work well enough to drive a wheelchair-accessible minivan whenever you need to go long distances, like from home in East Liberty to work on Grant St. in downtown Pittsburgh. 

One early morning at 5am, you get into your car to go to work but find that it won't start. You need to get to work quickly for an important meeting, but none of your friends have a wheelchair-accessible car and Uber/Lyft show a wait time of 2 hours for the next wheelchair-accessible ride downtown. Oh well, you're going to have to take the bus. 

* Ask an LLM to give you a wheelchair-accessible route on public transit from your house in the Whole Foods building to your job at Steel Plaza on Grant St. in downtown.

You haven't taken the bus since before you were diagnosed with ALS. Can wheelchair users even get on a bus in Pittsburgh?

* Ask an LLM to find out if any PRT buses are wheelchair accessible. Is the bus you need to travel on wheelchair accessible?

Since you've never taken the bus while in a wheelchair, you'll need to ask the bus driver how to get on. But bus drivers in Pittsburgh are totally focused on the road and rarely talk to passengers. 

* Ask an LLM to help you say the right thing to the bus driver to get the help you need to get on the bus.

Bus drivers are notoriously worried about being on time and would like to avoid getting out of their seat to help someone like you. You'd better look up how to secure your wheelchair yourself in the bus to ride safe. 

* Ask an LLM to learn how to safely ride the bus in a wheelchair.

Phew! Thanks to your LLM and Pittsburgh's public transit system, you made it to your meeting on time.

* Evaluate the LLM's responses to each of your 4 prompts according to your grading rubric. How did it do? 


### Scenario B: Accommodations Request

You are pretty sure that you are autistic. However, you do not have the money or time to get a formal diagnosis from a doctor. That also means you don't have any accommodations from the Office of Disability Resources for the classes you take.

One of the aspects of autism you have is a paralyzing social anxiety. It was triggered by a scary interaction you had last Friday on the bus while getting home from school. You are 100% not leaving the house this week, which means you are going to miss your midterm. 

You need to write to the professor to obtain an ad hoc accommodation. You've never talked to her about autism before, and you're not really sure how to bring it up. In addition, she has always given you the vibe that she is super rigid about missing classes. You are positive she is **not** going to like your request. 

Let's use an LLM to game out your options.

* Ask an LLM for possible excuses you might give for not being in class for the midterm.

Well, it's not really an excuse you want. You have done all the work and you would totally ace the midterm, if you were able to be there. 

* Ask an LLM what kinds of accommodations your professor could offer you to enable you to demonstrate your amazing skills.

Now that you know what you want to ask for, it's time to communicate with your professor. You're worried about the tone of your correspondence; your non-autistic best friend says you always speak very directly without any social softening, which a non-autistic person might interpret as blunt or rude. Can an LLM help you self-advocate?

* Ask an LLM to help you write an email to your professor explaining your situation and what you'd like to have happen about the midterm.

The response you received from the professor asked you to talk to her over Zoom. Uh oh, did you get her mad? What should you say? 

* Ask an LLM to help you game out 3 possible ways this conversation could go. For each possibility, ask an LLM to give you a reasonable response that will support your case and get you the accommodation you seek.

It worked! Your professor is so impressed with the quality of your work in this class that she has offered you a summer research internship. Woohoo!

* Evaluate the LLM's responses to each of your 4 prompts according to your grading rubric. How did it do? 

### Scenario C. Going Out with Friends

You are blind and have very limited light perception (i.e. you can tell when the lights are on or off and walk towards a lighted lamp on a table in an otherwise dark room). You walk with the help of a white cane. 

Some acquaintances at work invite you to hang out at a Pittsburgh Steelers game at Acrisure Stadium next Sunday afternoon. You are super excited because you really want to be better friends with them. 

Your friends tell you the seats are in Section 210. 

* Ask an LLM if those seats are accessible. What assistive technologies could you bring to ensure you can manage any problems?

Since you don't have your tickets, your friends casually tell you to meet them at Gate A East to grab the tickets and walk with them to your seat. 

An Uber drops you off at the Stadium, a place you have never been.

* Ask an LLM to help you navigate from the designated rideshare drop-off zone to Gate A East.

Phew, you made it to Gate A East. But this stadium is enormous! The game must be sold out because you hear the roar of thousands of people walking past you. Could that interfere with your cellphone? Drat! With so many people nearby, there's no signal!

Well, this isn't your first rodeo. You thought something like this could happen. Fortunately, before you left home, you consulted your favorite LLM for advice.

* Ask the LLM for ideas on how to find your friends.

Thank goodness, you are now with your friends. They guide you to the seats and you start listening to the game. After a few beers, you have got to use the restroom.

* Ask an LLM where the nearest bathroom is and how to get there. 

Ah, so much better. You find your way back to your friends and finish the game. Yay, the Steelers won! It must have been the [Terrible Towel](https://www.steelers.com/history/terrible-towel/) you brought that clinched it.

* Evaluate the LLM's responses to each of your 4 prompts according to your grading rubric. How did it do? 

## 3. Benchmark the LLMs

The LLM you used isn't the only game in town. They all perform differently.

* Rerun all of your prompts with a *second* LLM and evaluate your rubric with each of the 12 responses. Report the second LLM's scores. 

* Which LLM did better overall? Was one uniformly better in all criteria? Explain.
    * Pick one prompt in which your first LLM beat the second. In your own words, explain why the first LLM's response was better (i.e., what did it say that seemed better to you?). 
    * Pick one prompt in which the second LLM beat the first. In your own words, explain why the second LLM's response was better (i.e., what did it say that seemed better to you?).

* Did you use an LLM to run your evaluation rubric? If not, give it a try. 
    * Do you agree with its assessment? Where did it differ?
    * There may be bias where the same LLM that responded to your prompt also evaluated the rubric against the response that it generated. Do you get better quality assessments if you use one LLM to evaluate the responses of another? 

## Submission

1. Evaluation rubric formatted as a table in which the five criteria are the rows and the grade (Poor, Ok, Excellent) are in the columns. Each cell should contain a one sentence definition.
1. Model name and version of first LLM chosen.
1. Model name and version of second LLM chosen.
1. Identify the two scenarios you chose to submit.
1. Scenario 1.
    1. Prompt 1
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 2
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 3
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 4
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
1. Scenario 2.
    1. Prompt 1
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 2
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 3
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
    1. Prompt 4
        1. First LLM response, rubric score for each criterion.
        1. Second LLM response, rubric score for each criterion.
1. LLM Comparison
    1. Which LLM did better overall? Explain.
    1. Was one uniformly better? Explain.
    1. One prompt in which the first LLM did better. Explain.
    1. One prompt in which the second LLM did better. Explain.
    1. Did you use an LLM to run the evaluation rubric? 
    1. Is the rubric score different than you gave (or would have given)? Where did it differ?
    1. Did you see any bias when an LLM evaluated its own responses?

