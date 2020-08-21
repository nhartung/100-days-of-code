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

### Day 8 August 9th, 2020

**Today's Progress**: Got a lot of good functionality added to the CollectableLight. Movement works, attraction works, collection works. Could probably use some cleaning up, but the base functionality is there. 

**Thoughts:** I could really use a particle that emits light to the scene. I could start looking into creating a custom shader with that behavior.

### Day 9 August 10th, 2020

**Today's Progress**: Played with shaders.

**Thoughts:** AFter some playing around, I realized that I don't think a shader will solve my problem. I'm trying to create a new light source, not modify fragments based on lights. I'll need to go with a non-particle solution if I want to move forward with this approach. For now I can ignore this feature. Light emitting particles are required, but would be cool.

### Day 10 August 11th, 2020

**Today's Progress**: Played around with IES files to generate lights. I think I have a good idea on how I'm going to generate different lighting effects moving forward.

**Thoughts:** I didn't actually do much coding, or learn anything towards Godot today. Hopefully I can get back on track towards that tomorrow. I got a bit distracted trying to get some cool new light effects to work. Although, what I've done today should go a long way towards some cool lighting effects for a finished game.

### Day 11 August 12th, 2020

**Today's Progress**: Continued to play around with IES files and learned more about shaders. I figured that the use of IES exports might not quite work for my needs. No worries, it's not far off and I'm smart, I can generate the images I need using the IES files as a starting point. I created a shader that dampens the resulting IES light exports to make them look more realistic in a 2D environment. Now that I have that working I can hopefully generate some different lights and put together a cool little demo with them.

**Thoughts:** Shaders are cool.

### Day 12 August 13th, 2020

**Today's Progress**: Playing around with lights and other assets that interact with them.

**Thoughts:** Playing around with shaders yesterday paid off as I needed it today for some of the sprite work I was doing.

### Day 13 August 14th, 2020

**Today's Progress**: Put together a "showcase" of what I've been working on. Still minimal, but looks kind of cool. Still working towards a concept, but I have some ideas.

**Thoughts:** You can definitely create some cool aesthetics with lights, even in 2d.

### Day 14 August 15th, 2020

**Today's Progress**: Got a camera and collisions working.

**Thoughts:** Both were easy, but I needed to convert my Area2D objects into KinematicBody2Ds in order to have everything work properly. I could use some refactoring to pull out some common code.

### Day 15 August 16th, 2020

**Today's Progress**: Got some better sprites for the blocks I've been using. Started creating some moveable block clusters. I need to figure out a strategy for having the block anumations participate in the collision detection logic. Ideally while still using a Tween for movement.

**Thoughts:** I think it's starting to look like it could actually be a game. I have some pretty cool concepts thought up as well. We'll see what the future holds.

### Day 16 August 17th, 2020

**Today's Progress**: Fixed my collision issue. As it turns out, I need to call move_and_slide, even for cycles in which the movement vector is zero. Otherwise the physics engine will not operate.

**Thoughts:** TileMaps greatly simplify a scene. I should also look into "AnimationPlayer" in leiu of using a set of Tweens for my environment movements.

### Day 17 August 18th, 2020

**Today's Progress**: Mostly a refactoring day. Switched the SquareTransform from using Tweens to instead using an AnimationPlayer. Better for many reasons. Also made the BigBlock textures a parameter that can be specified. Leveraging this in the SquareTransform allows me to make use of any textures I want for the object, meaning that I'll have common logic for any set of textures I want to apply this to.

**Thoughts:** Godot is still surprising me with some of its capabilities that make life easier.

### Day 18 August 19th, 2020

**Today's Progress**: Started to create a concept for a light "generator". Honestly spend far too long trying to figure out a shader to generate the lighting effect I wanted. Got it rendered by the end of the day, so at least I'm not stuck. I'll continue the concept tomorrow.

**Thoughts:** Shaders are powerful, but can be difficult.

### Day 19 August 20th, 2020

**Today's Progress**: I refactored code related to move_and_slide. Apparently you aren't supposed to use the delta parameter when using this function. However, you are when you call move_and_collide. I assume there's a good reason, but it's odd. Anyway, continued work on the "Generator" concept that I'm working on. Got some cool animations working now. As usual, it was very easy to set up.

**Thoughts:** Working with sprite sheets is super easy.
