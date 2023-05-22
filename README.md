# entityworld
documenting ideas around digitally modeling knowledge as a graph based system, with an eye towards note taking and beyond

## Core abstractions: entities and connections
Entities are sort like a platonic ideal. Except of course ideals don't exist; there is no chairness of a chair, there's only a pile of wood, and monkeys that decided to come up with a name for the same butt supporting pile of wood.  Without disappearing down an epistemological rabbit hole, we can generally agree human knowledge is recursively defined. 

So let's define the most basic abstraction of an _entity_ -- a sort of blank container for any idea. We will leave it this generic, and build out other ideeas recursively. From a POV of comp sci, an entity is a node in a graph.

I also want to have a _connection_ as the other basic primitive, this one describing some sort of link between the nodes of the graph.

So far so good. But a little boring. Why don't we define a _human concept_ entity as an entity that has a unique to it meaning, like a human "type system" of sorts. This allows us to say, model my husky John Waters. We can define him as a unique entity _John_, and we all understand it to be this specific John. Same with his friend, sausage dog friend Bruce Willis. 

At this point we are not yet discussing *how* we are storing the knowledge, how we entered it, whether it's text or a picture or the sound of their barks; Instead, let's wait to define this later. 


### Use case: note taking
In an attempt to fix note taking for a forgetful ADHD brain, i've run into limitations of every piece of software for the same reasons. even when adding hyperlinking and tagging, notes become a mess. 

The issue with note taking software isn't that it's not modeling the right sort of note taking behaviour; it's that "note taking" is a paper-bound concept forever limited by the idea of a "thing" holding "text". 

Instead, we should question why we take notes, and solve the original problem.  The actual problem is: we need to capture information _about_ a thing. That can be text, or richer media. Instead of modeling a series of blobs of text, we can instead model an "entity", and attach meaning to it via whichever means appropriate, which may not even be written word or text altogether. 

The benefits are gigantic: note taking itself dispenses with text entirely if wanted. E.g. how I document an entity on a bird with text and pictures will probably look different from someone who doesn't use their vision, and instead prefers to document. The necessity of a screen reader as as an input or output layer falls away.

For example, instead of a series of text notes on my cat Sofi, I have "Sofi" the entity, a uniquely identifiable "thing" that is itself no matter the context. I can describe who she is; save videos of her; write down her dietary preferences and link the note up to her veterinarian entity via a "vet" relationship. Now, no matter where I am, I can get at information about "Sofi", whether that's via a search for vets or cats, or I can easily share everything I know about her in an already structured way.

Note taking is a just a view into "knowledge structuring" which sadly currently ends at "text entry".
