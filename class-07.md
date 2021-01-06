
# It's the end of the Scope as we Know it

With so many things happening in program we write, so many names to remember and paths to follow, scope and scope management become very important; without it we're at a carnival or a music festival with no map, no program, the stands and stages have been strewn about wherever the event planners could stash them, the attendees are camping in and among and around all of the sights and smells and sounds. It is Chaos incarnate and nobody is having any fun. Imagine trying to find a specific stand, your friends campsite, or the stage the DJ you wanna hear is rumored to be at but you really don't know because there's no program saying if they're even playing the event. Such an event would have no continuity, and more time would be spent trying to find the things and people you enjoy, than actually enjoying them. This is code without scope and scope management. 

### This name is mine, there are many like it...
The most obvious way scope impacts a program, is with Names. Where you assign a name in your code also assigns it to a scope, like a specific stage at the festival, that name belongs to that stageing area and if you look for that name in a different stage, you will be sorely dissapointed when it is not at all the person or thing you were looking for even though the NameTag says it is. so how do we keep it all straight in our heads? The simplest way to maintain general order of course is not to name things the same, and if we absolutely must do so, make special notes about which one belongs to which stage!

### The Pylibrarian, the NameSpace catalogue, and their scope.decimal system
Time to make all of our analogies complete by going back to library. Python follows a specific procedure when looking for names, each section or scope, has its own card cataloge, the NameSpace! the NameSpace is a dictionary of all names available to that scope, just like sections at the library, fiction, autobiography, self.help, etc. the interpretry (representign our Pylibrarian in the heading) will look for a name following a set procedure nown as LEGB, an acronym for: Local, Enclosing, Global, Built-in.

- `Local Scope: Names only exist inside the function you are currently in, even if it is the same as a name in a different cataloge(scope)`
- `Enclosing Scope: Names exist in the function around and above a nested function but not in the function or in the global scale`
- `Global Scope: sometimes called Module scope, these names can be acessed from anywhere in the code and referenced using the decimal system (dot.notation)`
- `Built-ins: these are similar to the Global scope catalogue but require no additional naming or assigning, they come with the Standard Library. like free bookmarks at a real library`










#### [Return to Main index of Notes](./README.md)