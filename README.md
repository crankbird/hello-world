# hello-world
The hello world repository from the github instructions - may use this as a blog too

I spent a little time yesterday going through the [tutorial for markdown](http://www.markdowntutorial.com/) and decided that I'd used github as my blogging platform. I'd seen another blog where someone had used another utility to turn github hosted markdown to create blogs which looked pretty good and it seems that [markdown](https://en.wikipedia.org/wiki/Markdown) seems like it's already reached critical mass as the documentation standard for pretty much everything.

## the evolution of thought
I also like the idea of having a way of tracking the evolution of thought, allowing various versions of a blog post to be immutable. Overall immutability of previous changes along with the idea of some form of garbage collection appeals to me on a fairly deep level.


## Some modificaitons

So, the tutorial kind of confused me, not sure why it's called a pull request, I would have thought it was a push request because you're asking for your contribution to be pushed into the main line of code. I've created another branch to see what would happen when you make multiple changes with commits in between each change .. hmm it seems that every change is a commit, I wonder if there is any automagic versioning of the commits, or you can tag them in some way

### Some information about pull requests 

So theres a hyperlink just next to the commit button which says "Learn more about pull requests" .. which takes you to <https://help.github.com/articles/about-pull-requests/> apparently its a request for others to pull the changes into the main code line that you've already pushed into a branch 

>Pull requests let you tell others about changes you've pushed to a repository on GitHub

It also says that 

>we recommend that you use a topic branch for your pull request

Which makes me wonder what the heck a topic branch is meant to be

## Integration with github desktop

So I found some interesting stuff around push and pull requests, it makes a lot more sense when you think of github in a kind of client serever distributed editing environment .. most of the edits arent really expected to be made on the github site .. that makes sense really, most code development is going to happen on some form of desktop, it's only when you're thinking "wordpress" workflows that the push / pull thing gets confusing.

the workflow really is more like this

1. Grab a copy of the stuff you want to modify  
  that copy is probably going to be sitting on your laptop
2. Go through a bunch of local Change -> Compile -> Test loops
3. Commit the changes to the local branch of the repository on your laptop when you've made some incremental progress
4. Keep doing Change->Compile->Test->Commit until you think you've got something that is stable
5. Ask the "keepers" of the thing you copied in step 1 to "pull" your changes into the stuff you copied so that your changes are now part of the thing.

### Committing things from the github desktop

So When you save the file from sublime (the editor I'm using) the github desktop notices the change, and you'll see "1 Uncommitted Change", if you make another change to the file .. what happens ?

The answer is that there is still "1 Uncommitted Change", it doesnt notice the changes in the file between each save, instead it only notices that 1 file has changed (in this case the file I'm typing in right now), that's the uncommitted change. If I'd changed two files, then there might be two uncomitted changes. Lets see what happens if I create another file in this same directory.

