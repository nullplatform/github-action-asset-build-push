# Nullplatform Asset Build & Push Composite GitHub Action

<p align="center">
  <a href="https://github.com/nullplatform/github-action-asset-build-push/actions"><img alt="javscript-action status" src="https://github.com/nullplatform/github-action-asset-build-push/workflows/units-test/badge.svg"></a>
</p>

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
  name: ${{ secrets.NULLPLATFORM_API_KEY }}
  type: docker-image
```

See the [actions tab](https://github.com/actions/javascript-action/actions) for runs of this action! :rocket:
