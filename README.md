# MKT-vault
An Obsidian vault built for functional use in a professional setting for one-man-shows.
# The Idea

The idea behind this vault is to provide a viable solution to many different issues a marketing or social media manager functioning with a minimal tech stack / budget (startup or low volume business) might face. As someone who fits that description, the goals that I wanted to fulfill for myself were as follows:

- A place to store all of my meeting and communication notes, be they a quick phone call or passing conversation, or a scheduled meeting. Automatic template based generation of these notes at a single mouse click, with frontmatter housing the majority of the administrative information and the body of the note being where I would summarize or note action items. 
  
- A place to store contact information with detailed notes about them (and their organization), record of meeting/communications that I've had with them, and time since last contact. 

- A place to collate content and project ideas in a quick, streamlined, and organized manner. Frontmatter attributes which can be modified and are reflected in various data visualizations. 
  
- A place to track live content and active projects, their scope, and any notes/headwinds/analytics related to them. Frontmatter attributes which can be modified and are reflected in various data visualizations. 

- A place to track my daily productivity as it relates to various marketing efforts, projects, designs, etc. I may be working on.
  
- A place to remind myself of recent "Wins", on days when things are particularly difficult. 

- The ability to aggregate and summarize my notes on various work related topics quickly, for use in future negotiation. 

- An offline calendar I can add work events to, visible or accessible at all times. 

# The Execution

- The way I've decided to go about accomplishing this is by using Obsidian's linking features to do most of the relational heavy lifting. Through community plugins, we can leverage the database we're creating to visualize data, link data cross functionally, and make informed decisions about strategy based on those insights. Full list of community plugins provided below. 
  
  
  - Dataview provides a bunch of functionality for serving linked data in various places
  - Templater allows us to make more advanced templates than the default plugin
  - Trackers allows us to visualize the data we collect in our various notes. 
  - PixelBanner gives us the nice aesthetic banner on the homepage. 
  - Meta Bind gives us the note-creation buttons we use with Templater. 
  - Admonitions is included as I plan to replace the default callouts with Admonition style callouts for their aesthetics. 
  - Excalidraw is included because it's awesome and super useful for creating flow charts and storyboarding. 
  - Style Settings is included to allow for some tweaking of certain theme elements. 
  - Full Calendar is included because it satisfies one of my core needs for this system -- an offline calendar with event functionality. 
  - Advanced URI is included along with Hotkeys for Templates because I use these in combination with Flowlauncher to create certain notes even when Obsidian is not focused or not opened yet. 
  - Tasks is included to aggregate and track task items across the Vault, although not yet implemented. 

# How To Use This Vault

Feel free to use this vault as a starting point, edit it and make it your own. Far from me to tell you how you should use it, but I can tell you how I use it. I find that having a fairly rigid structure works better for me in a work environment than my non-work vault, where I employ a much more Zettelkasten style of note taking for my knowledge management. In this case, I want my 'work knowledge' organized and structured in such a way that things are relatively silo'd but still relationally linked. 

1. Download Obsidian from obsidian.md/download
2. Install to the directory you prefer.
3. Download this repository using the linke below "Releases" or by cloning the repository with "git clone github.com/dataskillup/MKT-vault"
4. Place the Vault folder in the location you wish for it to live permanently.
5. Launch Obsidian, choosing the second option to "Open folder as Vault..." and select the folder you just moved.
6. ***IMPORTANT*** You MUST enable community plugins when prompted in order for the various automations and templates to function correctly. 
7. I keep Obsidian open at all times on a second monitor, open to the Homepage. 
8. My homepage has all the buttons I use to create a new note based on templates. This cuts down on the friction of specifying the things I want included in frontmatter when creating a new note. 
9. If something isn't included in the template that I later decide I want, I can always add it to frontmatter. 
10. Document everything. The system is only as useful as you make it through rigid use. I come from a sales background where your paycheck is only as good as the notes you've taken on your interactions, and so I aim for the least friction in note creation I can manage. If I had JS background, I would definitely be using Dataviewjs. 
11. Use the task tracking and daily note to keep track of your productivity. 
12. Use the Dataview queries to keep track of current and potential projects, ideas, and wins on the horizon. 
13. Use the CRM as close to how you would a traditional CRM as possible. I've included the ability to include both companies and individual contacts via buttons.

#### Why use Obsidian instead of (insert product/suite here)?

- As mentioned, I'm operating with basically no real tech budget, in an environment where I'm providing my own technology, and there are no other stakeholders who will be using this system. A tool like this is invaluable in making the case for raises, budget increases, campaign success, etc. As such, I want as much control over all aspects of the system as possible. I work best when working out of a central location, so I wanted as much of the data centralized within one application as possible. I also just really like markdown as a concept, and the flexibility provided by the community through Plugins. 


#### Are there more plans for this notebook?
- Yeah, I plan to expand the functionality a bit more through the incorporation of Smart Connections and adding a section with templates for on the job skill learning notes. 

##### Acknowledgements:
- To the authors of all of the listed plugins and themes, thank you!
