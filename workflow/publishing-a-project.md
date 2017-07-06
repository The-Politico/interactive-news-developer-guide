# Publishing a project

Some simple guidelines for what to do before you hit the big red button.

### Editing process

An Interactive News editor signs off on all projects before they are published or deployed to master. See the publishing checklist below for details.

##### Design reviews

An editor will conduct a dedicated UX and design review with you, but editing interactive components should be an iterative process. Show your work early and often to an editor and the final edit will go much more smoothly.

https://www.gitbook.com/book/politico/politico-newsroom-developer-guide/edit###### Code reviews

Code reviews are required for medium and long-turn projects and for any project touching durable infrastructure like datalab. The format these will take is fluid based on the project.



---

## Publishing checklist

Make sure you've done all these things on your project before you publish.

### Copy editing

- [ ] Ensure that your project has been copy-edited.

### Meta tags

* [ ] Double check that your `meta.json` file is completely filled out.
* [ ] Triple check that you have the `publishPath` and `url` correctly configured in your publish path.
* [ ] Create a social share image at 600 x 325px, named share.jpg in the `dist/images` directory on interactive pages.
* [ ] Update the timestamp on the article every time you publish. Our style is to add an updated timestamp alongside the original when publishing additional content.

### Documentation

* [ ] Update the README in your project.
* [ ] If you're deploying an app or tool, make sure to add a `Developing` docs section with full instructions for anyone on the team to spin up your project locally.

### Github

* [ ] Create a private repo for your project and push your latest code (which you should do daily, tbh).
* [ ] Prefix interactive and embed repo names with `interactive_` or `embed_`, respectively.
* [ ] Talk with your editor about whether we will make this repo public after publishing.
* [ ] If you're working on an existing project, push your code to a branch which will be merged into master after a code review with your editor.

### Notify

- [ ] Communicate the live URL address, a preview URL and the time the story will be available to promote with any or all of the following teams:


##### Homepage

`tp-webeditor@politico`
* [ ] Provide an embed code for embeddables or request a story shell for interactives.
* [ ] Send the live URL address and time story will be available to promote.
* [ ] Suggest homepage art, which can be a gif or a static image.
    * [ ] HP art should be cut to: **1160 X 629** 
    * [ ] If time allows, offer a thumbnail to be used at smaller display sizes - this thumbnail should also be cut to 1160 X 629 (Yes, it will look huge, but it will run small on the site). This option should be more graphical.
    ie: ![](/assets/new_share.jpg)
* [ ] Remind them to send an alert for the story at publish time.


##### Social
`tp-webproducer@politico` `teischen@politico.com` 
* [ ] Supply them with any social elements, your share.jpg image, gifs, suggested share text, etc.


##### **Comms, business analytics, advertising** 
`tp-projects@politico.com`
* [ ] Send a working headline and short summary of the project 
* [ ] On bigger projects, check if a special ad map has been created for the project.


#### Slack
* [ ] Retire your project slack channel.




