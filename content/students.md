+++

+++

<!-- <div class="alert alert-danger" role="alert" >
<center><img src="https://data.adrien-gruson.com/web/teaser_call.png" style="border: 3px solid;"/></center>
I am actively looking for a Ph.D. for a join project with Poitiers university on differentiable rendering and material modeling. <a href="https://data.adrien-gruson.com/web/sujet_en.pdf" class="alert-link">More information on the official call.</a>
</div> -->

This page contains guidelines and Q/A for anyone interested in being supervised/mentored by me or collaborating with me. 

## How to reach me

<div class="alert alert-danger" role="alert" >
It is important that you <strong>read this entire page first and clearly state it inside the email</strong> you will send to <a href="emailto:adrien.gruson@etsmtl.ca">me</a>. 
</div>

You must also provide information inside this first email to maximize your chance of getting my attention and avoiding unnecessary back-and-forth. Providing clear information is essential if you want to be supervised by me. To help you write this first email, here is a list of what type of information I would like to see:
* What are your research interests? Why do you want to perform research in computer graphics?   
* What background experiences do you have to support these interests? My suggestion is to summarize your prior and concrete experience in computer graphics (e.g., classes, coding projects, previous research experience,  etc...). Avoid being too general here. 
* How do you see your interest align with mine? What kind of collaboration are you seeking (Master, Ph.D., etc...)?
* Are you already in Canada? What is your current situation (working inside a company, finishing studying in a particular program, etc...)?
* What experience/skills are you seeking to develop by working with me?

I also suggest attaching your CV or/and putting a link to your website/GitHub inside this first email. All this information will help me to identify what you want and see if we can fit together. Usually, if we both decide to go forward with your application, we will arrange a meeting to clear out our mutual questions :) Note that I might request additional documents during our exchanges via email (e.g., academic record, recommendation letter, etc...). However, these documents are not required to be inside your first email. 

## Research Topics

My main expertise is in computer graphics and, more precisely, light transport simulation also called physically-based rendering. Rendering is the numerical process that takes as input a given scene description (surfaces, materials, light sources, camera position, ...) and simulates how the light gets propagated and scattered in a virtual environment to produce a physically-based rendered image. My research seeks to reach the ideal rendering system robust to any lighting complexity, highly performant, and easy to use for the artist (no parameters!). If you want to know more about my research, it is a good idea to look at my publication page on this website you are currently visiting :) 
 
Aside from doing research in forward rendering, I started to work on differentiable rendering and how machine learning can be integrated in light transport simulation. Both these new research axes have strong ties with my expertise (i.e., rendering). The goal is to explore and develop new exciting  applications which exploits computer generated images. Below are some of the research topics that I am actively exploring to help you see my research directions.

**Exploiting and controlling correlation in rendering**  is an efficient way to design robust estimators. For example, Markov-chains sampling generates correlated samples that explore the integration space locally. Another example is the gradient-domain rendering, which uses *shift-mapping operators* to produce positively correlated samples to estimate image space gradient. Using and controlling samples correlation in rendering has always been an important topic. I strongly believe this is a key and required property for designing more efficient and informed sampling techniques. 

**Designing robust sampling routines with data-driven approaches** is a recent topic in light transport simulation. Indeed, previous rendering techniques often rely on hard-coded decisions or complex user parameters, making it difficult to get optimal performance for a large variety of scenes. Therefore, moving toward more automatic approaches, potentially leveraging the scene information (via machine learning), is an important step to designing next-generation rendering algorithms.

**Improving the scalability of differentiable rendering** needs to be done as too much variance or computational cost in the estimated gradient might prevent the use of rapid iterative solvers. Moving to dedicated and efficient sampling strategies and potentially new (continuous) representation might be important for improving performance and scalability. This new performance gain will open to new applications, including interactive applications of differentiable rendering.

**Exploring new volume rendering integration techniques** by exploiting the additional continuous integration space over path segments. Indeed, compared to surface rendering, volume rendering needs to perform this extra integration, which is often costly and leads to high variance. Therefore, improving this integration process is essential to converge to a unified and general rendering technique for surfaces and volumes. 

## Common questions & answers

**What work environment can I expect working with you at ÉTS?**

I strongly believe that an inclusive and stimulating work environment is essential for performing good research. I also think that exchanging ideas with other people is crucial to bringing innovative ideas. For these reasons, my students will be placed inside the common multimedia students' lab space, which regroups students from different professors on various topics. 

I tend to work closely with my students (e.g., coding together, discussing papers, doing derivation on the whiteboard, etc...). So, you can expect to get regular integration with me.  You can also expect me to organize group events with other students to ease your integration inside ÉTS.

**Can I perform all my research activities remotely from home?**

One thing for sure: I will not micromanage you. I am normally flexible regarding the time spent inside the lab. However, I usually prefer that students regularly come to the lab to build a team spirit and encourage spontaneous discussions. 

**Does I need funding/scholarship to be supervised by you?**

I have a simple rule: students need to be paid for their work. So you can expect that if we decide to work together, you will receive some retribution for your work. However, as you might know, funding can be a limited resource in research. Therefore I will encourage and help you apply for scholarships before or during your studies (e.g., NSERC, Mitacs, ...). There is also an additional advantage to get your own scholarship, you can list them on your CV :) 

Note that some scholarships do not cover [your tuition fees](https://www.etsmtl.ca/en/studies/tuition-fees-ets). These fees can be important for international students. However, graduate students can get [reduced tuition fees in some conditions](https://www.etsmtl.ca/en/ets/bourses/exemptions-from-additional-tuition-fees).  

**Is it a problem if I don't speak French?**

This question might be worrying you, and it is totally fine! I had the same concern when doing my first post-doc in Japan :)

So, as you might know, French is the only official language in Quebec, and ÉTS is a french engineering school. This mean that most of ÉTS classes are taught in French. However, at [Master](https://www.etsmtl.ca/en/studies/Graduate-Programs/Master-Engineering-Information-Technology#Master's-Degree-with-Thesis-(research-profile)M.A.Sc.-) and [Ph.D.](https://www.etsmtl.ca/en/studies/PhD-Program/doctorate-engineering-ets) level, you can do all your studies in English at ÉTS, under my supervision. In this case, you will pick and follow courses at other Montreal universities (e.g., McGill).  

Concerning the outside aspect of your studies: as Montreal is an international city, it is not required to know French to live here. Moreover, I will assist you in filling in French documents or associate you with a French speaking peer. 

## Additional ressources

[Prof. Hachisuka's Graduate Study Survival Guide](https://cs.uwaterloo.ca/~thachisu/survival.pdf): Describe many aspects of doing graduate studies in detail, including motivations, possible outcomes, and challenges. Highly recommended read! (note that he was one of my past post-doctoral supervisors)