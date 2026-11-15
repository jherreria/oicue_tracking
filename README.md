# OICue

> Your sanity-saving companion for ORCLE® Integrations (OIC)

**OICue** turns opaque IAR/CAR files into clean, readable psudo-code YAML (or JSON) so you can actually understand what that integration is doing — without the usual stream-of-curse-word symphony or monitor-smashing meltdown.

Tired of reverse-engineering integrations left behind by “the other guy”?  
OICue helps you:
- Understand existing integrations faster than opening the OIC designer
- Speed up code reviews
- Find where variables are set or referenced
- See the all actions and its attributes; no more clicks to see one.

**Live web app → [oicue.vercel.app](https://oicue.vercel.app/)**

All processing happens in your browser. Your files never leave your machine.

---

## Features

- Multi-file support (drop several IAR/CAR at once)
- YAML or JSON output
- Schema handling: inline / catalog / sidecar / omit
- Preview, copy, individual download, or ZIP of everything


## Supported orchestration elements

`activityStreamLogger` · `assignment` · `callout` · `catch` · `catchAll` · `data stitch` · `ehStop` · `for` · `globalTry` · `globalVariable` · `integrationProperties` · `invoke` · `map` · `note` · `notification` · `parallel` · `parallelBranch` · `pick` · `pickReceive` · `publish` · `receive` · `reply` · `route` · `scheduleReceive` · `stageFile` · `stop` · `subscribe` · `switch` · `throw` · `try` · `wait` · `while`

*(Coverage based on real-world examples — let me know the missing ones.)*

## Limits (web app)

- Up to 20 archives / 50 MiB total per batch
- Up to 500 generated files / 50 MiB of YAML
- Nested IAR/CAR supported up to 3 levels
- Trial valid through **January 31, 2027**

## Trial & Support

This project is under a trial license until **January 31, 2027**.  
See [LICENSE](LICENSE).

For licensing or support, contact [Jorge Herreria](https://www.linkedin.com/in/jherreria/).

---

© 2026 Jorge Herreria
