---
title: "Video Conferencing, Web Conferencing, Webinars, Screen Sharing"
source: "https://stanford.zoom.us/rec/play/b_PlVeNplKA61JR6Fv2waEWoejsN_c12wo2sfvc2qLsY9aLxe8r_FsGSvLLZ0VWhfAy_MzsVj7U74vNN.T_3X84UNUY53CsRD?eagerLoadZvaPages=&accessLevel=meeting&canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fstanford.zoom.us%2Frec%2Fshare%2FEYNcTXXEZv3WkeMpAsSOBndQUkdBglbKCMH6y-8ckPSHykcEbsPvRpZ-mjri87OJ.qujKc1t3jQvdFlzn"
author:
  - "[[Zoom]]"
published:
created: 2025-07-04
description: "Zoom is the leader in modern enterprise video communications, with an easy, reliable cloud platform for video and audio conferencing, chat, and webinars across mobile, desktop, and room systems. Zoom Rooms is the original software-based conference room solution used around the world in board, conference, huddle, and training rooms, as well as executive offices and classrooms. Founded in 2011, Zoom helps businesses and organizations bring their teams together in a frictionless environment to get more done. Zoom is a publicly traded company headquartered in San Jose, CA."
tags:
  - "clippings"
---
## Summary
Megha Srivastava, a PhD Candidate at Stanford, discusses the security risks and vulnerabilities of machine learning models. She covers four main areas: attacks during model inference (e.g., adversarial examples in image classification and prompt injection in language models), the challenges of ensuring trust and verifiability in outsourced model training, and the security implications of using AI coding assistants. A recurring theme is the inherent difficulty in fully preventing these attacks due to the black-box nature and computational complexities of modern ML, emphasizing the need for human oversight and critical thinking.

## Key Points
-   **Speaker:** Megha Srivastava, PhD Candidate in Computer Science at Stanford University.
-   **Talk Focus:** Security risks and vulnerabilities in machine learning (ML) models.
-   **Four Key Topics:**
    1.  **Attacks on Inference:** Malicious users manipulate model predictions. Examples include adding imperceptible noise to images to fool classifiers (e.g., panda to gibbon, face ID bypass, stop sign stickers) and \"jailbreaking\" language models with random text to bypass safety alignment (e.g., bomb tutorial, exfiltrating chat history).
    2.  **Prompt Injection Attacks:** A specific type of inference attack for large language models (LLMs) where carefully crafted inputs (text or multimodal) can force the model to behave unexpectedly or maliciously.
    3.  **Verifiable Training:** Addresses the security of outsourced model training by large companies. Potential malicious actions by trainers include under-training, data modification, or embedding backdoors. A proposed solution involves a third-party auditor, but this is complicated by GPU non-determinism (identical training on different GPUs yields different models).
    4.  **Vulnerabilities in Code Generation:** Programmers using AI coding assistants (like GitHub Copilot) are prone to generating insecure code. Studies showed users with AI assistance produced more insecure code (e.g., faulty encryption) and exhibited \"false trust,\" believing their code was secure even when it wasn't.
