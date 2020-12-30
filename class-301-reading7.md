# What Google learned from it's quest to build the perfect team

- Working together in teams or collaborating with colleagues has show an improvement in efficiency and work performance. 

> n Silicon Valley, software engineers are encouraged to work together, in part because studies show that groups tend to innovate faster, see mistakes more quickly and find better solutions to problems. Studies also show that people working in teams tend to achieve better results and report higher job satisfaction. In a 2015 study, executives said that profitability increases when workers are persuaded to collaborate more. Within companies and conglomerates, as well as in government agencies and schools, teams are now the fundamental unit of organization. If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.(Duhigg, 2016)

* The most productive employees 
- Rotate dining companions
- Avoid micro managing 

> The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright. (Duhigg, 2016)

### Successful teams

- Every member spoke about the same amount, every member needs to have a voice and feel comfortable to give their opinion
- had high "average social sensitivities" Each member was able to pick up on the feelings of others via their non-verbal cues

> But Google’s data indicated that psychological safety, more than anything else, was critical to making a team work. (Duhigg, 2016)

> Rozovsky and her colleagues had figured out which norms were most critical. Now they had to find a way to make (communication and empathy) — the building blocks of forging real connections — into an algorithm they could easily scale. (Duhigg, 2016).

- Everyone within the team needs a chance to speak and contribute.  It is important that everyone within a group feels free to speak up and to be heard.  Also, psychological safety and emotional conversations are related and they need to accepted.  The closer one feels to a team the better they can express their ideas without worry of rejection or non acceptance.  True freedom and thought of expression allows for growth


# How I explained REST to my brother


> The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.
- A web page is a “representation” of a resource
>  Oh, right. Those URLs tell the browser that there's a concept somewhere. A browser can then go ask for a specific representation of the concept. Specifically, the browser asks for the web page representation of the concept.

>Yes - and more. We need to be able to talk to all machines about all the stuff that's on all the other machines. So we need some way of having one machine tell another machine about a resource that might be on yet another machine.
- it's called a "redirect"

> Machines don't have a universal noun - that's why they suck. Every programming language, database, or other kind of system has a different way of talking about nouns. That's why the URL is so important. It let's all of these systems tell each other about each other's nouns.

- that's another big aspect of REST. Well, verbs are anyway.

- Verbs are important. There's a powerful concept in programming and CS theory called “polymorphism”. That's a geeky way of saying that different nouns can have the same verb applied to them.

> Well, that's important. What if instead of me being able to say to you, "get the bottle," and "get the magazine," and "get the book"; what if instead we needed to come up with different verbs for each of the nouns? I couldn't use the word "get" universally, but instead had to think up a new word for each verb/noun combination. "shmet the bottle", "mandle the magazine", "zorp the book"

- But some verbs are almost universal like GET, PUT, and DELETE.

> So anyway, HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you type in and back comes a web page.

* But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.

- HTTP isn't just for getting, yet HTTP is actually a general purpose protocol for applying verbs to nouns

- Each of the systems would retrieve information from each other using a simple HTTP GET. If one system needs to add something to another system, it would use an HTTP POST. If a system wants to replace something in another system, it uses an HTTP PUT, or, to do a partial update, it'll hopefully use PATCH. The only thing left to figure out is what the data models should look like.

- Now, we just tell Rails what we want our data to look like, and it takes care of all of the communication pieces for us. It's a huge boost for productivity!

* RESTful web frameworks 
- Ruby on Rails.





Reference :  https://gist.github.com/brookr/5977550

### Reference - https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html. Charles Duhigg, Feb. 25, 2016.
