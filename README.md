# Exercise 3: No more Mister nice Todo List!
Big times, everyone; databases getting bigger, requirements toughter. One more time, this exercise consolidates all pieces of knowledge you've got. We've already got taste of the React and Redux and now it's time to handle some routing.

This project has nothing new in it. Literally, I haven't done anything, only dreamed of the next steps and guess what, the very implementation is on you guys. :slightly_smiling_cute_face_emoji:

#### *NOTE1*: We begin with the same old `dev-server` here, (and in the process we'll hopefully move to real db). I haven't added new styles since the last assignment, so you need to provide your own sulition and please be creative 🎉🎉🎉

#### *NOTE2*: The setup didn't change since the last assignment either, meaning, you have all the good stuff here, React + Redux, but we'll definitely need Router as well, which you need to install on your own and connect stuff together and finally make the things happen. :fingers_crossing_even_cuter_face_emoji:

#### *NOTE3*: Our database that is served by the dev-server now has much more data and at the moment you still need to spin it up on your own machine. Task lists for previous days are available by the following api: `http://localhost:8686/YYYY-M-D` (*for example: `http://localhost:8686/2019-1-19` if you wish to get tasks for the January 19*). When adding new todoes please follow the same syntax for URL as well. A total list of all previous tasks, which you will need for `Calendar` component must be fetched here: `http://localhost:8686/allTasks`. There is no implementation available, so I will support you if there are any difficulties.

#### *NOTE4*: THE TASKS IN THE DB ARE FAKE AND WERE AUTO-GENERATED BY A 'SUPER COMPUTER SOFTWARE 💻' SO DON'T BLAME ME IF THERE IS SOMETHING RIDICULOUS 🙃

## Considering that the application works after the last two assignments, here is what else we need on top of it to complete this task:
  1. Application opens showing todo list of *today* (plus add proper date on top, styling is up to you).
  2. Pay attention to buttons: `Back`, `Fwd` and `Calendar` on the first snapshot below.
  - Back and Fwd buttons are used for navigating in the history and getting todos based on the date (date format YYYY-M-D).
    * Fwd must be inactive if the date is today.
    * URL should change based on the date presented. For example: If we are presenting a task list for the *26th of January*, url should look like: `http://localhost:3000/2019-1-26` and so on.
    * It should be possible to just enter url in the same format and get a page with tasks list of that day.
  3. `Calendar` button shows us a grid with todos for previous month, see the second snapshot below (at the moment only January is provided).
  - Each day is presented as a square-card with the tasks in it.
    * It should be possible so see which tasks are completed and which are not.
    * Each task in the database has a specific `tag`(#family, #work, #misc...) specifying the type of task. Add a small cirle in front of task name for specific tag (pick colors on your own, but be consistent i.e one use color per tag).
    * It should be possible to go back and fwd between months as well (buttons are missed on the snapshot, but you got the idea).
    * Calendar should be available by the link: `http://localhost:3000/calendar`.

#### HAPPY HACKING! 🙌

#### Snapshot 1: Todo list with today's date and a new set of buttons  
![Snapshot 1](https://raw.githubusercontent.com/voogieJames/react-101/exercise3/snapshots/snap1.png)


#### Snapshot 2: Calendar view with tasks for the last month
![Snapshot 2](https://raw.githubusercontent.com/voogieJames/react-101/exercise3/snapshots/snap2.png)


## Available setup

After cloning the repo you need to start npm project, meaning, download all dependencies(`npm install`) and then you can run following scripts:

### `npm start`
Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm run dev-server`
Starts local *dev-server* run on the port `8686`.


