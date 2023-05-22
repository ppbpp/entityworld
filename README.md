# entityworld
documenting ideas around digitally modeling knowledge as a graph based system, with an eye towards note taking and beyond

## Core abstractions: entities and connections
Entities are sort like a platonic ideal. Except of course ideals don't exist; there is no chairness of a chair, there's only a pile of wood, and monkeys that decided to come up with a name for the same butt supporting pile of wood.  Without disappearing down an epistemological rabbit hole, we can generally agree human knowledge is recursively defined. 

So let's define clear the slate, and pretend we are in a vacuum. We have infinite curiosity and absolutely nothing yet in existence.

The most basic abstraction we need is `entity` -- a sort of blank container for any idea or "thing". Entities themselves can be unique. We will leave it this generic, and build out other ideas recursively on top of it. From a POV of comp sci, an entity is a node in our graph.

I also want to have a `connection` as the other basic primitive, this one describing some sort of link between the nodes of the graph. A graph is really boring with only nodes and nothing connecting them (and this is a really boring argument against loneliness).

So far so good. But still not very useful. Let's make something. I want to add a little character to the void and model my husky John Waters. We can define him as a unique entity `John Waters`, and we all understand it to be this specific husky John, with no other entity like him anywhere else. Same with his friend, sausage dog friend `Bruce Willis`, let's add him too. 

At this point we are not yet discussing *how* we are storing the knowledge, how we entered it, whether it's text or a picture or recordings of their barks. We haven't even yet defined what a dog is. Our world knows nothing of fur, or other entities with possibly shared but unrelated names. We just have an empty void with 4 things: entities, connections, Jono and Bruce.  


### Case study: note taking
This is my original motivator. In an attempt to fix note taking for my forgetful ADHD brain, i've run into limitations of every piece of software for the same reasons: even when adding hyperlinking and tagging, notes become a mess of trying to remember where each piece of information is stored. I struggled through academia massively: even though I could build a web of context in my mind, it became near impossible if it had to be built out of a mix of physical media, the web, PDFs and other random shit I struggled to organize and keep mapped.

When we share a note or a piece of text with embedded media, what we truly mean to do is share knowledge about a "thing". The thing might be a recipe, itself a collection of ingredients that are both agreed upon by humans, and standardized actions that can be taken on them. There are billions of recipes out there but everyone on earth understands exactly the same idea of a "recipe". 

The issue with note taking software isn't that it's modeling the wrong sort of note taking behaviour; it's that "note taking" is a paper-bound concept forever limited by the idea of a "thing" holding "text". 

Instead, we should question why we take notes, and solve that original problem, which is: we are trying to capture information about a thing. That can be text in multiple languages, sound, video, whatever. Instead of modeling a series of blobs of text, we can instead model an "entity", and attach meaning to it via whichever means appropriate, which may not even be written word or text altogether. This is why it always feels so clunky to have an audio recording app while trying to take text notes, for instance. The whole thing turns into managing various sources of media by gluing it via text bound "notes".

This is why text-based Notes and Evernote and even the "open canvas" Freeform and OneNote are inherently broken: they're modelling whiteboarding, not knowledge capture. They are what HTML5 tried to fix: pure presentation concern. So long as we use text based notes, we are forever stuck in a world of using `<i>` tags instead of `<strong>`. Anyone who's tried to have a running text note while inserting images of graphs, audio of a lecture and photos of the whiteboard, will understand. And when you add all this media, it becomes forever hidden inside whatever app embedded it, never to be seen by the operating system. 

The benefits of using entities here are gigantic: "note taking" itself dispenses with text entirely if wanted. E.g. how I document an entity on a bird with text and pictures will probably look different from someone who doesn't use their vision, and instead prefers to document. The necessity of a screen reader as as an input or output layer falls away.

For example, instead of a series of text notes on my cat Sofi, I have "Sofi" the entity, a uniquely identifiable "thing" that is itself no matter the context. I can describe who she is; save videos of her; write down her dietary preferences and link the note up to her veterinarian entity via a "vet" relationship. Now, no matter where I am, I can get at information about "Sofi", whether that's via a search for vets or cats, or I can easily share everything I know about her in an already structured way.

Note taking is a just a view into "knowledge structuring" which sadly currently ends at "text entry".
