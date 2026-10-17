# Homework 6: Accessibly Design with AI

This homework is worth 200 points.

It should be done individually. 

HW6 is due on Gradescope on Monday, November 2, 2026 11:00am ET.

## Learning Goals

- Learn how to find, read, and understand academic research papers to help you dive deep into a new topic.
- Map a user's journey to accomplish a goal.
- Use the user-centered design process to develop a conceptually novel user interface. 

## Assignment Context

You work for Amazon's Alexa team. After a few gangbuster years where everyone and his cousin bought an Echo Dot to put in their homes, the novelty has worn off. No one is buying anymore Echo Dots, and most current owners now use their Echo Dots just to set cooking timers.  

A consulting company hires you to find out what went wrong with the Echo Dot. Using what you learn, they want you to invent a new paradigm for an audio-first, audio-only GenAI-powered web browser they believe will reinvigorate the product (enabling Amazon to sell more powerful Echo Dots) and create new markets for everyone to make lots of money.

You believe that there's an untapped market in selling mobile, cellular-enabled, web-browsing Echo Dots to people with mobility impairments, specifically people who find it difficult to use a mouse and keyboard to control a computer and are using them in situations where they can't look at a screen. These include people who can't use their hands (e.g., paralysis, carpal tunnel syndrome, or ALS) who are traveling through the city to go to work, visit friends and family, and see the sights. 

## Instructions

This assignment has three parts. 

1. Look up academic research from the SIGCHI community to learn about the usability challenges found in audio-only user interfaces. Narrow down your search to explore use of these interfaces by people with mobility impairments. Create a list of challenges found by researchers and a matching list of strategies they found users engaging in to overcome each challenge. 
1. Contextualize the lessons academics have learned to the task at hand. Create a project brief that defines the user for whom you are designing, their goals, where they are using this mobile, wifi-enabled, audio-only web browser, and the problems they would face achieving their goals. Choose one goal and define a journey map to show how this user tries to achieve that goal. Use the challenges and lessons learned from the academic papers to contextualize your journey map to your specific user and task. 
1. Using the user-centered design process, design a new user interface to make it quick and easy to use a mobile, wifi-enbled, audio-only web browser while on the go. Brainstorm some ideas, choose a concept, and design a prototype to illustrate how it could work. Create a complete list of steps the user will take to finish one task and turn those steps into a storyboard. Explain how your design overcomes the challenges identified by the academic research and the problems identified in your journey map.
    1. If you are feeling bold, try using GenAI to create a prototype of your application. If you can make an application that enables a user to accomplish your task (and can demo that it works to the instructors), you will earn extra credit.

CMU offers educational access to several LLMs:

