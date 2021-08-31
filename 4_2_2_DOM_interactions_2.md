# 4_2_1 Dom interactions 2

Use this file as a starting point. [4_2_2.html](./4_2_2.html)

## Task 1:

Create an event listener for clicks on the accordion title. When the event listener is triggered, it should show the accordion text.

## Task 1b:

Make sure that you can toggle the accordion text. So that when you click the title a second time, the accordion closes.

## Task 2:

Make a transition for when the accordion text appears / disappears.

## Task 3:

We now want to add another accordion. The challenge now is too open and close the right accordion text. There is a number of ways to do this. But you might want to start with restructuring the HTML. Here is some suggestions for possible approaches. Try at least two of these:

- Give the accordion title and text a unique ID. Such as "accordion-title-1" and "accordion-text-1" so that you can correspond the accordion title being clicked with the text it should show.
- Place the accordion text within the accordion title (in its own div). In that way, could could show the text with some smart CSS by setting a class on the accordion title.
- Place the accordion text and accordion title together in an accordion container div. When you receive an event, find the currentTarget / target in the event object, and use that to iterate the DOM three. (find sibling, or find the parent, and it's children with a specific class (such as accordion-text).

## Task 4:

Create at least 2 more accordions, so that you have 4. Now we want to make sure that only one accordion text is open at a time. So you need to write a javascript that first closes all accordion texts that are open, and after opens the correct accordion text. You can do this using document.getElementsByClassName() or document.querySelectorAll(). Solve the the task with both of these, and keep the one you like.

## Task 5:

Create a "delete" button on the accordions. So that you can remove an accordion from the view.

## Task 6:

You have run out of accordions. You need to create a button to add more accordions to the view. The button should display a form when clicked, where the user can input a title and text. When saved, the new item should be added to the view as an accordion.
