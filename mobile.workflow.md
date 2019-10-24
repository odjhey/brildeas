# A highly opinionated guideline of writing mobile apps (RN/MST/GQL)

# Cycle
1. Pitch
1. Shape
1. Bet
1. Build

# MVP
Always start with an MVP = 1-4 User stories

# Mobile Workflow

## MAIN LOOP (SPRINT)
---
#### MUST be achievable within 3days, max 2weeks
  1. Create your User Stories  
  **TEMPLATE**  
  As a __persona__, i should be able to __direct app action__, to __real world reason__.  
      1. Write a Gherkin/Cucumber scenario
      1. Create git issue for repo/status tracking purposes
      1. Add prelim tests based from Gherkin
  1. Start FE/BE cycle
  1. Can Story be merged to an EPIC? do so.
  1. Repeat

## FE/BE Cycle
---
### Frontend
1. Wireframe  
    1. wireframe.pptx
1. Components  
    1. composable md
    1. compound/composite.md
1. Storybook
    1. docs/composable.md
    1. docs/composites.md
    1. storybook/stories/*.story.tsx
    1. docs/screens.md
    1. storybook/stories/*.screen.story.tsx

### Backend
1. backend  
    1. mongo
        1. models/
    1. gql
        1. graphql/
    1. business logic
        1. modules/core
    1. business logic
        1. modules/plugins

### After 
1. mst-gql
    1. src/models/
1. screens + data
    1. app/screens/
1. data tests
    1. `__tests__/screens/` #TODO for polishing
1. navigation

## Preemptive activities (Scheduled)
1. TODO: divide by start and end of week
1. count completed git issues for the week
1. check milestone end dates
1. review user stories
1. cross off backlogs
1. update backlogs
1. remove stale/cancelled backlogs
1. add backlogs

# Git
## Morning Activities
1. Check PRs  
    1. check against standards
1. Comment/Review PR
1. Merge mergables
1. Pull nightly changes
1. Check changes
1. Review changes
1. Comment on issues
1. Update your backlogs
1. Update/Close your issues
1. Pick a task
1. Commit often please
## EOD Activities
1. PR completed backlogs
1. Update your backlogs
1. Update/Close your issues
1. 
## Commit
## PR conditions
## Issue templates
## Update Projects
## Git Structure
## Branches

#TODOs
1. add naming conventions
    1. file naming
        1. storybook
        1. components
        1. tests
    1. variable/props/interfaces etc naming
    1. git
        1. commits
        1. prs
        1. issues
        1. branch
1. add eslint and prettier setup
1. add babel and tsc setup
1. add circle ci config
1. containerize
1. update gitignores
1. maintain boilerplates
1. props/types/schema required or not
1. please use component composing, for observers, so we can observerized all components haha
    1. by eg. using props.children in all composite components
1. create a whole section about testing


1. how to modularize business logic (https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
1. break into apis/nodemodules
1. business logic should not be DB dependent