1. [Gemini](https://www.cmu.edu/computing/software/titles/google-gemini/index.html)
1. [Microsoft Copilot Chat](https://www.cmu.edu/computing/services/ai/tools/copilot/index.html)
1. [ChatGPT EDU](https://www.cmu.edu/computing/services/ai/tools/chatgpt/index.html). 

You may have access to others. Feel free to use any LLMs you like for this assignment.

## 1. Academic Research

Many academic researchers study human-computer interaction and accessibility. Someday, you may join this community! For now though, we want you to learn from the research that has already been conducted to help you with your task.

You will conduct a GenAI-assisted literature search for empirical HCI studies of audio-only user interfaces, such as Alexa, Cortana, or Siri. Restrict your search to studies conducted with physically disabled users. 

Consider using [Elicit](https://elicit.com), [Consensus](https://consensus.app), or [Perplexity](https://perplexity.ai) to super-charge your search over basic Gemini, ChatGPT, or Copilot chatbots. 

Create a prompt for an LLM to ask it to search the ACM SIGCHI research literature to list the top 5 challenges that users with physical disabilities have with audio-only user interfaces, like Alexa, Cortana, or Siri. Have it match those challenges with a set of strategies these users engage in to overcome the challenges. 

Read over the list. Do you believe them? Are these the most salient problems you want to give back to the consulting company that hired you? If not, try changing your prompt to be more specific about the problems you expected to find and your intended use cases to see if it can do better.  
   

## 2. Journey Map

User-centered design begins with a definition of the problem. This problem statement is then turned into a set of needs and requirements for our design. Remember, your goal as a consultant is to find the killer app for a mobile, wifi-enabled, GenAI-powered, audio-only web browsing device for people with physical impairments. 

Write a problem statement that includes answers to the following questions:

1. Who is the user? 
1. What task do they need to accomplish?
1. What problems do they have with existing solutions? 
1. How could a mobile, wifi-enabled, GenAI-powered, audio-only web browsing device solve one of their problems? 

Define a user persona to stand in for your users. This user persona is the one who will use the new device directly. You may use an LLM to help you create this user persona. 

1. Give this character a background story. What is their name? Who is in their lives? What do they like to do? Where do they live? What disabilities do they have?
1. List 2 goals this character has that involve traveling through the city to go to work, visit friends and family, and see the sights.
1. List 2 frustrations this character has experienced trying to accomplish their goals.

Create a journey map for your persona that follows them through one goal, step-by-step. It should show where things go wrong. This journal map should take the form of a table where the columns are the steps they experience in achieving their goal, and the rows are 

1. The name of step.
1. The actions the persona takes in that step.
1. The thoughts that go through their minds during that step. 
1. The emotions they are feeling in that step. Are these positive or negative?
1. The design opportunities you see to make this step better. These should be inspired by the challenges and strategies you found in your academic research contextualized to this specific persona and goal.


## 3. User-Centered Design

It's time to come up with a design for the user interface for this mobile, wifi-enabled, AI-powered, audio-only web browser device. In this step, you should brainstorm a few ideas, pick the concept you like the best, and develop it into a prototype. 

Brainstorm 3 divergent (i.e. wildly and creatively different) ways for a user to have a conversation with the new device to accomplish the goal you chose for your Journey Map. Be sure that your ideas cover all the steps and include the design opportunities you noticed in the Journey Map. The more ideas you generate, the more likely you're going to like one of them. You may use an LLM to help you come up with the ideas. 

Choose one of these ideas to orient your concept around. Describe the concept in one high-level, 80,000 foot view sentence: what it is, who iit is for, and how it works. This is best generated by your brain, not an LLM.

Enumerate the steps and actions your user will take to accomplish their goal with your design concept. Prompt an LLM to draw these out in a storyboard. Remember to tell the LLM about your user persona so it draws the right character!

Now is the fun part. Explain to the consulting firm how your concept works, how it overcomes the challenges you identified in your academic research, and how it leverages the design opportunities identified by your journey map. 


## 4. Extra Credit Opportunity

Have you ever used GenAI to create an application? These days, developers can create a working application from a single LLM prompt. Try writing a single prompt to Gemini, Claude, or Anthropic's LLMs to create a working version of your application prototype. Record a demo video of it working (and show the instructors a live demo in class). If it works, you'll receive an extra 100 points on this assignment. 


## Submission

1. Academic Research
    1. The list of the 5 challenges you found with matching strategies.
    1. A reference list in APA format of all the research papers whose information went into the creation of your list.
    1. URLs to all AI chatlogs used in this part of the assignment (i.e. prompts and responses from the AI) 
1. Journey Map
    1. Problem statement
    1. User persona
    1. Journey map
    1. URLs to all LLM chatlogs used in this part of the assignment.
1. User-Centered Design
    1. A one-sentence description of your design concept.
    1. The list of steps and actions users must take to accomplish their goal with this new device. 
    1. The storyboard (blown up to the size of an entire 8.5x11" sheet of paper (or one page in Google Docs))
    1. The explanation of your concept, challenges, and opportunities intended to be read by your boss at the consulting firm. This should be at least 500 words long --- after all, they're paying you big bucks for this concept. Earn it!
    1. URLs to all LLM chatlogs used in this part of the assignment.
1. Extra Credit (optional)
    1. URL to your code checked into a GitHub repository.
        * Be sure you have given permissions to the instructors to access this repo.
    1. URL to an 1-minute, unlisted YouTube demo video recording of your application working to accomplish your user's goal.
    1. URLs to all LLM chatlogs used to do the extra credit.