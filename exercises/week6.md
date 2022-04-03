# Week 6

## Twine

### Change the Story Styles

1. In the bottom right of Twine click the title of your story to reveal the menu.
2. Select "Edit Story Stylesheet".
3. Add styles for the story, links and change the font.

Example styles:

```css
@import url('https://fonts.googleapis.com/css2?family=Homemade+Apple&display=swap');

tw-story {
  font-family: 'Homemade Apple', cursive;
  color: #FFF;
  background-color: #000;  
}

.story-image {
  width: 100%;
}

tw-link, tw-link:link, tw-link:visited {
  color: #FFF;
  text-decoration: underline;
}
tw-link:focus, tw-link:hover, tw-link:active {
  color: #FFF;
  text-decoration: none;
}
```

## Inform 7

1. Go to the [Inform 7 website](http://inform7.com/) and download a copy of Inform.

### Create a Inform 7 Story

1. Create a repository with on [GitHub](https://github.com/) (with an empty .gitignore)
2. Add the repository locally with [GitHub Desktop](https://desktop.github.com/)
3. Open the .gitignore with [Visual Studio Code](https://code.visualstudio.com/) and add the list shown
   ```
   # mac
   .DS_Store

   # inform
   *Build
   *Index
   *.plist
   *.blurb
   *.rtf
   *.iFiction
   *.skein
   ```
4. Commit the change
5. Open Inform 7 and create a new project
6. Save the project in your repository directory
7. Add some text to the file leaving the name of the project and your name where Inform adds it. Make sure to include "Release along with an interpreter." on the line between your story title and the story text:
   ```
   "Story title" by Your name

   Release along with an interpreter.

   The Living Room is a room. West is The Kitchen. The Living Room has the description "The room is well lit."

   The Kitchen is a room. The Kitchen has the description "This is where we cook."
   ```
8. Click "Go!" to test
9. Click "Release" to release
10. Commit the change
11. Push to GitHub

### Publish the Inform 7 Story with Netlify

1. Go to [Netlify](https://www.netlify.com/)
2. Select "Add a new site"
3. Select "Import an existing project"
4. Select "GitHub" as your Git provider
5. Select the repository that you created for your Inform story
6. Leave the branch to deploy as `main`
7. For the "Publish directory" make this `Rooms.materials/Release`
8. Click "Deploy site"

## Bitsy

You will be editing your Bitsy story in the Bitsy Game Maker.

### Create a Bitsy Game

1. Open GitHub Desktop and create a new repository for your Bitsy game
2. Go to the [Bitsy Game Maker](https://ledoux.itch.io/bitsy)
3. Select "Run tool"
4. There are a lot of different things that you can do with Bitsy so look at this [Bitsy tutorial](http://www.shimmerwitch.space/bitsyTutorial.html) and make some changes to your Bitsy game
5. Select "download game" depending on your browser set up this will either download the file to where that is configured or give you a choice
   - If given a choice save it as `index.html` in the repository you created in step 1
   - Otherwise, find where it has downloaded to and copy it as an `index.html` into the repository you created
6. Commit the change
7. Push to GitHub

### Publish the Bitsy Game with Netlify

1. Go to [Netlify](https://www.netlify.com/)
2. Select "Add a new site"
3. Select "Import an existing project"
4. Select "GitHub" as your Git provider
5. Select the repository that you created for your Bitsy game
6. Leave the branch to deploy as `main`
7. Click "Deploy site"
