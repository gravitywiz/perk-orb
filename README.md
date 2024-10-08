# Perk Orb for CircleCI

### Important note

If you're unable to publish, try running the following:

```bash
circleci orb pack ./src | circleci orb publish - gravitywiz/perk@dev:alpha
```

### [➡️ Orb on CircleCI](https://circleci.com/developer/orbs/orb/gravitywiz/perk) (requires login)

An orb that contains various commands, executors, and examples for testing perks using CircleCI.

Additional READMEs are available in each directory.

## Resources

* [CircleCI Orb Registry Page](https://circleci.com/orbs/registry/orb/gravitywiz/perk-orb) - The official registry page of this orb for all versions, executors, commands, and jobs described.
* [CircleCI Orb Docs](https://circleci.com/docs/2.0/orb-intro/#section=configuration) - Docs for using and creating CircleCI Orbs.

### How to Publish
* Create and push a branch with your new features.
* When ready to publish a new production version, create a Pull Request from _feature branch_ to `master`.
* The title of the pull request must contain a special semver tag: `[semver:<segment>]` where `<segment>` is replaced by one of the following values.


| Increment | Description|
| ----------| -----------|
| major     | Issue a 1.0.0 incremented release|
| minor     | Issue a x.1.0 incremented release|
| patch     | Issue a x.x.1 incremented release|
| skip      | Do not issue a release|

Example: `[semver:major]`

* Squash and merge. Ensure the semver tag is preserved and entered as a part of the commit message.
* On merge, after manual approval, the orb will automatically be published to the Orb Registry.
