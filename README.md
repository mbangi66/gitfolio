# gitfolio
personal website + blog for every github user Gitfolio will help you get started with a portfolio website where you could showcase your work + a blog that will help you spread your ideas into real world. Check out this live demo to see gitfolio in action.


Getting Started
Let's Install
Install gitfolio

npm i gitfolio -g
Let's Build
gitfolio build <username>
<username> is your username on github. This will build your website using your GitHub username and put it in the /dist folder.

To run your website use run command (please refrain from using this for now)

gitfolio run
🎉 Congrats, you just made yourself a personal website!

Let's Customize
Forks
To include forks on your personal website just provide -f or --fork argument while building

$ gitfolio build <username> -f
Sorting Repos
To sort repos provide --sort [sortBy] argument while building. Where [sortBy] can be star, created, updated, pushed,full_name. Default: created

$ gitfolio build <username> --sort star
Ordering Repos
To order the sorted repos provide --order [orderBy] argument while building. Where [orderBy] can be asc or desc. Default: asc

$ gitfolio build <username> --sort star --order desc
Customize Themes
Themes are specified using the --theme [theme-name] flag when running the build command. The available themes are

light
dark
TODO: Add more themes

For example, the following command will build the website with the dark theme

$ gitfolio build <username> --theme dark
Customize background image
To customize the background image just provide --background [url] argument while building

$ gitfolio build <username> --background https://images.unsplash.com/photo-1557277770-baf0ca74f908?w=1634
You could also add in your custom CSS inside index.css to give it a more personal feel.

Let's Publish
Head over to GitHub and create a new repository named username.github.io, where username is your username. Push the files inside/dist folder to repo you just created.

Go To username.github.io your site should be up!!

Updating
To update your info, simply run

$ gitfolio update
This will update your info and your repository info.

To Update background or theme you need to run build command again.

Add a Blog
To add your first blog run this command.

$ gitfolio blog my-first-blog
(use "-" instead of spaces)

This will create a my-first-blog folder inside blog. Inside my-first-blog you will find an index.html file which contains all the necessary elements for writing a blog. Customize the content of the file to write your first blog.

This also adds content to blog.json file. This file helps in showcasing your blogs on your personal website as cards. You could customize the JSON object that corresponds your current blog.

Blog Demo? here

Default JSON Format

{
  "url_title": "my-first-blog", // the title you provide while creating a new blog, this appears in url
  "title": "Lorem ipsum dolor sit amet", // main title of blog
  "sub_title": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.", // sub-title of blog
  "top_image": "https://images.unsplash.com/photo-1553748024-d1b27fb3f960?w=1450", // main image of blog
  "visible": true // don't worry about this
}
