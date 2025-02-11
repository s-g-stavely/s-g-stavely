# Creating software for manufacturing lines

I've spent a little time writing software that runs in a manufacturing line, for calibrating and testing the hardware being produced. Here's some design goals of this software that I feel are important.

## Think about the users

Your software is being used as a means to an end, by a person under pressure to keep the line productive. They are not necessarily skilled with computers. They will be using your software to perform many of the same actions over and over. Design with them in mind, so that you make their life easier, not harder.

Create a UI that can be easily understood and interacted with. Use big text and buttons. Use bright green to indicate success and red for failure. Don't worry whether it looks good.

## Be ready for errors

Be clear about the causes of errors, using language that the user will be able to understand. Try to give enough information that they can troubleshoot the problem. If possible, permit the user to retry failures, so that they don't need to start the entire process over again. Keep log files around to help with debugging.

Since your software is interfacing with the physical world, all sorts of weird things can happen. It pays to watch someone actually using it, and see what's difficult for them.

## Decide whether to be strict or forgiving

It's hard to write good instructions for how to use your software. What's more, in practice people will often choose not to follow them. They might do this because they've figured out a better way of doing the work, or because they need to use the software for something you didn't plan for. They also might simply be under pressure to get work done quickly, and willing to subvert the intended process to do so.

So, you should consider how much flexibility you want to build into the process. Can steps be skipped? Can config values be edited by hand? Making it more flexible means it can handle more real-world problems, but risks it being misused.