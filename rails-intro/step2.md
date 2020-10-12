## We have an app!

Now that we have our app, we can start to add some crud functionality. For our first CRUD resource let's create some 'Zas bra. 

We'll Create our pizza resource with several properties and types:

```
name: string of text
cost: integer
description: block of text
vegetarian: boolean
```

Fortunately for us, Rails allows us to `scaffold` a resource, automagically building all of the CRUD functionality out of the box!

Run this command:

`rails g scaffold Pizza name:string cost:integer description:text vegetarian:boolean` {{execute}}

Once that's done we'll want to make sure this is setup in our database properly by running:

`rails db:migrate`{{execute}}

Congrats! We've done it!