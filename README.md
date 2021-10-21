# Git Workshop

## Perfect Commit I.

1. Add the *right* changes.
2. Compose a *good* commit message.

>Golden rule of perfect commit **Only compine changes from the same topic**.

#### View the changes in a fiile

```git
git diff <fileName>
```

#### Deside patch level.

```git
git add -p <fileName>
```

## Perfect Commit II.

1. Subject = concise summary of what happened
2. Body = more detailed explination.
    - What is now diffrent than before?
    - What is the reason for the changes?
    - Is there anything to watch out for / anything particularly remarkable?

## Branching Strategies

### A Written convention
#### Agree on a Branching workflow in your team

1. Git allows you to creatr branches - but it doesn't tell you how to use them!
2. You need a written best practice of how work is ideally structured in your team - to avoid mistakes & collisions.
3. It highly depends on your team / team size, on your project, and how you handle releases.
4. It help you to on board new team members.

### Integrating Changes & Structuring Releses.

1. Mainline Development ("Always be integrating")
2. State,Release, and Feature Branches

#### Mainline Development

- Few branches 
- relatively small commits
- high-quality testing and QA standards

#### State,Release, and Feature Branches

- Diffrent types of branches
- ... fullfill diffrent types of jobs

**2 types of Branches**
1. Long-running
2. Short-Lived

#### Long-running Branches
- exist through complate lifetime of the project.
- often, they mirror "stages" in your dev life cycle
- common convention: no direct commits!

#### Short-Lived Branches

- for few features, bug fixes, refactorings,experiments...
- will be deleted after integration (merge/rebase)

>Example of Branching strategies.
>1. github flow
>2. gitflow

```git
git branch <branchName>
git checkout test
```
*make some changes*
```git
git status
git add <fileName>
git commit -m "message"
git push --set-upstream origin <branchName>
```

```git
git commit -m"Title" -m"Description........."
```













