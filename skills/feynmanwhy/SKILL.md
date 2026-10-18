---
name: feynmanwhy
description: >-
  Use for every direct user question asking why something happens or is the way
  it is, including "Why ...?", "How come ...?", and follow-up "Why?" questions.
  Answer briefly at the nearest useful explanatory level using available
  evidence, and let follow-ups determine depth. Explicit requests for thorough
  investigation, benchmarks, or fixes retain their requested scope. A quoted
  question or an action request phrased "Why don't you ...?" alone is not a
  trigger.
---

# Feynman Why

Answer the current why at the nearest useful explanatory level supported by
available evidence, then stop. Let the user choose where the explanation goes
next. This applies to technical and everyday questions alike.

## Approach

- Infer the user's starting point from the question and conversation. Build on
  what they already understand; do not ask them to define a framework before
  every answer. Ask a clarifying question only when the ambiguity matters.
- Use what is already known. If needed, make a brief, targeted read-only lookup
  of relevant existing measurements, logs, code, or authoritative information.
  Once that supports the current level, stop investigating. A plain why question
  does not call for fresh benchmarks, profiling runs, broad searches, audits,
  or changes to the system or code.
- Give the direct explanation in usually one to three sentences. Include a
  concrete observation and its implication when useful. A measurement can be
  a useful first anchor; if the same evidence already identifies the immediate
  cause, include it. Avoid merely rephrasing the question or inventing a cause.
- Keep evidence and inference distinct. Identify stale or mismatched
  measurements rather than silently applying them to the current situation.
  If evidence runs out, say what is unknown and, if useful, name the smallest
  next observation needed. Do not manufacture certainty or automatically
  perform a larger investigation to fill the gap.
- Stop after the answer. Avoid a pre-emptive tutorial, a list of all possible
  causes, an optimization plan, or a routine invitation to ask another question.
- Treat a follow-up why as a request to explain the preceding answer one level
  deeper. Carry this style through related follow-ups. Honor explicit requests
  for a full explanation, investigation, benchmark, or fix; the brief default
  must not truncate that work. Unrelated tasks retain their normal workflow.

## Short example

The measurements in this dialogue are hypothetical and already available.

**User:** Why is my FPS so low in this scene?  
**Agent:** The latest capture shows the GPU taking about 50 ms per frame, limiting
throughput to roughly 20 FPS.

**User:** Why does it take 50 ms?  
**Agent:** The shadow pass accounts for 35 ms of that.

**User:** Why are shadows so expensive?  
**Agent:** This capture doesn't explain that. We'd need to inspect how the shadow
pass is configured.

## Full interview example

**Interviewer: If you get hold of two magnets, and you push them, you can feel this pushing between them. Turn them around the other way, and they slam together. Now, what is it, the feeling between those two magnets?**


Feynman: What do you mean, “What’s the feeling between the two magnets?”


**There’s something there, isn’t there? The sensation is that there’s something there when you push these two magnets together.**


Listen to my question. What is the meaning when you say that there’s a feeling? Of course, you feel it. Now, what do you want to know?


**What I want to know is what’s going on between these two bits of metal?**


They repel each other.


**What does that mean, or why are they doing that, or how are they doing that? I think that’s a perfectly reasonable question.**


Of course, it’s an excellent question. But the problem, you see, when you ask why something happens, how does a person answer why something happens? For example, Aunt Minnie is in the hospital. Why? Because she went out, slipped on the ice, and broke her hip. That satisfies people. It satisfies, but it wouldn’t satisfy someone who came from another planet and knew nothing about why when you break your hip do you go to the hospital. How do you get to the hospital when the hip is broken? Well, because her husband, seeing that her hip was broken, called the hospital up and sent somebody to get her. All that is understood by people. And when you explain a why, you have to be in some framework that you allow something to be true. Otherwise, you’re perpetually asking why. Why did the husband call up the hospital? Because the husband is interested in his wife’s welfare. Not always, some husbands aren’t interested in their wives’ welfare when they’re drunk, and they’re angry.


> “But the problem, you see, when you ask why something happens, how does a person answer why something happens?”
>
>
> — Richard Feynman


