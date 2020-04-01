# Hang In There

A boilerplate repo.

## Set Up

1. One teammate: fork this repository
2. Go to settings and turn on GitHub Pages for this repository
3. All teammates: clone down this repository
4. `cd` into the repository
5. Run `open index.html` to view it in the browser

## Progression

### Iteration 0 - Main Page

![Screen-Shot-2020-04-01-at-2-52-36-PM.png](https://i.postimg.cc/dV78HSYC/Screen-Shot-2020-04-01-at-2-52-36-PM.png)

- When the page loads, we should see a poster with a randomly selected image, title, and quote

- When the page loads, we call the randomize function. The randomize function uses the getRandomIndex function to bring back an image, title, and quote for the main page.

### Iteration 1 - Switching Views

Form page:
![Screen-Shot-2020-04-01-at-12-53-21-PM.png](https://i.postimg.cc/25zpYvSC/Screen-Shot-2020-04-01-at-12-53-21-PM.png)

Saved posters page (once working with extra saved posters):
![Screen-Shot-2020-04-01-at-12-54-14-PM.png](https://i.postimg.cc/BtWyVPz9/Screen-Shot-2020-04-01-at-12-54-14-PM.png)

- When a user clicks the "Make Your Own Poster" button, we should see the form, and the main poster should be hidden

- We added an event listener for the click on the make my own poster button, a function is called that reassigns the hidden class to the main poster class and off the poster form class. We applied this same idea to the rest of the buttons on the app

_Hint: go check out the HTML and CSS files to see how the form and saved posters sections are being hidden in the first place_

## Iteration 2 - Creating a New Poster

Form being filled out:
![Screen-Shot-2020-04-01-at-12-51-59-PM.png](https://i.postimg.cc/d0nbV1hr/Screen-Shot-2020-04-01-at-12-51-59-PM.png)

Once poster is saved:
![Screen-Shot-2020-04-01-at-12-52-14-PM.png](https://i.postimg.cc/sXNb5N92/Screen-Shot-2020-04-01-at-12-52-14-PM.png)

- On the new poster form view, users should be able to fill out the three input fields and then hit the save button
- When the save button is clicked, several things will happen:
  - Save the submitted data into the respective arrays (image URL into the images array, etc) so that future random posters can use the user-created data
  - Use the values from the inputs to create a new instance of our Poster class
  - Change back to the main poster view (hiding the form view again)
  - Display the newly created poster image, title, and quote in the main view

## Iteration 3 - Saving & Viewing Posters

Saved posters view:
![Screen-Shot-2020-04-01-at-2-52-36-PM.png](https://i.postimg.cc/dV78HSYC/Screen-Shot-2020-04-01-at-2-52-36-PM.png)

- When a user clicks the "Save This Poster" button, the current main poster will be added to the `savedPosters` array.
- If a user clicks the "Save This Poster" more than once on a single poster, it will still only be saved once (no duplicates)
- When a user clicks the "Show Saved Posters" button, we should see the saved posters section
- All the posters in the `savedPosters` array should be displayed in the saved posters grid section

## Iteration 4 - Deleting Saved Posters

- From the saved posters view, if a user double clicks a saved poster, it will be deleted

_Hint: How will you update the data model to achieve this?_

## Optional Extensions - Gettin' fancy

Here's a list of possible extensions to implement - but **ONLY IF** your team has completed all the previous iterations **AND** have cleaned up your code to make it DRYer and more readable.

You are welcome to add your own extensions. Be sure they are thoughtful in terms of UX/UI, and that they do not break any prior functionality.

- Implement data validation and error handling into the form (disable button, provide error messages if data entered is not correct, etc)
- In the main poster view, allow users to click each piece of the poster (image, title, quote) to update just that piece with another random item from the appropriate array
- When a user single clicks a saved poster, create a modal to view it larger
- Allow users to drag and drop saved posters into whatever order they want them to appear


Project spec & rubric can be found [here](https://frontend.turing.io/projects/module-1/hang-in-there.html)
