# 100 Days Of Code - Log

### Day 0: August 1st, 2020

**Today's Progress**: Created a [blog site](https://nhartung.github.io/) using Jeykll. I'll my blog to provide occasional larger updates.

**Thoughts:** Although it's not related to my 100DaysOfCode, I found building a site with Jeykll to be extremely intuitive and simple. This will be my path in the future for basic blogs and web pages.

### Day 1: August 2nd, 2020

**Today's Progress**: Learned more about using Light2D and LightOccluder2D. Started to play around with a playable character and movement.

**Thoughts:** The built in Light2D and LightOccluder2D functionality is extremely easy to use. With the plan that I have now, my game will incorporate lighting heavily. Knowing that there is an easy to use framework in place for lighting gives me hope that some of the concepts I hope to implement will not be very difficult. Starting messing around with player movement. I'm not sure yet if I want to use the built in KinematicBody2D movement or roll my own in an Area2D. I'll likely go with the latter, as it's what my prior experience is, and I don't think I need the capabilities of KinematicBody2D for what I hope to create.

### Day 2: August 3rd, 2020

**Today's Progress**: Implemented vector based movement for Area2Ds as well as started messing around with the particle system.

**Thoughts:** The particle system is pretty fully features. However, it doesn't seem to have the lighting capabilities that I may require. I'll likely need to look into rolling my own particles or creating some sort of customer shader for the existing particle system.

### Day 3: August 4th, 2020

**Today's Progress**: Starting to look into creating my own particles, but it turned into a refactoring day. Learned how to use plugins to create custom nodes and how to call in "library" functions.

**Thoughts:** The refactoring I did today was very useful. I envision myself creating many reusable Nodes as I continue development. There's something nice about being able to pull in our own custom nodes into the scene, rather than calling library functions inside individual scripts. They each have their use and I'll need to be careful to use them appropriately.

### Day 4: August 5th, 2020

**Today's Progress**: Continued creating custom light particles. I have something basic working, but it needs a lot of customization in order to work appropriately. However, I think I've discovered where I want to put my focus for my first feature. The player collected light particles.

**Thoughts:** I'm dealing with some pretty annoying editor bugs (I think). I need to find some time to submit an issue to Github. I've posted to discord, but no responses yet.


### Day 5: August 6th, 2020

**Today's Progress**: Honestly, spent too much time messing around with the editor bug I talked about yesterday. I discoverd an open issue against it: https://github.com/godotengine/godot/issues/36592, although I'm not sure if it's a bug or "feature". I've implemented a workaround for now and am moving forward. Still working on the light particles.

**Thoughts:** Editor bugs are annoying.

### Day 6 August 7th, 2020

**Today's Progress**: Played around with Visual Scripting.

**Thoughts:** It's an interesting feature, but not one that I'll use personally. I mainly investigated it because I'm considering its use for a model-based design tool that I'm proposing at work.

### Day 7 August 8th, 2020

**Today's Progress**: Back on track, continued working on the CollectableLight. Got the movement to a place where I'm happy with in. Attraction is next.

**Thoughts:** Nothing much.
