# udacity
As we refresh the page, the first page with heading of "Feeds" is visible, it quickly moves to the "Udacity Blog"
page (which is the home page and the first entry in allFeeds global array loaded by default), after which the
"CSS Tricks" page is visible. This page is loaded as part of testing loadFeed() functionality. The last page
visible is the "HTML5 Rocks" which is loaded to test whether loadFeed() changes content.

1. The first test suite, called the RSS feed, checks whether the global array allFeeds is defined and does not have a length
   of zero.
2. The second test suite, called the "the Menu" has 2 specs
    - The first spec is to check whether the menu is hidden by default as the home page is loaded.
    - The second spec is to check whether the clicking of the hamburger menu icon, hides/shows the menu. For
      testing this, the menu icon is clicked and checked whether the side menu appears. It is clicked again
      through code, and checked whether the side menu hides. DISCLAIMER : Since consecutive clicks are made,
      the showing/hiding of menu is not visible.
3. The third test suite, called "Initial Entries" checks whether the loadFeed() populates the .feed container.
   As part of testing the function, index value of 1 is provided to the loadFeed() which is the "CSS Tricks" page
   and is visible on the screen.

4. The fourth test suite called "New Feed Selection" checks whether the content changes after loadFeed() is
   executed. Here loadFeed() is executed with an index value of 2 and hence the "HTML5 Rocks" page is visible.
