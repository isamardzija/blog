---
title: "5  Lessons Learned From A Frontend Interview (With Examples)"
seoTitle: "Frontend Interview: 5 Lessons Learned From An Actual Interview"
seoDescription: "Five of the most important takeaways that will help you ace an upcoming frontend interview & land the job."
datePublished: Wed Dec 13 2023 14:20:34 GMT+0000 (Coordinated Universal Time)
cuid: clq3uzlp7000008jngvpia0cd
slug: 5-lessons-learned-from-a-frontend-interview-with-examples
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/mpN7xjKQ_Ns/upload/535270f8094faf64903955e5a2d72f0f.jpeg
tags: interview, frontend, frontend-development

---

A job posting pops up on one of my feeds:

**Frontend Web Developers Wanted: After a long time we are finally hiring again**

While not necessary looking for a new job, I still wanted the experience and a test of my knowledge.

Here is exactly how I was able to land that interview and the key takeways that I got from it.

## Applying for the interview

The job requirements were right up my alley:

* Detailed knowledge of semantic HTML & HTML accessibility
    
* Advanced CSS understanding (selectors, specificity, animations)
    
* Know how to work with JavaScript
    
* Bonus points for using TailwindCSS
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1702476655238/8350c8ea-2c3d-4df5-b896-8882c52f787c.webp align="center")

And my favorite thing about this job posting...

...there weren't any forms to fulfill!

Just an instruction to send your resume + past works to an e-mail address.

There was a note that if the applicant has no projects, they could do a task instead. The task was building a frontend interface for a shopping cart from a design provided in Figma.

