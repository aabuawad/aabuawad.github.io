# [Hugo Academic Theme](https://github.com/wowchemy/starter-hugo-academic)

The following sections are necessary for editing the website:

*To Run Server:*
- In terminal, run: cd ~/Documents/Personal_Website/aabuawad/ (where file is located)
- In terminal, run: hugo server
- Webpage should be visible at http://localhost:1313/

*Main Page:*
- For the photo, go to content > authors > admin > and change the "avatar.jpg" image.
- For the links under the photo and the biography section, go to content > authors > admin > _index.md > and change the icon info and biography text. 
- To update the CV, go to static > uploads > and change the "cv.pdf."
- For the skills, content > home > skill.md > and change the information for the skills icons. 
- For the experience, content > home > experience.md > and change the information for the jobs. - For the company logos under experience, assets > media > icons > brands > and change the svg images (make sure to update text in experience.md to match these icons, only use .svg images; convert in images inkscape to svg)
- For the Accomplishments (now used for Honors & Awards), content > home > accomplishment.md > can add "See certificate" link by using certificate_url: '' option. For some links, icons automatically update, but for my icons, I added the svg images to brand folder as listed above and listed the svg name under organization: option. 

The number of columns in a section can be configured for most content blocks. Valid options are:

'1': a single full-width column with the section content appearing directly underneath the section title (if set)
'2': two columns with the the section title appearing on the left and the section content appearing on the right

Edit your site
This quick tutorial will explore how to customize the Academic Resume starter template. You may also find it useful for customizing other templates.

Hugo site structure
There are 3 main folders for Hugo sites:

content/ for your Markdown-formatted content files (homepage, etc.)
assets/media/ for your media files (images, videos)
config/_default/ for your site configuration files
config.yaml to configure Hugo (site title, URL, Hugo options, enable page features)
params.yaml to configure Wowchemy options (SEO, site features)
menus.yaml to configure your menu links (if the menu is enabled in params.yaml)
languages.yaml to configure your site’s language or to set language-specific options in a multilingual site
Choose the right color theme for you
Check out the color themes and have fun choosing a style you love.

Once you have settled on a color theme, edit your config/_default/params.yaml file in a text editor, such as the online GitHub editor, and set the theme option to the name of the chosen theme.

The site configuration files in the config/ folder may be formatted in either TOML, or YAML like page front matter.

When you are adding parameters to your config files, consider which section of the file they should be added to, otherwise they may have no effect.

Your theme comes with a font set to style your titles and text, but you may choose to override it by specifying one of the available font sets with the font option:

Minimal (modern)
Classic (original Academic v1 style)
Rose (traditional serif)
Mr Robot (futuristic)
The font size may be adjusted from XS (extra small) to XL (extra large) with the font_size option.

Don’t worry if you are not 100% happy with the colors or font yet, as these can be fully customized later.

Choose the right layout for you
Wowchemy has a layout for you whether you are you creating a website for your CV, academic research, blog, course, lab, business, photography, portfolio, or restaurant!

What kind of content would you like to publish? Wowchemy supports:

Pages: any general content
Landing Pages: pages that can consist of content blocks, such as the homepage
Posts: blog posts or news
Publications: import your research publications from BibTeX
Online Courses: share knowledge online
Projects: publish your portfolio or projects
Notes: collaborate on content across notebooks, sections, and pages
Software Documentation: document your software projects
Talks/Events: publish any talks which you are presenting
Slides: write slides very efficiently with Markdown, present them at your talk, and share them online
Once you have decided on the type of content that you would like to publish, take a look at the available content blocks and consider which ones you would like to add to your homepage.

Then, open your content/_index.md file (or content/home/ folder in older versions) which contains your homepage content and delete the sections that you do not want.

You can add as many content blocks as you like, or even design your very own custom block.

Next, let’s position the homepage sections according to your preference. To move a section up or down, simply cut and paste the section within your list of sections in your content/_index.md. (Or for older versions, the order is controlled by the weight option.)

Customize it
After selecting a theme and a layout, make it your own.

Core parameters
The core parameters for the website can be edited in the config/_default/params.yaml file.

Edit your personal/business details under the Contact Details section:

