# Blog

This repo contains a scaffold that is ready to be deployed to Heroku for a simple blog application.

# Tasks

1. Deploy to Heroku: `heroku create --region eu` + `git push heroku master`
1. A `post` model. It should contain a `title:string`, `body:text`
1. Create a blog controller that is at the root of the application, that displays a list of blog entries, and
   allow the reader to click on individual entries to see more
1. Create an `admin/posts`-controller where you can edit your posts
1. Validate that the blog has a title and a body
1. Deploy to Heroku
1. Add a boolean `published` column (default value should be false), that allows you to toggle whether or
   not a blog post should be shown on the front page of the blog
1. Deploy to Heroku

Notice: once you have added a model, or a migration to your app, you need to migrate the database on
heroku as well! Locally you do it with `bundle exec rake db:migrate`. On heroku you will need to do it
with `heroku run db:migrate`
