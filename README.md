# Noted
## The free web notes app, written in Angular & NestJS

------------------------------------------------------------

Noted is a web application that provides a simple interface to add, edit and delete notes from a database.<br>
It can be ran locally, with all the data stored on your machine, or elsewhere on the network or even the wider internet, if you choose so.<br>
A Sqlite3 database is used for the advantage of running no additional services like a MySQL server.<br>

----------------------------------------------------------------

## Installation

Prerequisites:
- [Node](https://nodejs.org/) and NPM (usually comes with Node) installed
- [Git](https://git-scm.com/) installed

----------------------------------------------------------------

### Serving the app with Nest + Serve

1. Clone the repos:<br>`git clone https://github.com/sbcomputertech/Noted-front`<br>and<br>`git clone https://github.com/sbcomputertech/Noted-back`
2. Create the build directories: `mkdir build`
3. Go into the front-end repo: `cd Noted-front`
4. Install dependencies: `npm install`
5. Build using the angular command line: `ng build`
6. Copy the output to the build folder: `cp -r dist/noted/* ../build`
7. Go back to the original directory: `cd ..`
8. Go into the back-end repo: `cd Noted-back`
9. Install dependencies: `npm install`
10. Build using nestjs command line: `nest build`
11. Run the built back-end headlessly: `node dist/main.js &`
12. Go to the build directory: `cd ../build`
13. Install the global serve package: `npm install --global serve`
14. Serve the front-end: `serve -p 2000 front`
15. Test it out!
