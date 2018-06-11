# The Four Layers to Great Documentation

When I started to publish some open source projects, I did a deep dive into how to document them. This is the most useful method I’ve found.

Good documentation requires four layers, each building on the previous layer.

### Getting Started
### Guides
### Concepts
### API
The best way to write these is to start from the bottom (API) at work your way up to the top (Getting Started). Incidentally, readers of your documentation will start from the top, and only occasionally find their way to the bottom. Even then, starting writing from the bottom up helps to better inform the top layers.

## API
This is the only section of your code that can be auto-generated.
Documentation is written exclusively for humans, and that usually means a
human needs to write it. You can auto-generate your API docs from your source
code, if you have commented it.

This should be comprehensive documentation of how to use the API of the project, typically generated from the source code.

You should be documenting your code, so that when you come back to it in 12 months you can understand it again. Be selfish, and kind to your future self, let them know what you did and why. You will not remember. (This side benefit here, is everyone else can understand too).

## Concepts
What are the fundamental building blocks for this project? Try to break the project up into pieces, and write a detailed explanation of each one.

The goal here is to explain the building blocks of your project. Expect anyone who will implement your project to read through this section. You want this to be detailed and thorough. You don’t need an essay on each, a few hundred words and a diagram might be enough.

If you need to write a long page for a concept, be kind to the reader, and try to create sections for easy reference. While some will read it from top to bottom, it’s more likely it will be skimmed for the most relevant part for the reader at that time. Some headings and a table of contents is all you need.

## Guides
A guide or tutorial, is the ideal way to explain how to use your project to solve a specific use case.

They should be written with the end use in mind, considering their use case and knowledge. It’s better to over explain, than not. Something may be simple and obvious to you, but unheard of to your user.

Think about why you started the project in the first place, and make a list of the use cases you wanted to solve. It may help to write a small user story for each, something like: “As a project maintainer, I would like to know how to write good documentation, so that I can get more users of my project”. The typical format to produce a user story is: “As a [role], I can [feature] so that [reason]”.

In that last paragraph, I did two things. First, I said making a list of user stories will help with working out what guides to write, but then I gave an example of a user story, and the template to write them. You could have searched to find out what a user story is, but by explaining it right there I’ve not only saved you a bit of time — I’ve removed the ambiguity of what we’re talking about. A user story may mean something slightly different to you.

But back to guides. You want to have at least 3 to 5 to explain how to use your project. It could be how to use it on each particular operating system, or how to integrate with the 3 most popular frameworks.

Or, how to integrate with a focus on a particular concept from the previous section.

Most likely you’ll have 1-3 guides when you publish your project. As issues and frequently asked questions appear, turn these into guides.

## Getting Started
This is the single most important section you will write, and does not consist of a single ‘Getting Started’ page.

If you’re project is a small library, you may be able to get away with just a Getting Started section. Typically in this scenario, you would only have one main concept, and a set of examples functioning as the Guide section.

First, work out what your landing pages are. You may have a website, a GitHub readme. You might also have a page on npm, godoc, pypi, or another package manager. Normally all of these except the website will be direct copies of your readme, so lets start with that.

### Readme.md
To start you need to answer the following questions clearly, and concisely:

What is this project called? What does this project do?

Then, explain how to get it. Maybe it’s a download via a package manager, or a link to a releases page containing binaries.

Now, show a simple use case. Here you’re showing the public interface of the project. For many projects the best Getting Started, is literally showing the implementation code. Don’t show everything, just enough to run it once.

We’re now in the footer of the readme. It’s nice to add information on how to develop on this project, so information on how to setup a development environment, and examples of how to run the tests should be here.

It’s strongly recommended to include information about how to contribute to the project, where to raise issues, the process for new features and pull requests.

You should include information about SemVer if you’re using it. (If you’re not using SemVer, please consider it — your users will thank you).

Many projects like to acknowledge their major authors and contributors in the footer area too.

And finally, at the very bottom include a license. This is typically a note of the license type, with a link to a LICENSE.md file. You must include a license, without one people will be wary to use your project.

## Badges
You don’t need them. Although they can be useful to your users. Use your own discretion here, don’t go overboard. They can provide a bit of social proof.

## Website
If you also have a website (you don’t always need one), your “Getting Started” consists of the front page, and a dedicated getting started page. If you want to include them both on the once page, just ensure theres a link that can take a reader directly to the “Getting Started” section.

The front page usually covers the same information as the Readme, and is often wrapped in a nice design. Don’t go overboard here, you’re focus is on readability above all else. Sometimes a cool graphic or animation can get a project shared around — but don’t focus on that at the expense of your actual users.

Documentation is the best marketing tool for your project, and the best indicator of the trustworthiness and maturity. It takes effort to document a project well, but if you want users it’s worth it.

As an example of this approach to documentation you can look at a project I recently published Bunjil.