![Checkout cart interface design from the take-home project](https://cdn.hashnode.com/res/hashnode/image/upload/v1702468473566/e9b0b91d-d878-40e3-a35d-9f894c0837ef.png align="center")

Even though I have several projects under my belt, I decided to do the task.

Call me crazy, but I like CSS. I quickly whipped it up and deployed it to the world wide web.

Once that was done, I spruced up my CV and sent them an e-mail containing a link to my Github profile. For a good measure I also linked the live version of the project as well as the code.

I figured that the task would be just a cherry on top of my existing work... which is where lesson #1 comes from:

## **Lesson 1: If there is a task to submit, that will be the focus of the interview**

Which makes perfect sense. It's the freshest project so it's the best way to gauge applicant's current skills. And it can be compared to other candidates who have submitted theirs.

While my project was basically a picture-perfect replica of the design, I didn't pay any special attention to the nuances of the code itself.

For example...

I exported all icons from Figma in PNG and imported them as such. Which is fine, right? But fine is not optimal.

Converting them to HTML SVG elements has better performance because you're not sending a few dozen requests to fetch the images.

![Figma project that was provided with the task](https://cdn.hashnode.com/res/hashnode/image/upload/v1702468700464/ddb4b6c9-1928-4649-a87c-18b72dd03eaf.png align="center")

Another example:

I used Tailwind to take care of a few hover states. But on others I did it with JavaScript.

When asked why...

I didn't know what to reply.

Probably because I completed the project in a few sittings. In between of those I must have changed my approach randomly. Bad idea.

I overlooked a few other similar things which they noticed and would ask me about. Focusing on replicating the design made me take some shortcuts that wouldn't be a good idea in a production environment.

### Example 1: Questions related to the submitted project

---

My interviewers made sure to ask me specific questions about the parts that weren't properly done:

* *What do I know about HTML headings?*
    
* *What HTML tag would I use for selecting the quantity of a product in a shopping cart?*
    
* *What is the &lt;img&gt; tag consisted of? What do we put in the "alt" attribute if the image is decorative?*
    

---

Lesson learned! Go through my future tasks with a fine-toothed comb before submitting them.

Speaking of production environment...

## **Lesson 2: Site performance is an important thing to companies**

Another thing that stood out in my frontend developer interview was the amount of questions related to performance.

We already mentioned the optimization strategy of turning images into SVG's. Other questions were in regards to website sizes.

For example:

*How much do I think that an average webshop sites with lots of images "weighs" (in megabytes)?*

My network tab is always opened when developing.

But it never occurred me to open it when I'm shopping around.

![Firefox's console network tab.](https://cdn.hashnode.com/res/hashnode/image/upload/v1702467270143/bceda46d-0e0e-4d34-88bd-74ccd1bed325.png align="center")

Since the company I was interviewing for is doing eCommerce projects exclusively, of course this is something that they will care about.

### Example 2: Questions related to website performance

---

Here are some performance-related questions asked during the frontend interview:

* *Is 20MB worth of initial network requests big for a website?*
    
* *How big (in MB) should a regular webshop site be?*
    
* *What is CLS?*
    

---

After the interview I checked some popular webshop to see if my answer was correct.

Here's the data:

| Website | Size in MB |
| --- | --- |
| Amazon | 4.32 |
| IKEA | 5.35 |
| Nike | 9.21 |
| Walmart | 4.56 |
| Costco | 10.72 |

And here's a pro tip for future frontend web development interviews:

Look at the company's portfolio and check out some of the sites. Don't just check how it looks, check the performance as well. That way you can bring it up in an interview if you get similar questions.

## **Lesson 3: Dust off the basics**

Here's a big stupid hole that I fell into.

I was unsure about some basic CSS things that I was using every day!

How come?

Well, as we start using additional tools and frameworks, they start handling some stuff for us.

For example, I frequently copy and paste Josh Comeau's [CSS reset](https://www.joshwcomeau.com/css/custom-css-reset/) which among other things changes the display property of images.

![The part of CSS reset which affects the display property of media elements such as img.](https://cdn.hashnode.com/res/hashnode/image/upload/v1702466729070/6d40b90d-c81d-4699-a0e0-94377f05e461.png align="center")

Which is super useful.

But it did make me forget that by default, &lt;img&gt; is an [inline-block element](https://www.w3schools.com/tags/tag_img.asp)!

### Example 3: Questions touching the basics of CSS

---

Some other basic questions that I stuttered through:

* *What color is #0000ff?*
    
* *What is the difference between em and rem?*
    

---

In my case, using Tailwind was the reason that I stopped caring about such things in my projects. It takes care of a bunch of little things like that by default.

But that's no reason not to know them off the top of my head for a frontend interview. Lesson learned!

## Lesson 4: It's still an interview for a company

Just because we are IT nerds talking to each other doesn't mean that regular interview stuff is out the window.

### Example 4: Regular interview questions

---

Expect to see some regular interview style questions such as:

* *Can you introduce yourself to us?*
    
* *Why do you want to work here?*
    
* *What are your top 3 strengths and weaknesses?*
    

---

Thankfully I have lots of experience interviewing outside of the IT field, so I didn't stumble through this. But I was a bit surprised at how classical some portions of the interview was.

[Talking about yourself](https://www.greatfrontend.com/behavioral-interview-guidebook/self-introduction) in the context of frontend web development is something I'll be rehearsing from now on.

## Lesson 5: Expect open ended situational questions

Now that we've remembered the theory behind this whole thing, it's time to put it to use. There were lots of questions that didn't have a yes/no answer (or true/false I should say).

Judging by how many I was asked, there are quite important to interviewers.

They make it easy to assess your knowledge and experience. So it's something to definitely pay attention to.

### Example 5: Open ended questions I was asked

---

Here are are some frontend interview questions I was asked:

* *Is the frontend developer responsive for the speed of a website?*
    
* *If a website is unavailable, what can be the reason?*
    
* *Have I used Tailwind? What do I like about it?*
    
* *How would I add graphics such as a two-tone logo to a website?*
    

---

I expected these, just not so many! So it's definitely something to consider for other web development interviews.

## Recap

I've noted my experience down because I hope it helps someone enter the frontend field. The market is currently stalling for a bit, so now is the best time to prepare for the upturn.

Now I'd like to hear from you:

Hopefully, you found my experience useful...

And if you did, please share it with someone else that might benefit from it.

If there is anything else that you're interested in, feel free to ask in the comments!

**P.S. Just to see how off I was - what was your answer to the average webshop size in MB?**