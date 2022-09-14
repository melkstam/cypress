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

Lastly, Cypress has what seems like an active Discord where users and developers can interact with each other. The team at Cypress seem to be very welcoming and nice to everyone. 

| Process difficulty | Issue tracker                                    | Documentation                                                              | Communications                                              |
|--------------------|--------------------------------------------------|----------------------------------------------------------------------------|-------------------------------------------------------------|
| **Easy**           | Contains issues tagged as suitable for beginners | Contains guides and tutorials for new developers                           | Contains specific communication channels for new developers |
| **Medium**         | Contains issues marked with difficulty           | **Contains introduction chapters and suggested readings in documentation** | **Contains open communication channels**                    |
| **Hard**           | **No metadata on difficulty in issue tracker**   | No clear introduction to new developers                                    | Restricted communication channels                           |

## Development process

While Cypress is open source, it is still a for-profit company behind it. I think this can make contributing a bit harder as I, on some level, will "compete" with people being paid to contribute to the project. This also means that they have bigger resources to create good processes and tools to use, meaning I think it can be hard for me to reach what is here considered "Hard". I do however aim to do serious contributions and to help out. I do think I have some qualities and experience from work and earlier hobby projects which could come handy.

| Development process | Group contributions                                                                                                  | Planning and reflection                                                                                                                                             | Engineering practice                                                                                                      |
|---------------------|----------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| **Easy**            | Shares code, tutorials and development tips to other members of the team. Actively participates in project meetings. | Creates a plan for each sprint with sufficient details to guide the work, amounting to a number of hours that correspond the amount of credits given by the course. | Uses the required set of tools and suggested practices for code contributions in the host project                         |
| **Medium**          | **Shares documentation and material, and also gives valuable feedback on others' contributions**                     | **Uses the plan actively and updates the plan to take into account new information and events**                                                                     | **Takes care to follow established good practices in continuous development and testing**                                 |
| **Hard**            | Actively helps team members improve, and provides tutorials or other help to team members                            | Uses external sources from the host project to validate the feasibility of the plan and to update accordingly                                                       | Contributes with general quality improvements for the process of developing, building and testing software in the project |

## Contributions

TO BE ADDED

