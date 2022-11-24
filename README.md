# builder-nika
Nika Khanjani's Personal Site

## To Edit
Clone to local, `cd` into project root and enter `hugo server -D` to compile and run. Changes to code are available instantly.

NOTE: If you don't have [Hugo](https://hugo.dev) installed on your system, use `homebrew` and the `brew install hugo` command. Learn about [homebrew here](https://brew.sh).

## Using the SubModule
This builder users a base theme from a SubModule. To pull the submodule, you need to run:

````
git submodule update --init --recursive
````

after you clone the site.

## To Deploy
Simply commit changes and push back to the `main` branch. Site will be compiled and visible automatically at:

https://dev-tnb-builder-mac.netlify.app

# Getting Started with the TNB Site Builder

The TNB Site Builder is powered by Hugo. If you want to create a brand new site, follow these steps:

1. Create a repo on github called `TNB3000/builder-YOUR-SITE`
2. On your local machine, if not already installed, use `homebrew` to install HUGO: `brew install hugo`
3. Create a local folder for your site and `cd` into it
4. Create a new site named `your-site` by entering `hugo new site your-site`
5. Add the TNB Starter theme site with :

````
git init
git submodule add git@github.com:TNB3000/hugo-tnb2021.git themes/tnb2021
````

6. Edit `config.toml` and set `theme = "TNB2021"`

7. Start the Hugo Server in draft mode `hugo server -D`

And start hacking away at overriding the base theme, as per Hugo documentation:

https://bwaycer.github.io/hugo_tutorial.hugo/themes/customizing/