# :warning: Repository Deprecation Notice :warning:

Dear users,

We want to inform you that this repository is now **deprecated** and will no longer be actively maintained.

## Action Replacement

This action should be substituted by the following actions provided by nullplatform:

- [Nullplatform Github Action Asset Build](https://github.com/nullplatform/github-action-asset-build)
- [Nullplatform Github Action Asset Push](https://github.com/nullplatform/github-action-asset-push)

Please consider transitioning to these actions to continue your workflow seamlessly.

If you have any questions or need further assistance with the transition, please feel free to reach out.

# Nullplatform Asset Build & Push Composite GitHub Action

You can use the GitHub Action to manage build assets workflow on Nullplatform.

## Change action.yml

The action.yml defines the inputs and output for your action.

Update the action.yml with your name, description, inputs and outputs for your action.

See the [documentation](https://help.github.com/en/articles/metadata-syntax-for-github-actions)

## Package for distribution

Update version in ``update-version.sh`` file changing ``VERSION_NUMBER`` and then run:

```bash
chmod 400 ./update-version.sh
```

```bash
./update-version.sh
```

## Usage

You can now consume the action by referencing the v1 branch

```yaml
uses: nullplatform/github-action-asset-build-push@v1
with:
  build-id: 123456
  application-path: .
  type: docker-image # docker-image, lambda, etc.
  name: main
```
