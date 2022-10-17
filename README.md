# Groundflr Take-Home Test

## The Goal

Design a UI that renders a [list](https://vuetifyjs.com/en/components/data-tables/) of users with columns corresponding to the following data i.e. `firstName`, `lastName`, `age` and `actions`. The `actions` column will display either a [`checkbox`](https://vuetifyjs.com/en/components/checkboxes/) or [`button`](https://vuetifyjs.com/en/components/buttons/) that toggles between two kinds of visual and behavioural states i.e. assigned and unassign. On clicking either actionable a `user` should be toggle -assigned, or -unassigned, to the corresponding `LearningExperience`, which to all intents and purposes is the domain name for a learning resource type such as an article, video, meeting, project, etc. The schema of both the `User` and `LearningExperience` are avialable on the [`server`](git@github.com:groundflr/groundflr-test-server.git) under the `./app/Repository/Schema` folder.

## Project Structure

The project is divided into two apps the `client` app and `server` app.

1. A [`vue`](https://vuejs.org/) powered client, created using [`vue cli`](https://cli.vuejs.org/)
2. An [`Express`](https://expressjs.com/) powered server exposing a REST API.

## Evaluation Criteria

1. Maintainability; usage of well-meaning naming conventions, [SOLID](https://en.wikipedia.org/wiki/SOLID) and functional principles.
2. Effeciency; solving a business problem with as simple as solution as feasible i.e. ["...[m\]uch less code ... doing much, much more...]"](https://blog.cleancoder.com/uncle-bob/2013/11/19/HoardsOfNovices.html)
3. Since the test was design to be acomplished by using client side storage such as `localStorage` or even `sessionStorage` the `server` app is optional however if you've the time and need to show off coding chops you can include it as part of the solution.
4. TypeScript, ESLint, testing, CI/CD setups, deployments, etc. are out of source however bonus marks *can* be awarded for using the same to show off coding chops.

## Setup instructions

Follow these instructions to get the projects up and running:

1. Install Node.js. Make sure you have [Node](https://nodejs.org/en/download/) >= v14.19.3 installed on your machine.
2. Install [MongoDb](https://www.mongodb.com/docs/manual/installation/) or database of your choice if you're using the `server` app.
3. Download the [client](git@github.com:groundflr/groundflr-test-client.git) and [server](git@github.com:groundflr/groundflr-test-server.git) repositories.
4. Install dependencies.

    This will install the Node dependencies for both projects.

    ```bash
    cd cd path/to/<repository>/
    npm i
    ```

5. Starting the two app

    ```bash
    cd path/to/groundflr-test-client/
    npm run serve

    cd path/to/groundflr-test-server/
    npm run dev
    ```

6. Open http://localhost:8080/ and http://localhost:8081 to verify if the client and server application work respectively.
7. And, you're all set up!

## Submitting Code

We would prefer that you share the code via a GitHub, BitBucket, or GitLab repository to make it easier for us to view and discuss with you if we have questions.

If you share your code via a private repo, please give the following email addresses access:

- dev@groundflr.co
- tafadzwa@groundflr.co
- nic@groundfr.co

### Customizing Configuration for Vue
See [Configuration Reference](https://cli.vuejs.org/config/).