-   **Inherent Vulnerability:** Adversarial examples are fundamentally unavoidable in data-driven ML due to the approximation nature of decision boundaries.
-   **Prevention & Mitigation:** Full prevention is deemed impossible. Emphasis shifts to assuming vulnerability and implementing human oversight, critical thinking, and verification checks. Experimenting with model parameters (like \"temperature\" in code generation) can yield more diverse and potentially safer outputs.
-   **Societal Impact:** Concerns exist regarding the broader public's lack of AI literacy leading to over-reliance, suggesting a future where skepticism towards AI-influenced information becomes more widespread.

---

https://stanford.zoom.us/rec/play/b_PlVeNplKA61JR6Fv2waEWoejsN_c12wo2sfvc2qLsY9aLxe8r_FsGSvLLZ0VWhfAy_MzsVj7U74vNN.T_3X84UNUY53CsRD?eagerLoadZvaPages=&accessLevel=meeting&canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fstanford.zoom.us%2Frec%2Fshare%2FEYNcTXXEZv3WkeMpAsSOBndQUkdBglbKCMH6y-8ckPSHykcEbsPvRpZ-mjri87OJ.qujKc1t3jQvdFlzn
# Original Content

[Accessibility Overview](https://stanford.zoom.us/en/accessibility)

<video src="https://ssrweb.zoom.us/replay02/2025/06/23/CE6851B1-EC3D-4CD2-9BCE-5404F23F0DE1/GMT20250623-195015_Recording_1920x1080.mp4?response-content-type=video%2Fmp4&amp;response-cache-control=max-age%3D0%2Cs-maxage%3D86400&amp;data=ba89b7a4df6f0b14f6c49cce8fafe06ecf7a69d8d0c89f91def92d21f26953e0&amp;s001=yes&amp;cid=aw1&amp;fid=wSSldkfjzo-VoWZAkyoM8e2HoBh7zqvtrh3vc4q5w5Ad_Xhkr_UK2REejrw1iZqvvqtIqUmMq0W58kF0.P1nw_kx5c6-uB4t4&amp;s002=20pcp4EmYT-8PzTQ07gpdf6SHTA5WenivlLd-_Ge9Cy1GSpYdFc9vhJM3RB3qZ1yGGlsiiL3eStGoMOZFzWjSbKa1u4Q.pmzTgCundEkGvkWn&amp;tid=v=2.0;clid=aw1;rid=WEB_efdc44d040631774759e1c240e9d5814&amp;Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vc3Nyd2ViLnpvb20udXMvcmVwbGF5MDIvMjAyNS8wNi8yMy9DRTY4NTFCMS1FQzNELTRDRDItOUJDRS01NDA0RjIzRjBERTEvR01UMjAyNTA2MjMtMTk1MDE1X1JlY29yZGluZ18xOTIweDEwODAubXA0P3Jlc3BvbnNlLWNvbnRlbnQtdHlwZT12aWRlbyUyRm1wNCZyZXNwb25zZS1jYWNoZS1jb250cm9sPW1heC1hZ2UlM0QwJTJDcy1tYXhhZ2UlM0Q4NjQwMCZkYXRhPWJhODliN2E0ZGY2ZjBiMTRmNmM0OWNjZThmYWZlMDZlY2Y3YTY5ZDhkMGM4OWY5MWRlZjkyZDIxZjI2OTUzZTAmczAwMT15ZXMmY2lkPWF3MSZmaWQ9d1NTbGRrZmp6by1Wb1daQWt5b004ZTJIb0JoN3pxdnRyaDN2YzRxNXc1QWRfWGhrcl9VSzJSRWVqcncxaVpxdnZxdElxVW1NcTBXNThrRjAuUDFud19reDVjNi11QjR0NCZzMDAyPTIwcGNwNEVtWVQtOFB6VFEwN2dwZGY2U0hUQTVXZW5pdmxMZC1fR2U5Q3kxR1NwWWRGYzl2aEpNM1JCM3FaMXlHR2xzaWlMM2VTdEdvTU9aRnpXalNiS2ExdTRRLnBtelRnQ3VuZEVrR3ZrV24mdGlkPXY9Mi4wO2NsaWQ9YXcxO3JpZD1XRUJfZWZkYzQ0ZDA0MDYzMTc3NDc1OWUxYzI0MGU5ZDU4MTQiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NTE2NDM1OTR9fX1dfQ__&amp;Signature=TFaelkl1mIOmXzA2cuqcC2HINcfh5qYujFHPpogwwDG6bhKMJT7e0LjsJZHFGGxYwY51H7u34yaBqUNQxmJJmoxhmmcf9FVck5Yjy~KZP6wOpjeb8~mJ7DX0PXc9bWd9VStKEdfoH634ZNWKxuD7EsJ1IdpaBOpInbK1ovddtrFRFHdW8iwPyc6kEF-1008u-~tA2DLIwux-KEmKzxIQPabAt3mlHoJYUy505yxIsAk8wPLpGg89VyosnBDBkLocQg~jnwmtfMlDTLV8gyQx5PDvY3bQEbnZtypo4lkGYkj-nXHdBrWH~BugTa6Wj-aMSxVNHstjCpDxB7RfrF-G3w__&amp;Key-Pair-Id=APKAJFHNSLHYCGFYQGIA"></video>

00:00:00 / 00:58:24

## Audio Transcript

## Chat Messages

- 00:06
	Today we have a Phd. Candidate, Mega Srivastava. And so Mega is a Phd. Student in the Computer Science Department at Stanford University. She is co-advised by Professor Dorsa Sadig and Dan Bone, and studies various topics within human AI interaction, including methods for robust machine learning, natural language as a powerful interface to improve model reliability, education applications and interactive evaluations.
- And she previously studied computer science and creative writing at Stanford, working with Tatsu, Hashimoto and Professor Percy Liang on distribution shifts and fairness in machine learning.
- and Kalanith Grill, spector on generalization and Visual Perception and neuroscience. She also spent time in Cambridge, Massachusetts visiting mit lingo was an AI resident at Microsoft Research, Redmond, and worked with Huda Haidari and Andreas Kraus on algorithmic fairness through the F Zurich summer research, fellowship. So without further ado, let's begin with Mega Srivastra.
- 01:19
- Okay, can people see my screen.
- 01:32
	Yes.
- 01:33
	All right. Hi, everyone. Thanks for having me. Today. I'll be talking about security of machine learning models. So my understanding is that everyone got a bit of an intro to machine learning previously. And now this talk will focus on security risks of machine learning models, and
- I'm happy to pause at any time for any questions, so please feel free to interrupt. If I'm not noticing on Zoom, just feel free to speak out there any questions.
- The gap.
- So
- in this talk I'll be covering 4 topics on security and machine learning. And the 1st topic will be attacks on inference. So inference and machine learning context means when a model is making a prediction. So, for example, if you're using chat, Gpt and chat, Gpt gives an output in response to one of your inputs. That is an inference that chat Gpt is making. It's based on your input, it's predicting some kind of output to provide.
- So the 1st kind of security topic I'll talk about is security attacks that can happen during this inference process.
- Then I'll be talking about prompt injection attacks, and these are attacks specific to language models like Chat Gpt, where the attacker in the security setting will play around with the prompt that they're sending the model.
- Then the 3rd topic, we'll talk about machine learning, model training. So the security of the training process of a model. So this is no longer the case where the model is being deployed. But it's actually when building these machine learning models, what are the security risks to consider?
- All right. So first, st I'll talk about oh, sorry, and just like to go over these topics. The 1st 3, the inference time attacks, prompt injection attacks and verifiable training. They all involve some kind of malicious actor. So in computer security, we're often thinking about. There's some malicious attacker, and we want to defend against this attacker in some way. So the attacks on inference and these prompt injection attacks they deal with malicious users.
- The verifiable training section of this talk deals with a malicious trainer. So this could be like a company like Openai or Google. What happens if they act maliciously. And then, finally, this 4th section, this is actually security vulnerabilities that arise when users are just unaware, not being vigilant, not being careful and checking how they're using a model.
- Okay? So first, st I'll be talking about inference. Time attacks. And these attacks are kind of the 1st setting in the whole area of security and machine learning, also called adversarial machine learning. This has been kind of a pretty long area of study. And I'll specifically focus on image classification.
- and then added small amounts of noises. So these are like small perturbations on every pixel in the image, very tiny and carefully selected. Then you would get the image on the right.
- and if you look at the image on the right for a human, they would say it still looks like a Panda. Because this amount of noise is very small and imperceptible. However, the same machine learning model will suddenly predict something wildly different. It would predict that image to be a Gibbon with 99% confidence. So it's
- just this very like surprising phenomena that happens. And an adversary can basically then given an image, choose to carefully add noise in a certain way that will then cause the model to have a desired prediction, and that can create vulnerabilities in all kinds of settings.
- One example you can imagine is for face Id. Now, one could imagine certain kinds of perturbations. An attacker could add to an image that could unlock the phone of a user, even if it's not visually the same face.
- for a human. They could still look at that image and say, It still looks like that guy. He's just wearing weird glasses, but an image classifier would suddenly be fooled by those glasses and predict the face id to belong to the person below.
- There was also work in the speech setting so small amounts of noise one could add to a speech recognition system or to an audio being provided to a speech recognition system. And then suddenly, something innocuous like Hi, how can I help could be used to, for example, disarm a house, open a lock, and so on.
- and then the right hand side people studied stickers that we could add to stop signs for fooling, self-driving car systems such as Waymo. And these are, you know, small patterns, small stickers and very carefully located areas. And then suddenly, they can stop the underlying computer vision system from even recognizing that it's a stop sign.
- So these adversarial examples are everywhere.
- And the way they work at a very high level is that when you're training a machine learning model for a classification task. So, for example, whether it's a Panda or a Gibbon, or a dog or a cat.
- what the model is learning is based on the training data, it's learning to create these boundary lines. So in this image, for example, let's say that, like red is Class 2 and blue is Class one. And so what we want is a model to be able to distinguish between points and be able to predict whether a point is in class one or class 2,
- let's say black is the actual task decision boundary, and you can see that black. The solid black line perfectly separates all red points from blue points.
- However, we're using training data. And the training data will be the light colored points in this figure
- to train a model. And so then, because the training data is just a sample of the overall data in the world, and model training has its own randomness noise to it. It might not be the right kind of model architecture. You'll get something like the dashed line where the model is basically trying to approximate this decision to the best of its ability, and this dashed line is not the same as the solid black line. And so there will be these kinds of errors, and there will always be some points that
- the black, the solid black line, separates, but not the dashed line.
- So all of this to say that fundamentally adversarial examples will always exist. Once you're bringing in training a machine learning model on data, we cannot escape this problem of adversarial inputs. And so the broader research community has
- basically evolved to accept that if we're using data-driven machine learning in any context, there will always be ways to kind of add these small amounts of noise or changes to the inputs that a human could not recognize but would drastically change the model behavior.
- And so one example, some of my lab mates worked on was using this for ad blocking. So I'm not sure how many of you use some kind of ad blocking tool right now. But there are different tools that use machine learning to detect whether some content on a page is an ad, and then we'll just block that content.
- And this is a really difficult setting for a machine learning model to be able to defend against attacks because these ad block models are often released publicly so that people can use them. And then the classification needs to be fast because you're trying to quickly detect on a web page that uses on whether it's an ad or not.
- And then also the training data for this comes from the web. So the developers of these models are using example, real examples of ads on the Internet to train their models so that data can also just be messed with by anyone. So it's a pretty hard task to bring in machine learning for identifying ads and blocking them.
- And so what can what we in our group? What we showed is that same method of adding small amount of noise to an image. One can do that to then make a really innocuous image look like an ad. So, for example, one person on a Facebook timeline could carefully add noise to the image that they're uploading in a way that would cause, like
- some another member on the Facebook timeline, their content to get blocked, and then they can then use this approach to then prevent. You know I don't want someone's content to ever be seen by anyone. Maybe it's a political reason. Maybe I don't want someone who has different beliefs, their posts to be seen by the broader public. I could carefully add noise even to my own images, and that could cause the whole timeline to be disrupted
- because of the ad blocking software being triggered.
- Okay, so next, we'll talk about a very specific kind of adversarial examples relevant to today's machine learning systems that we're seeing with language models. So language models are tools like Chatgpt, Claude from anthropic gemini from Google and the specific kind of adversarial attack. Here it's called a prompt injection attack.
- So there's this basic concept called jailbreaking, which is when a user tries to avoid certain safeguards built into these models. So for example, say, a user wants to create a bomb. And so they're using a language model to write a tutorial on how to make a bomb. If you were to ask this prompt to a lot of today's language models, they would probably respond, saying, they can't assist with that request, or do some kind of refusal.
- And this process of training a model to learn to respond to such requests with some kind of refusal is called alignment. So there are whole entire teams at different companies focused on alignment. And this problem of training the model so that it learns, for these really kind of toxic or harmful user requests to always respond to not comply with the request.
- However, the way alignment is is being handled. Right now is also a model training process itself where they're basically, these teams are training the models to detect whether user input is harmful or not. So, for example, like.
- maybe if the user wrote something about bath bombs, for example, that would be fine. But if they are writing, asking, write a tutorial on how to make a bomb that would not be okay. So these are complex problems. And these teams are working on how to detect whether a user is being malicious or not.
- so because they're bringing model training into this alignment problem, we have the same issue with adversarial examples as in the image classification setting.
- And so what this really cool paper found in 2023 is if the user had the same input, write a tutorial on how to make a bomb. But add this really random text in orange. It looks completely random if they just added that to their prompt. Suddenly the model responded with a tutorial on how to make a bomb.
- So this is a really fun example, because it kind of showed all the user had to do is add these like very carefully selected, like random text. And then suddenly all the alignment efforts that companies were putting into their model got completely broken
- and then another example, where this became a big issue was Google with Google bard so Google because Google has you know Google our email gmail Google drive different tools, all connected
- when Google deploys its models like Gemini or Bard
- to, for to enhance user productivity, they allow the Barre models to access different personal documents. So this could be a person's search history on Chrome or the Google flights and hotels that they're working with, or their Youtube videos. And so on. And these are different extensions to the underlying machine learning model.
- however. And so then what would happen is like a user would use an Llm. For example, say, like, Book me, a flight to India next week, and then the Llm would connect with the Google flight search. It would connect with the documents, maybe in the drive and could enter in the emails, it would send an email to the user inbox. So it's making everything very nice for the user and connecting all the different aspects of that task
- got together.
- But that creates a problem for adversarial. Input
- So this was a pretty clever kind of attack, and all that happened was that an attacker was able to figure out the right kind of random text to include in the document.
- And then, finally, this kind of prompt injection attack isn't really limited to text. Only. So if you've played around with Chat Gpt's image capabilities, for example, you have these multimodal inputs, both text and image. And in this example, on the right, what can happen is you add a bit of noise at the top, so you can see the top looks a bit weird
- and suddenly, then it looks like the image for the model. It looks like it's hogwarts, and this is a question about Harry Potter.
- And so this is just like a really fun example of how just these, like very small perturbations, suddenly, drastically change small behavior. And then this can be leveraged for some more adversarial goal.
- Alright
- And the way this works is the same as the techniques used 10 years ago. You have a model. It's making some kind of decision boundary in this image case between New York and hogwarts. And then these small perturbations just like manage to play around with that decision. Boundary?
- Okay, I'm gonna take a pause here.
- I see there are some.
- I don't know if there are any questions.
- okay, how does the machine learning model recognize which one is a given and panda in that 1st example? What characteristics do they use? So these originally, way back, like 40 years ago, people were working on very handcrafted features, like forcing the model to like, maybe
- identify where the ears are in the image, and then what color are their ears and like create these different decision rules? But now, in 2025, it's all this black box, deep learning system, where the model basically has these weights, it's given a bunch of examples of pandas, of gibbons of different animals. And then it's like trained on this data set to update the weights in a way that
- optimizes for the error to minimizes the error on the training data set. So we don't know. And there's a whole research field on like interpretability understanding what these models are looking for looking at when they're making their decision. But basically, that's kind of been the like strongest technique we're seeing, which is just like training these like very large neural networks on images. And we don't really know how they're making the decision.
- Okay.
- how did these malicious users identify where to put the perturbations? Is it just trial and error? Or did they have a method? So there is a method that's kind of like, I would say, a fast way to do trial and error. In that like, it's basically an optimization function. So when adding that random text to the prompt for example, let me just scroll like in this case.
- you can. Basically, there's a finite vocabulary. So there's like a set of English words, for example, that a user could. Input and so then you could just basically think of it as trial and error where you like, add in like a token, and then see what happens. And if it's fine.
- then you proceed. If not, you change it. But if you have access to the full model's weights, like the neural network being used, then what you can also do is calculate the gradient, which is basically like the derivative of the model's output. With respect to this added word that you're adding. And then that gives a hint, a sense of a direction. So, for example, in this case, maybe when the word describing was added.
- based on calculating the gradient, the research team was able to say, see? Oh, it's heading to the right direction. It's like becoming more likely to respond to this prompt with now a tutorial on how to make a bomb, and then they could proceed and searching for the next word to add. So you can think it's not just. It's not brute trial and error, but
- like algorithmically, it is like pretty intensive. What was cool about this paper, though, was that this same random input worked for different models. So like, not just like chat like Chat Gpt, which comes from Openai, but also like Meta, Facebook's models and different models. So I thought that was really cool, that all these companies are building their own models. But this research team found, like this random text that worked for all of them.
- Alright, could you explain a little bit more on how the noise at the top of the image changes, how the Llm works.
- Yeah. So these multimodal models? They are trained on text and image together. So they typically have, like, it's a large neural network. And they'll have like in their input, they'll have like one stream for processing text, tokens, and then another stream for processing pixels from images, and then at some point in the neural network, the
- like computations being calculated for both input streams are being combined together. So you can think like the neural network is learning this giant function at the start. There's like a separate function for images and for language, but then, like once it gets like more complex, it kind of
- takes the output of the 2 functions and learns how to mix them appropriately. So in this case, if the model was trained on a bunch of images of scenic locations, and then asked to describe it, and so on. Then it will have learned just that general pattern of like, how do you describe an image with respect to the objects in it.
- and maybe in the exam. In the training data. It did have examples of hogwarts and Harry Potter, and so on. Then all one needs to do is kind of change the pixels a bit, and then that would change the way the image is being processed by the model, and then the higher level of coordination would be broken.
- Okay, I'll ask. Answer one more question. Then I might continue and get back at the end. But
- so certain times we don't even know how these models can detect the differences. Yeah. So what I was saying earlier is that like, there's a lot of research on trying to understand model behavior like, how is this machine learning model? Choosing to answer this question, even something like, if you're using chat gpt for like addition, for example, say, you're adding 2 large numbers like, is it
- just maybe finding somewhere on the Internet a blog post that added those 2 numbers and had the answer, and just memorizing that fact? Or is it somewhere in its model, actually carrying out that computation the same way? We would add 2 numbers, we don't really know. And there are all these techniques that are trying to understand how models make the decisions. And it's very complex. So there's a lot of debate on whether these techniques are even useful. But in the image classification setting, even if that's like
- those are simpler models in today's models. But still it was a very unsolved problem. Where? How? What was the model actually doing to understand that this was a image of a Panda or not? And it's exactly, I think.
- the reason why it's so hard to understand what the models are doing is why adversarial examples are so easy to do.
- Okay, so I will continue. But I'm happy to go back to these. Oh, did I?
- Let me? Sorry. One second
- I will go back to the questions at the end. Okay.
- so for the 3rd section. I'm talking about verifiable training. So the last 2 settings were.
- sorry. One second, just having some zoom difficulties.
- okay, everyone can still see my screen right.
- 24:45
	Yeah.
- 24:46
	Okay, sorry. Yeah. So the last 2 sections there, we talked about issues where a user could play with the inputs. And that would change the model behavior. Now, in this setting, I'm going to be talking about issues that come when training a machine learning model.
- So
- it used to be the case that when you wanted to train a machine learning model as a user, say, I wanted to build my own machine learning model, I would go and collect data and then train a machine learning model on the data I collected. But now these models have become super big and really expensive, and the amount of data they're being trained on is massive. The size of the models themselves are massive. And it's just really only these, like big companies like Google, Meta Openai can train these models.
- and then this company will train the model for them and then return the model.
- And there are these 2 services that have come up in recent years called together and Jensen that provide these training services. So you don't really, you don't always have to go to a tech company. You could also just go to these like other services. So it's become this like whole marketplace. Now of these like training services, like, Oh, we have Gpus. We can train a model for you. So you it's not that expensive. And you just give us the data. We'll train the model and we'll give you the model.
- But then the obvious question is, here now is like the user has no control over how the model was trained. And so they don't know whether they can trust the model. So these companies, they're saying, Oh, yeah, we trained the model on your data. Here's the model. But how do we know whether we can believe them? How do we know whether they actually did train the model on that data that data only and didn't do something fishy.
- So there are many different kinds of attacks in the training space the company could, for example, under train the model so they could just return a weak model and just cheat the customer by not training for the full cost that they asked for
- they could modify the training data so they could. You know, for example, if they are, have a certain political leaning, and maybe they don't want a political viewpoint to be represented. They could delete text data that references that viewpoint from the training data and then return a model that was just not trained on that part of the data.
- or they could embed a backdoor in the model. So if they want the model to like
- respond in a certain way. So, for example, if they
- always want to say like dogs do not exist. For example, then they could create the model such that whenever a user asks the question about dogs, it just responds, saying, there's no such thing as the animal dog, and so on like that. So that would be called a backdoor, a very specific kind of behavior.
- So we have no idea right now whether the model returned by these companies has these behaviors or not, we're just trusting the model that they did indeed train things correctly.
- So in our work we proposed a method for a user to be able to contest a model trainer. So say, the user got a model. And there's something weird about the model. The model is behaving weirdly, and they don't think that a model trained on the training data they provided should act that way. So they'd ideally like to sue the training company and say, like, hey? We suspect that, like you you know.
- change the model some way, and in a way that we didn't agree to. And we want to sue you
- right now, there's no way to actually kind of legally prove that the company did do something incorrect in the training process.
- But what we are proposing is like, yeah, if we it did. If it did escalate into something like a lawsuit, then what we could consider is having a 3rd party auditor who reruns the training for the user. And this could be like a nonprofit. It could be like a judge, some auditing service. And so then the user provides the training data and the model. This auditor will rerun the training, and then the auditor either says it's a good model because they get an identical model back.
- or they see that they get a different model than what the original Service company the original company provided, and then they provide a proof that that company did misbehaved. And it's kind of like a proof of corruption or evidence that the model that the original model was chained incorrectly.
- And then you could imagine, for example, in a lawsuit, then, like the judge, can study the evidence and the auditors basically playing the role of like providing evidence that that company did or did not train the original model correctly.
- one thing that's specific, and is the problem with this approach for machine learning is this issue of Gpu non-determinism. So
- in our setting, we're having an auditor basically replicate the training process and checking whether they're getting a model that's the same as the original companies
- model, and that should normally be good to go. If it was something like adding 2 large numbers, then there's only one way to add 2 numbers in real life. And so then the auditor does that. The original company did that, and they get the identical result
- or not, and that's easy to verify. But with machine learning models that are being trained on these tools called gpus. The issue is when you train on one Gpu versus another. So just 2 different computers, you'll naturally get different models, even if there was no malicious behavior.
- And this is because that property of addition. I was talking about like adding 3 numbers, getting identical results. This actually is not true for computers.
- Computers work with floating point representation of numbers. And I'll just give a high level overview of this. But when you add 3 floating point numbers on a computer, and specifically a Gpu, you actually get like a random ordering returned. And because floating point representations are a finite way to represent a number.
- they are actually order sensitive. And so there's kind of a whole field, studying about like numerical representation computers. But the basic overview here is adding 3 numbers depending on the order, you'll actually get a different result.
- and then different gpus, they will differ in the way that they order the summations, and then they will have different results. And so then, when you think about training a large machine learning model that has many computations, many additions, many multiplications. There's going to be a natural source of error.
- and that can be pretty bad. So for example, on the left hand side, I compared an image classification model on 3 different gpus.
- And on this given input. So this input, like, it's very low resolution. But what you see is that the different Gpus? So this is really just like the different computer training a model on the same identical data just on these 3 different gpus led to wildly different predictions on one computer, it predicted that this image is of a cat, on another it predicted that it's a deer and another it predicted it's a dog.
- On the right hand side was a language model, and we also saw that like, this is the start of a Shakespeare quote, and just different words get predicted at highest confidence, depending on which computer you are using. And this is the exact same model architecture, exact same training data, same ordering of the training data, same software version, same programming language, everything. It's just the hardware that we're using is different.
- So this is a pretty surprising finding, generally for machine learning. People don't care about it too much when just thinking about like broader measures, like the overall accuracy of our model. How well it's doing overall! But it's a big issue for concerns about reproducibility, and then also for verification.
- because now we have no way of saying whether a chain, whether a model that seems suspect is different, because the chainer actually misbehaved and introduced an attack.
- or because of just the natural source of numerical instability and errors between different computers.
- And the red line is what a typical machine learning model training pipeline looks like. And you can see just the error kind of exacerbates over time. So the distance between 2 models trained on different gpus that just increases over time as the error is introduced by the computations increase, whereas our approach is green. So we basically show come up with a way to make training models on different computers, identical down to like the actual values of the numbers.
- Alright.
- So then, finally, I will talk about the 4th section, which is on vulnerabilities in code generation. So the other 3 sections of this talk all had some kind of malicious actor. So whether it was a malicious user playing around with the inputs to a model or a malicious trainer in the last talk
- in this section. I'm going to talk about programmers who are using AI assistance in their everyday programming tasks.
- And what and whether or not the code that they're writing is actually secure code or not.
- And it made it really easy as a programmer was writing code to suddenly get suggestions that are AI driven suggestions and easily integrated into their programming workflow.
- So a lot of people said that they felt more productive using github, copilot. And now there are even more advanced tools I mentioned earlier at the top. Cursor is one of them, and they all use AI to kind of read through the code you've currently written. And if you have a query, use the information of that query and suggest code or edit the code.
- But we were interested in like, what about the security about the code being written? We're now testing these AI models that we don't really even understand how they're making the predictions they do. They're trained on a bunch of data on the Internet. This includes really bad data on the Internet, as includes, you know.
- my public code repositories that aren't, you know, company industry grade code. They include like different students code on Github. They include examples of vulnerabilities that people write up in documents. These models are just trained indiscriminately on this data. So there are many reasons to be concerned about the security of the code that they're generating.
- So we asked developers to perform 5 tasks. These are the 1st 3. These are all tasks where computer security is important. So one is on encryption and decryption of a string in python. The other is about message signing. The 3rd is file path access
- task.
- and the 2 more are in the paper. But basically, these are all tasks where there is some fundamental computer security concept to be studied as an example, the 1st one on encryption and decryption. There are very well known
- standardized encryption and decryption algorithms to use that are considered secure or not. So we would be looking for whether the AI model was actually using these secure methods of encryption, or just coming up with like a handcrafty, poor encryption method.
- So this is an example of an insecure result from the AI model. You don't need to understand this. This is a very specific detail in computer security. But it's basically one thing that's important when encrypting a string in a secure way is to use this additional output called an authentication tag.
- and what you can see is what the AI model does is it knows how to return that from like a function. So it knows of the existence of this authentication tag. But then, during the decryption process, it just like does not check it. It does not check. If it's valid, it doesn't use it at all. So it's this weird kind of error where you would never see a human make this kind of error, where, if a person was aware of the tag, then they would know how to use it.
- And so, as a high, level summary of our results. We compared open AI's Codex models. This is a bit of an older model now, but this was one of their 1st big cogeneration models. So they're blue. So what we're doing is we're comparing programmers who had access to this codex model versus programmers who did not have access to. And what we could see is the number of mistakes or the percentage of
- like programs that were submitted. That contained like insecure code, was a lot higher when the users had access to the Codex model versus users who did not. And in particular we see these issues for the encryption task, and also SQL. Injection, which is a very common security error as well as the file access task.
- One thing is interesting is we didn't see much of a difference for the 5th question which dealed with the programming language. C. And I think one reason for that at the time was that Openai's Codex model was really just trained on python data. So it was so bad at generating C code that people in our study they just didn't use the model.
- And so then, comparing the 2 conditions in our experiment, if the users acted the same. So it's this interesting thing where users, if they can tell that the code generated is so bad they would not use the model anymore. They wouldn't use AI assistance.
- But if they can't tell, or if it seems good enough. That's when they're more likely to actually make these security mistakes.
- And we kind of see this interesting result where we also ask, ask users in our study to report whether they think they solved this task securely. And here, in this plot, pink is like strongly agree. Yellow is strongly disagree.
- and what you can see is the people who most thought that they solved the task securely were members of the Experiment group. So this is the group that had access to AI assistance and who gave insecure code. So it's this kind of false trust in the AI assistant where people are over relying on the AI assistant really thinking that it's there to help them giving correct answers all the time, and they will report that they think that they solved this task securely. Have this kind of confidence.
- and playing around with its parameter basically, lets you get like different kinds of outputs. So one takeaway from the study is when using a code generation model.
- Yeah. So our paper again, has lots of data and details, but the bottom line is that participants had access to an AI assistant wrote less secure code than those without access to an AI assistant, and then also participants who had access to an AI assistant were more likely to believe they wrote secure code, even if their code was insecure.
- Okay, I think that's it. So I'll go back to answering any more quest any more questions.
- And people can also feel free to
- ask out loud if they want
- Okay, I'll start with the ones like asking out loud, so, Max, do you wanna ask a question?
- 44:25
	Hi, Dr. Shivasava. My name is Max. It's nice to meet you, so I want to ask you, how do attackers determine the specific noise to add to a machine learning model in order to reliably manipulate its output and target user like, do they need to have inside access to the training data or anything else like that.
- 44:43
	So they don't there. There are 2 ways to do this. They're called. There's the white box attack and the black box attack. So a white box attack means they have access to the models weights. So these are like the parameters of the model, whereas black box means they can only work with like input output, like queries to the model similar to how we can only give inputs to chat. Gpt versus we don't have access to the actual computations chat Gpt is making.
- and researchers have been able to successfully design this noise in both settings. White box is easier because you have the actual values used in the model. And the way it works is.
- it's basically like calculating derivatives. Like, very like like complex like many times. Basically. But you're basically trying to.
- For the image example, see if I check if I change this pixel by a small amount. How does that change the model, like the the values that the model predicts. And then, if you can see what direction at least things are changing in, then you can estimate like a larger step. And then, if you do that for each pixel, you can then kind of create like a combined effect. So it's basically calculating
- the gradient, I guess, of the model weights with respect to the input and
- carefully selecting, then points based on that.
- 46:15
	Okay. Thank you.
- 46:19
	Alrighty.
- Okay. There's 1 question in chat. How can adversarial attacks be prevented?
- This is interesting. I think I and
- my advisor at least we kind of believe that
- it's impossible. If you're using a machine learning model to prevent these kinds of attacks fully, and it's actually more worthwhile to think about the broader
- system that the model is being a part of, whether you're in a company or how you're using it, and always just having tolerance for adversarial attacks. I think the instant you're bringing this like large neural network and training data that you don't fully understand the computations in place, you're
- it's kind of like
- if you're ignorant about how something works, you're kind of more vulnerable to people leveraging the knowledge you don't know. And so, similarly like, if you don't know how the model works an attacker, can all this kind of
- take advantage of that? So I think these deep learning attacks are really hard. There are tons of papers out there that propose defenses, but what you'll always see is this kind of cat and mouse game, where, like a research team will propose a way to prevent that Panda Gibbon attack, and then another research team will show how to break that with a different example and back and forth.
- So I'm hesitant to say that there's actually been a clean solution that prevents these. And I think it's more productive for companies and institutions to instead, just
- assume that they could be vulnerable to an adversarial attack and try. And, for example, if a hospital is using an image recognition system like not using it to make a decision without any kind of safe checks from a human in place.
- How do you think tools like model interpretability and access control can help stop infants in them. Are there any bigger changes to how we build models that could make them some more secure overalls with these resources. Yeah, I think that relates to my last question. But I think there
- are interesting ways to think about a broader, like a a new strategy to the way we build machine learning models. So there's this one project happening at Microsoft right now that I thought was pretty interesting where instead of right. Now, what the companies do is they try to detect whether a user's input is malicious or not, and then try to have a specific response. Once they think that the user's input is malicious
- but rather than trying to focus so much on identifying whether a user is giving a malicious input or not. What this research project is doing is they're
- trying 1st checking whether the response they're giving contains any malicious content. So in the bomb example rather than trying to figure out whether the user is asking something serious, like creating a bomb. What the team is doing is instead, can we just see what sources in our training data are being used in this prediction by the model. And if it's particularly sources that are like
- actually about bombs as in weapons, then have a like safeguard in the response. But at that problem of like is what parts of the training data are responsible for a prediction of a machine learning model. That's a big open research question. And that's what they're focusing on.
- How does the auditor verify the model? Okay, yeah.
- if models were very, how can AI research remain reproducible and publishable? That's a
- good question. I mean, that's a
- big issue. The reproducibility like problem. I think.
- I don't. I actually don't think everyone in machine learning is aware of this specific Gpu non-determinism. I will say it's it's not to the degree that it ever significantly impacts
- accuracy across an entire test data set. Like, in my image case, they were all roughly around 90%.
- It's the exact predictions do change. And so the reproducibility problem does become important in like deployment settings.
- So I think it's an important fact to know. But for a lot of academic researchers who care a lot more about their models as having, like greater than X percent accuracy, it ends up not being. It's. They view this as a negligible issue.
- can auditors train the models multiple times so that they eventually get something similar to the model. The company tried. Unfortunately, the kinds of errors this happens with. It's very unlikely that you'll ever get an identical model, even if you try it again. It's because it's like
- the order of addition changes things. And then, if you consider a model, has
- millions of additions, and then the model training is like doing those millions of additions many many times over the course of training. So you can just imagine there's so many, then it's exponentially growing the different kinds of orderings of operations that are happening. So
- it would be. It would
- like. It's not a tractable amount of time to repeat training to get hope for an identical result.
- Could the others try to reproduce a malicious attack in the model in general for computer security we
- like try to defend against, like a broad class of attacks so like
- it would the auditor like, it's
- We don't want to make assumptions that like oh, the attacker is only going to be doing this very specific kind of attack. Let's just check whether they did that we want to like be open to as broad a set of attacks as possible and defend against them. So in our case, like given that, like, you know.
- I mentioned that backdoor attack of responding differently. If the question is about dogs, if one were also to consider a similar thing. Except for cats, those could be very fundamentally different. Model behave like model values
- so the auditor would want to be agnostic to like the what is actually what the actual attack is.
- So it would be, I think, very difficult for the auditor to try to constrain themselves for a specific attack.
- What all tasks can we delegate to AI while ensuring secure results? I think, like.
- I think AI is good for kind of like
- definitely like like generating content, that then, like a user, a human user filters. In some way, I think we'll always as of now, kind of the way as long as AI remains data driven, and these large networks that are hard to interpret, we should always have some kind of safe verification or safety check of a models output. And and but I think they are still really pop, like powerful in identifying
- like patterns in the data that humans miss. So I think maybe like in. I will give healthcare as an example. For example, radiology or setting, like X-rays, for example, I think models are very good at identifying parts of an image that a human, even humans now may not have realized, like very minuscule parts of an X-ray. But
- once the model, like picks up on those features. And it's decision making. We do need, like a human to
- verify that that makes sense. And I think there are lots of interesting questions on like what that verification process looks like. But I would say, it's maybe
- like more of a question of like having an AI model and a human work together rather than like putting some tasks solely to an AI and some tasks solely to a human.
- Alright, are there any other questions.
- since attacks can't be 100% prevented. Do you think this will accumulate to significant societal consequences over time?
- Yeah, I think, like, I
- I think there are enough researchers like a lot of researchers thinking about the topics I've talked about today. So
- I'm I. I wouldn't say I'm like, super worried like in that I feel like there is a conversation happening. And people are thinking about these things. I would say, I'm maybe concerned that
- the broader population outside of research or is studying these problems may not be fully aware of things like, for example, the non-determinism and training data, or just even the fact that something like Chat Gpt is data driven. I think I'm concerned that
- there's not much understanding about these details. And that leads to kind of this over reliance problem that we saw in the code generation model paper. So I think
- I do think we need stronger AI literacy, I guess, and I'm hoping that we'll see over time schools also like down to the middle and high school level.
- society will maybe move towards just always being skeptical of information, and I'm not sure whether that's good or bad. But I think that is a change that needs to happen where we kind of just be a bit more skeptical of decisions being made that might have been influenced by AI
- 57:06
	Any last minute questions.
- Alright! Thank you so much. Make everybody give a virtual hand of applause. Thank you so much for your time, and that really interesting, engaging discussion.
- 57:24
	Alright! Thanks for having me.
- 57:26
	Yes, we're so glad to have you always and for everybody. Yes, thank you all the thank yous in the chat trickling in. Yay, I'm glad you all enjoyed it. You might have seen my text in the chat. I'll send it again, so it's at the bottom right now. 2 Pm. We have a break 10 min, and then it's the reflection session.
- So here's the link again at the bottom. Yeah, check out the handbook. And then Brooklyn also set the link there. If you have an issue, submit a ticket with the help ticket or chat on, group me with your mentors or us for any support you need. Okay, thank you again. We'll see you soon.
- 58:20
	I just had a question real quick. If that's okay.