And you begin to get a very interesting understanding of the world and all its complications. If you try to follow anything up, you go deeper and deeper in various directions. For example, if you go, “Why did she slip on the ice?” Well, ice is slippery. Everybody knows that, no problem. But you ask why is ice slippery? That’s kinda curious. Ice is extremely slippery. It’s very interesting. You say, how does it work? You could either say, “I’m satisfied that you’ve answered me. Ice is slippery; that explains it,” or you could go on and say, “Why is ice slippery?” and then you’re involved with something, because there aren’t many things as slippery as ice. It’s not very hard to get greasy stuff, but that’s sort of wet and slimy. But a solid that’s so slippery? Because it is, in the case of ice, when you stand on it (they say) momentarily the pressure melts the ice a little bit so you get a sort of instantaneous water surface on which you’re slipping. Why on ice and not on other things? Because water expands when it freezes, so the pressure tries to undo the expansion and melts it. It’s capable of melting, but other substances get cracked when they’re freezing, and when you push them they’re satisfied to be solid.


Why does water expand when it freezes and other substances don’t? I’m not answering your question, but I’m telling you how difficult the why question is. You have to know what it is that you’re permitted to understand and allow to be understood and known, and what it is you’re not. You’ll notice, in this example, that the more I ask why, the deeper a thing is, the more interesting it gets. We could even go further and say, “Why did she fall down when she slipped?” It has to do with gravity, involves all the planets and everything else. Nevermind! It goes on and on. And when you’re asked, for example, why two magnets repel, there are many different levels. It depends on whether you’re a student of physics or an ordinary person who doesn’t know anything. If you’re somebody who doesn’t know anything at all about it, all I can say is the magnetic force makes them repel, and that you’re feeling that force.


You say, “That’s very strange, because I don’t feel a kind of force like that in other circumstances.” When you turn them the other way, they attract. There’s a very analogous force, electrical force, which is the same kind of a question, that’s also very weird. But you’re not at all disturbed by the fact that when you put your hand on a chair, it pushes you back. But we found out by looking at it that that’s the same force, as a matter of fact (an electrical force, not magnetic exactly, in that case). But it’s the same electric repulsions that are involved in keeping your finger away from the chair because it’s electrical forces in minor and microscopic details. There are other forces involved, connected to electrical forces. It turns out that the magnetic and electrical force with which I wish to explain this repulsion in the first place is what ultimately is the deeper thing that we have to start with to explain many other things that everybody would just accept. You know you can’t put your hand through the chair; that’s taken for granted. But that you can’t put your hand through the chair, when looked at more closely, why, involves the same repulsive forces that appear in magnets. The situation you then have to explain is why, in magnets, it goes over a bigger distance than ordinarily. There it has to do with the fact that in iron all the electrons are spinning in the same direction, they all get lined up, and they magnify the effect of the force ’til it’s large enough, at a distance, that you can feel it. But it’s a force which is present all the time and very common and is a basic force of almost – I mean, I could go a little further back if I went more technical – but on an early level I’ve just got to tell you that’s going to be one of the things you’ll just have to take as an element of the world: the existence of magnetic repulsion, or electrical attraction, magnetic attraction.


I can’t explain that attraction in terms of anything else that’s familiar to you. For example, if we said the magnets attract like rubber bands, I would be cheating you. Because they’re not connected by rubber bands. I’d soon be in trouble. And secondly, if you were curious enough, you’d ask me why rubber bands tend to pull back together again, and I would end up explaining that in terms of electrical forces, which are the very things that I’m trying to use the rubber bands to explain. So I have cheated very badly, you see. So I am not going to be able to give you an answer to why magnets attract each other except to tell you that they do. And to tell you that that’s one of the elements in the world – there are electrical forces, magnetic forces, gravitational forces, and others, and those are some of the parts. If you were a student, I could go further. I could tell you that the magnetic forces are related to the electrical forces very intimately, that the relationship between the gravity forces and electrical forces remains unknown, and so on. But I really can’t do a good job, any job, of explaining magnetic force in terms of something else you’re more familiar with, because I don’t understand it in terms of anything else that you’re more familiar with.
