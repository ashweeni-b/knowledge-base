### Git Flow

- Uses several long-lived and temparory branches

| Branch | Use for |
| -------- | ------- |
| master | Always reflects production ready code |
| develop | Contains the latest development work for the next release |
| feature /* | Used to create new features; branched from develop and merged back when complete |
| release /* | Prepares a new production release from develop; allows final testing and minor bug fixes |
| hofix /* | Used to quickly patch production issues; branched from master |

#### How the Git Flow process work?

1. Developers create feature branches from develop to build new functionality
1. When its time for release, a release branch is created from develop. This isolates release preparation work so development can continue uninterrupted
1. Bug fixes can be added to the release branch, but major features should wait for a future release
1. Once ready, the release branch is merged into master and tagged with a version number. GitHub can use these tags to help you generate release notes
1. The same release branch should be merged back into develop to keep it in sync
1. If a critical production bug arises, a hotfix branch is created from master. Once fixed, it's merged into both master and develop

#### When to use Git Flow?

1. Best suited for projects with structured scheduled or versioned releases
1. Helpful if user maintains multiple production versions - e.g. long-term support branches
1. Ideal for slower, more structured development cycles - e.g. enterprise or regulated environments
1. Considered more heavy-weight than GitHub flow due to additional branch management

> _Note:_ Git Flow assumes merge commits for integrating branches. Using rebase or squash merges can interfere with its branch structure and history tracking

---