# Project Setup

## The Dark Days

When I first set up my site, I uploaded all of my files to an FTP server. Any update would require making the change locally, testing it, opening up Filezilla for the first time in ages, updating Filezilla to a newer release, then ten minutes later finally uploading my file update. No source control, lots of pain. Not a lot of fun and a big concern for keeping my personal history somewhat up-to-date.

## The Better Days

At some point I realized that since everything is served as a static file, [GitHub Pages](https://pages.github.com/) would be a fantastic way of serving the content. No more FTP uploaded. Integrated source control and easy updates from any computer. Just jump on my repo, edit the file from the GitHub editor, and voila, updated site. There were a few hoops I had to jump through to get this working.

### Hoop #1 - Setting up a username.github.io repo

Since I wanted my repo to be the root of my Github profile, I needed to set up a User Page. Github automatically does this when you create a 'username.github.io' repo on your profile. 

One side benefit of this is that I don't have to worry about using a `gh-pages` branch for my content. Anything that gets pushed to my master branch gets (almost) immediately pushed out to my production site. This makes updates extremely easy, which greatly increases the likelihood of me keeping things updated.

### Hoop #2 - DNS Servers

To get kevinlamping.com to point to klamping.github.io, I had to do a little bit of work updating my DNS provider configs. I won't go into too much detail, but [this content on setting up nameservers](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages/) really helped me out.

### Hoop #3 - Accidentally delete all your old blog content and random works in progress

Because I no longer hosted the code for my site on my old servers, I figured I could just delete that domain name record from the server information. However, right after pressing the delete button, I thought to myself: "Self, there was more on that server than the files for your website. You also had a couple Wordpress blogs, some old articles and a few projects that were never completed. You do realize you deleted all of that, right?"

Yep, I realized that. I guess sometimes it's best to just let go of the past, although I had some writing that I would have liked to have kept. 

## The Brighter Future

I have a few things I'd like to add to all of this:

1. UI Regression Testing - Probably Wraith. Or PhantomCSS. Or something else.
2. A Custom Theme - I like the default theme, but I also think my own site deserves its own theme.
3. More timeline details - It's hard to know what to add to your personal timeline. Too much info and you bog people down. Too little and it's not much use. Still, it'd be nice if I could integrate things like blog posts or side project work in to my timeline.
