# OICue

**OICue** is your sanity-saving companion for Oracle® Integrations (OIC) developers. Tired of deciphering integrations left behind by that "other guy"? OICue prevents stream-of-curse-word symphonies during integrations maintenance and monitor-smashing meltdowns. It parses the IAR/CAR and spits out clean OICue pseudo-code representation in a YAML (or JSON) file to turbocharge your understanding of existing integrations, speed up code reviews, find where that variable is being updated/referenced, etc; all these faster than any Formula 1 car.


**Web app:** [oicue.vercel.app](https://oicue.vercel.app/).

OICue 
## Actions coverage

Parsers orchestration element types. 
- `activityStreamLogger`
- `assignment`
- `callout`
- `catch`
- `catchAll`
- `data stitch`
- `ehStop`
- `for`
- `globalTry`
- `globalVariable`
- `integrationProperties`
- `invoke`
- `map`
- `note`
- `notification`
- `parallel`
- `parallelBranch`
- `pick`
- `pickReceive`
- `publish`
- `receive`
- `reply`
- `route`
- `scheduleReceive`
- `stageFile`
- `stop`
- `subscribe`
- `switch`
- `throw`
- `try`
- `wait`
- `while`


## Web app

The browser interface supports multiple IAR/CAR files, YAML previews, copy, individual downloads, and a ZIP containing all results. Use the Schema output dropdown to choose inline, catalog (default), sidecar, or omit. Sidecar catalogs are included as separate `.schemas.yaml` files in the results and ZIP. Errors and incomplete-reference warnings are displayed alongside the affected integration.

All parsing is processed in your browser. IARs/CARs stay on your device and are never uploaded.


### Limits

- Up to 20 selected archives, totaling less than 50 MiB per batch.
- Up to 500 generated files and 50 MiB of generated YAML per batch.
- Each archive is limited to 50,000 ZIP entries, 512 MiB of declared expanded data, and 64 MiB per entry, including nested archives.
- Nested IAR/CAR files are supported through three nested levels. Symlinks, traversal paths, and duplicate ZIP paths are rejected.
- The existing trial expires January 31, 2027. The same trial check applies to CLI, server, and browser conversion.

Coverage is based on the supplied examples, not every possible Oracle® action or export variant. Mappings follow the existing compact representation: closing XML tags are omitted and indentation conveys hierarchy.



## Trial and support

This project uses the existing trial license, functional through **January 31, 2027**. See [LICENSE](LICENSE). Contact [Jorge Herreria](https://www.linkedin.com/in/jherreria/) for licensing and support.

© 2026 Jorge Herreria