Any details entered here will be displayed in the Contact widget (if used)
For organizations, some contact details (such as phone) may be used to enrich search results (such as on Google)
To hide a contact field, simply clear the value to "" or comment the line out by prefixing it with a hash (#)
The contact form can be configured separately in the front matter of the Contact widget itself
If you are an organization or project,

edit your site_type to reflect the nature of your business
add your organization or project name under org_name
save your logo image as logo.png and upload the image to the assets/media/ folder, creating the assets and media folders if they don’t already exist at the root of your site
Enable rich content for your site under the Site Features section. If you write technical content, consider enabling the following options, otherwise set these options to false:

Code syntax highlighting with highlight = true
LaTeX math with math = true
Mermaid diagram drawing with diagram = true
The Privacy Pack can also be activated from the Site Features section. When the privacy pack is enabled, a cookie consent message will be shown to visitors (linking to your Privacy Policy) and visitor IPs anonymized in Google Analytics (if enabled).

To add a Privacy Policy, create a privacy.md file in your content folder and remove any draft option from the front matter to publish it.

Similarly, to add Legal Terms, create a terms.md file. Links to these documents will automatically appear in your site footer.

Introduce yourself
By default, a superuser is created with the username admin and corresponding user profile located at content/authors/admin/_index.md. Let’s open this file in a text editor and edit this file to make it your profile:

Add your display name (typically your full name) to the title field
Add your role/position or tagline to the role field
Write a brief sentence to describe yourself in the bio field - this can appear in the list of authors after the page content
Edit the organizations that you are affiliated with, or set this to [] to hide it
List your interests or hobbies in interests, or set this to [] to hide it
List your main qualifications using the education –> courses block
These blocks can be created or deleted as required
To hide qualifications, delete these blocks or comment out the lines by prefixing them with a hash (#)
Add your social or academic networking links
These are defined as instances of social and can be created or deleted as required
Now let’s add a biography or some fun facts about you after the front matter (i.e. after the last --- line). You can utilize Markdown and shortcodes for formatting.

To display an avatar, place a square cropped portrait photo named avatar into your profile folder at content/authors/admin/, overwriting the example image. Alternatively, if you have an existing Gravatar/Wordpress avatar, you can use it by setting gravatar to true in config/_default/params.yaml and entering your associated email address in content/authors/admin/_index.md. Note that you can delete the example avatar image to disable the avatar feature.

Once you have setup your account, your username can be referenced in the authors field in the front matter of content, as per the demo post.

Your display name, entered in your user profile, will then automatically appear in the page metadata. You can also enter additional names in the authors field of pages, with the option to create a user profile for them too if you wish. If a user profile doesn’t exist for an author, their name will appear exactly as you entered it in the front matter.

The superuser username can be changed from admin by renaming the admin folder. Usernames must be lowercase with any spaces replaced with hyphens (-).
If you change a username, you may wish to update any references to it from the author field of any About blocks (such as on your homepage at content/_index.md) and the authors field in the front matter of any pages which reference that user.
Menu
The main menu links in the navigation bar can be edited in the config/_default/menu.yaml file.

For example, to link to the homepage and an about page, we paste their relative URLs from the root of the site:

main:
  - name: Home
    url: /
    weight: 10
  - name: About
    url: about/
    weight: 20
To order your links, set the weight option to any numbers. Here we use multiples of ten so that it’s easier to change the order in the future if we have many menu items.

Linking to page sections

To link to a section of the homepage, use the form #<section-filename> where <section-filename> is section id. For example, #posts references a section with id: posts. You can rename your section ids in content/_index.md, just remember to use a dash (-) instead of spaces in the unique section identifier.

Sub-Menus

To create a dropdown sub-menu, add identifier: a-unique-reference to the parent item and parent: a-unique-reference to the child item, replacing a-unique-reference with a unique reference of your choice.

Example of creating a Tags sub-menu:

main:
  - name: Home
    url: /
    weight: 10
  - name: Tags
    identifier: tags
    weight: 20
  - name: Academic
    parent: tags
    url: tags/academic/
    weight: 10
Learn more about the underlying Hugo menu system here.

Add your content
Refer to our guide on managing content to create your own content such as blog posts, publications, online courses, talks, and projects etc.

Remove any unused example pages
Tidy up your site by deleting any unused pages leftover from the example template.

You will likely want to keep the _index.md files (notice the underscore prefix) as they configure the archive page for each content type (e.g. an index of all your blog posts).
Your Markdown-based site structure will be similar to:

📄 LICENSE.md
📄 README.md
📄 academic.Rproj - (optional) For RStudio users, otherwise can be deleted
📁 assets
📁 media
📄 icon.png - (optional) add your website icon here
📄 logo.png - (optional) add your logo here
📁 config
📁 _default
📄 config.yaml - define your site name and URL
📄 languages.yaml - edit this for non-English or multilingual sites
📄 menus.yaml - define your site menu
📄 params.yaml - personalize your site
📄 config.yaml - (optional) a dummy file for RStudio compatibility - non-RStudio users can delete
📁 content
📁 authors - user profiles
📁 admin - your username (can rename)
📄 _index.md - your user profile
📄 avatar.jpg - update with a photo of yourself or delete to not show any photo
📁 home - your homepage - personalize the homepage with widgets
📁 post
📄 _index.md - (optional) an archive of blog posts
📄 privacy.md - (optional) your privacy policy
📁 publication
📄 _index.md - (optional) an archive of publications
📁 talk
📄 _index.md - (optional) an archive of talks
📄 terms.md - (optional) your site’s terms and conditions
📁 data
📄 page_sharer.toml - (optional) customize social sharing buttons
📄 netlify.toml - (optional) defines Hugo version for deploying with Netlify
📁 scripts - (optional) scripts to maintain the template repository - can be deleted
📁 static
📁 admin - (optional) your Netlify CMS admin panel
📄 update_academic.sh - (optional) a script to help update Academic
📄 view.sh - (optional) a script to view your site locally
View your site
If you installed on your computer with Git or ZIP, view your new website by running the hugo server command.

If you installed using RStudio, run blogdown::serve_site() to preview your site in your web browser. We recommend previewing your site in your normal web browser as the in-built RStudio web browser is outdated and buggy.

Now visit localhost:1313 and your new Academic powered website will appear. Otherwise, if using Netlify, they will provide you with your URL.

Deploy your site
Before deploying your site, there are some final options we can set in config/_default/config.yaml:

Set title to your desired website title, such as your name or business name
Set baseurl to your website URL (this can be provided by your host such as Netlify)
You can make a great impression on your visitors with your own custom domain name
If you don’t have your URL/domain yet, come back to add it later - some features may not fully function until it is added
Publish your site to the world by following the deployment steps.

Inspiration
For inspiration, refer to the Markdown content which powers the demo of Academic Resume Template.

Support Wowchemy and its templates
Has Wowchemy and its templates helped you?

Wowchemy and its starter templates are open source and provided to you for free. An incredible amount of effort has gone into developing and maintaining the software. Please kindly consider giving back and supporting further development by sponsoring.
