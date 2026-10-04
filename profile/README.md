## neuraldoc keeps product documentation in step with the code

When the code changes, neuraldoc finds the documents that become outdated and proposes evidence-backed text changes. Every proposal shows its source in the code. A person reviews and approves.

| Repository | Purpose |
| --- | --- |
| [neuraldoc-app](https://github.com/neuraldoc-ai/neuraldoc-app) | The app. Run it in Docker, explore the example or check a project of your own. |
| [mobiq](https://github.com/neuraldoc-ai/mobiq) | Our example and test dataset: a fictional ERP vendor with a release, tickets and outdated documentation. |
| [mobiq-code](https://github.com/neuraldoc-ai/mobiq-code) · [mobiq-docs](https://github.com/neuraldoc-ai/mobiq-docs) · [mobiq-db](https://github.com/neuraldoc-ai/mobiq-db) | Code, documentation and database of that dataset. |

### Try it

Requirements: [Git](https://git-scm.com/downloads) and [Docker](https://docs.docker.com/get-docker/).

```bash
git clone --recursive https://github.com/neuraldoc-ai/neuraldoc-app.git
cd neuraldoc-app
docker build -t neuraldoc .
docker run -p 8080:8080 -v neuraldoc-data:/data neuraldoc
```

Then open http://localhost:8080/app/. The example runs without keys and at no cost. A project of your own needs a Jev key and a language model of your choice, see the [README](https://github.com/neuraldoc-ai/neuraldoc-app#readme). The interface is in German.

All repositories are MIT-licensed. Companies, people and contents in the example are fictional.
