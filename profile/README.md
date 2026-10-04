## neuraldoc keeps product documentation in step with the code

When the code changes, neuraldoc finds the documents that become outdated and proposes evidence-backed text changes. Every proposal shows its source in the code. A person reviews and approves.

| Repository | Purpose |
| --- | --- |
| [neuraldoc-dashboard](https://github.com/neuraldoc-ai/neuraldoc-dashboard) | The tool. Run it locally, explore the example or check a project of your own. |
| [mobiq](https://github.com/neuraldoc-ai/mobiq) | Our example and test dataset: a fictional ERP vendor with a release, tickets and outdated documentation. |
| [mobiq-code](https://github.com/neuraldoc-ai/mobiq-code) · [mobiq-docs](https://github.com/neuraldoc-ai/mobiq-docs) · [mobiq-db](https://github.com/neuraldoc-ai/mobiq-db) | Code, documentation and database of that dataset. |

### Try it

Requirements: [Node.js 24](https://nodejs.org) and Git.

```bash
git -c core.autocrlf=false clone --recursive https://github.com/neuraldoc-ai/neuraldoc-dashboard.git
cd neuraldoc-dashboard/frontend
npm ci
npm run dev
```

Then open http://localhost:5174/app/. The example runs without keys and at no cost. A project of your own needs a Jev key and a language model of your choice, see the [README](https://github.com/neuraldoc-ai/neuraldoc-dashboard#readme). The interface is in German.

All repositories are MIT-licensed. Companies, people and contents in the example are fictional.
