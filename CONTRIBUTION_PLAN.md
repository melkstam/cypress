# Contribution plan

Vilhelm Melkstam - *vilme951*

## Chosen open source project

I have decided to contribute to [Cypress](https://www.cypress.io/), an end-to-end testing framework for testing front-end applications. It is built in JavaScript and TypeScript with a front-end using [Vue](https://vuejs.org/) running as an [Electron](https://www.electronjs.org/) app. Cypress does not rely on selenium or any other web driver but instead uses its own in-house driver and is compatible with multiple different browsers, electron included. While mainly used for e2e tests, component testing is in beta.

### Statistics

| **Statistic**               | **Value** |
|-----------------------------|----------:|
| **Commits**                 |   ~18 500 |
| **Issues**                  |     ~2700 |
| **Contributors**            |      ~390 |
| **Weekly NPM downloads**    |       ~4M | 
| **Contributors last month** |        37 | 

`cloc --vcs git --md .` gives

| **Language**        |    files |     blank |   comment |       code |
|:--------------------|---------:|----------:|----------:|-----------:|
| **TypeScript**      |     1483 |     35650 |     23657 |     153670 |
| **JavaScript**      |     1433 |     37543 |     16937 |     145764 |
| **JSON**            |      354 |        53 |         0 |      46170 |
| **diff**            |       18 |        42 |       341 |      45638 |
| **Vuejs Component** |      264 |      2197 |       479 |      19026 |
| **HTML**            |      364 |      1427 |       103 |      17445 |
| **Markdown**        |      178 |      3587 |         0 |       6544 |
| **JSX**             |      171 |       825 |       372 |       4241 |
| **SCSS**            |       43 |       803 |       340 |       4111 |
| **YAML**            |       22 |       208 |       191 |       3406 |
| **Text**            |       14 |      1135 |         0 |       1508 |
| **GraphQL**         |        2 |       536 |      1013 |       1166 |
| **SVG**             |      217 |         1 |         0 |       1050 |
| **CSS**             |       30 |       117 |         2 |        762 |
| **Bourne Shell**    |       10 |        65 |        18 |        177 |
| **Svelte**          |        7 |        23 |         0 |        122 |
| **CoffeeScript**    |       22 |        13 |         3 |         76 |
| **EJS**             |        4 |         5 |         0 |         30 |
| **XML**             |        1 |         0 |         0 |         12 |
| **CSV**             |        3 |         0 |         0 |          9 |
| **SUM:**            | **4640** | **84230** | **43456** | **450927** |

## Technical difficulty

Below are my estimations of the technical difficulty marked in **bold**. To start of, the test suite is quite extensive and includes multiple different types of tests. When running these, I get some errors on my machine which I could not trivially solve. The build does however seem to be a bit simpler and I have yet not run into any problems.

As for domain knowledge, there are quite a few advanced concepts such as network stubbing, controlled code execution, interaction with browsers and other concepts which makes the application a bit complex.

Lastly, the project is about ~450 KLOC with several components such as CLI, test executor, driver, stubbing etc. This together with the quite extensive dependency list (as is common for JS/TS projects…). All these interact with each other and are tested.

| Technical difficulty | Build and test environment                  | Domain knowledge requirements                                        | Size                                                                                                                              |
|----------------------|---------------------------------------------|----------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **Easy**             | No configuration needed                     | No expertise apart from course-level knowledge required              | 50-400 KLOC, 0-3 external static libraries required.                                                                              |
| **Medium**           | **File settings and manual build steps**    | **A few specific new algorithms or tools to learn**                  | **400 KLOC-1MLOC, several components built and tested against both internal and external components.**                            |
| **Hard**             | Custom configuration languages, build tools | Several weeks or months of study estimated for initial contributions | More than 1 MLOC, several components shipped in multiple versions with dependencies on each other as well as external components. |

## Process difficulty

The team at Cypress does utilize labels for their [issue tracker](https://github.com/cypress-io/cypress/issues), of which some concern the difficulty. However, there is a quite small subset of the issues that uses these labels (around 100 of 2700), meaning that they are not necessarily very helpful.

The team have some guides on how to develop and contribute to the project, but nothing extensive. I have not really battle-tested the guides and documentation for developers yet, but hope to get a good start from it.

Lastly, Cypress has what seems like an active Discord where users and developers can interact with each other. The team at Cypress seem to be very welcoming and nice to everyone. As Cypress is a for-profit company with hired developers, I will of course not have access to their internal communications, in which they hold discussions and make decisions.

| Process difficulty | Issue tracker                                    | Documentation                                                              | Communications                                              |
|--------------------|--------------------------------------------------|----------------------------------------------------------------------------|-------------------------------------------------------------|
| **Easy**           | Contains issues tagged as suitable for beginners | Contains guides and tutorials for new developers                           | Contains specific communication channels for new developers |
| **Medium**         | **Contains issues marked with difficulty**       | **Contains introduction chapters and suggested readings in documentation** | Contains open communication channels                        |
| **Hard**           | No metadata on difficulty in issue tracker       | No clear introduction to new developers                                    | **Restricted communication channels**                       |

> NOTE: The issue tracker difficulty has been decreased from hard to medium due to the fact that the (relatively) small number of issues that have difficulty labels has been useful.

## Development process

While Cypress is open source, it is still a for-profit company behind it. I think this can make contributing a bit harder as I, on some level, will "compete" with people being paid to contribute to the project. This also means that they have bigger resources to create good processes and tools to use, meaning I think it can be hard for me to reach what is here considered "Hard". I do however aim to do serious contributions and to help out. I do think I have some qualities and experience from work and earlier hobby projects which could come handy.

| Development process | Group contributions                                                                                                      | Planning and reflection                                                                                                                                                 | Engineering practice                                                                                                      |
|---------------------|--------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Easy**            | **Shares code, tutorials and development tips to other members of the team. Actively participates in project meetings.** | **Creates a plan for each sprint with sufficient details to guide the work, amounting to a number of hours that correspond the amount of credits given by the course.** | Uses the required set of tools and suggested practices for code contributions in the host project                         |
| **Medium**          | Shares documentation and material, and also gives valuable feedback on others' contributions                             | ****Uses the plan actively and updates the plan to take into account new information and events****                                                                     | **Takes care to follow established good practices in continuous development and testing**                                 |
| **Hard**            | Actively helps team members improve, and provides tutorials or other help to team members                                | Uses external sources from the host project to validate the feasibility of the plan and to update accordingly                                                           | Contributes with general quality improvements for the process of developing, building and testing software in the project |

> NOTE: This has been lowered due to me understanding these as being related to the Cypress team, not the sprint group. Having a separate and quite different project has made it harder to share input and similar.

## Individual contribution

My goal is to reach a medium level on the individual contributions. I hope this is possible given the complexity of the project and the fact that it has a lot of open issues.

## Point summation

| Category                | Level       | Points |
|-------------------------|-------------|-------:|
| Technical difficulty    | Medium      |     12 |
| Process difficulty      | Medium/Hard |      7 |
| Development difficulty  | Medium      |      8 |
| Individual contribution | Easy/Medium |     10 |
| **Total**               | **Grade 4** | **37** |

## Sprints

### Sprint 1 (week 37-39)

- [x] Introduce myself in the Discord server
- [x] Read [contributing guidelines](https://github.com/cypress-io/cypress/blob/develop/CONTRIBUTING.md)
- [ ] Make first (small) PR
- [ ] Find good first (larger) issue to contribute to

The contribution guidelines were very good and useful. Most of it was very reasonable.  

As for the PR, even though there are 2.7K issues, most of them seems to be quite complex from what I've found. Will have to move this to next sprint.

### Sprint 2 (week 39 - 41)

This sprint was mostly about the first issue and pull request. I have also searched of more issues to take on, but I have noticed it's generally hard to get an understanding of how hard/complex issues are. I think this is mostly due to there being many moving parts and different sub-packages. 

* [Issue](https://github.com/cypress-io/cypress/issues/23995)
* [Pull Request](https://github.com/cypress-io/cypress/pull/24089)

What I noticed was the speed of development they had. I see this as both nice and as a bit of a trouble as it's nice to know that I can get quick responses, but I at the same time need to be quick with PRs and issues to get them solved and merged into the `develop` branch. 

### Sprint 3 (week 41 - 44)

Used Cypress a bit more on a project at work to get to know Cypress and its features. This sprint also included a lot of focus on other studying and the exam period, so not much has been done,

### Sprint 4 (week 44 - 46)

This sprint included quite a lot of dead time to find new issue to work on. I hop my now looser schedule will mean that I can put in more time and energy to quickly solve an issue and get a PR merged.

I have started looking at an issue ([link](https://github.com/cypress-io/cypress/issues/23679)).

### Sprint 5 (week 47-48)

This sprint included a lot of work on the ealier mentioned [issue](https://github.com/cypress-io/cypress/issues/23679). The solution is not trivial and is related to how markdown handles lines beginning with spaces. Normally, markdown removes these but that is not always wanted. The used library seems to have no settings for these, making the solution harder. The found solution is to escape all rows with `&#32;`, the HTML entity for space. [Link to PR](https://github.com/cypress-io/cypress/pull/24687).

I also looked at a last issue to work on, and found this one: [link](https://github.com/cypress-io/cypress/issues/21730). I started working on it a bit, but did not reach a PR.

### Sprint 6 (week 49-50)

I opened a new PR for the issue I started looking on in sprint 5 ([link](https://github.com/cypress-io/cypress/pull/24996)).

The rest of the sprint consisted on trying to fix issues with tests and to get them over the line. I had not noticed them earlier due to flakiness of their tests, meaning I thought they were false positives. They are a bit hard to solve, especially for the markdown space fix. This is mostly due to the fix being quite "dirty".

What surprised me from the first PR is the much slower space the maintainers seem to have. Last time, things moved very quickly, now It's much less press and stress. 

