1. use the following commends to build up my website on git-page
    
        git init
        git checkout -b gh-pages
        git status
        git add .
        git commit -m "init commit"

        git remote add origin [http://...](https://github.com/xiaorong117/Team_blog.git)
        git push origin gh-pages

2. use the following commends to update my website on git-page

        git status
        git add .
        git commit -m "init commit"
        git push origin gh-pages

3. the site is as follows:
***https://xiaorong117.github.io/Team_blog/***

1. use the following commends to see my local website
    
         bundle exec jekyll serve

2.  _config.yml
    - default settings for posts and image
  
        ```
        defaults:
            - scope:
                path: ""
                type: "posts"
            values: 
                layout: "post"
                categories: "my-blogs"
                permalink: /:categories/:day/:month/:year/:title.html
            - scope:
                path: "assets/img"
            values:
                image: true
        ```
    - baseurl: "/Team_blog" # the subpath of your site, e.g. /blog
3. 

    
         


---
layout: "post"
title:  "This is my first draft blog with keylly"
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/