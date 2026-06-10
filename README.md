# Scanaislop Mintlify Docs

Source for the public documentation site at `docs.scanaislop.com`.

The docs use Mintlify with `docs.json` navigation and MDX pages. Product behavior should be checked against the `scanaislop/aislop` CLI source before changing command, flag, scoring, or CI examples.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview documentation changes locally:

```
npm i -g mint
```

Run the following command at the root of your documentation, where your `docs.json` is located:

```
mint dev
```

View your local preview at `http://localhost:3000`.

## Publishing changes

Changes are deployed by the connected Mintlify GitHub app after they merge to the default branch.

## Troubleshooting

- If your dev environment isn't running: Run `mint update` to ensure you have the most recent version of the CLI.
- If a page loads as a 404: Make sure you are running in a folder with a valid `docs.json`.

- [Mintlify documentation](https://mintlify.com/docs)
