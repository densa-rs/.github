<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/densa-rs/densa/main/docs/brand/densa-logo-dark.svg">
    <img alt="densa" src="https://raw.githubusercontent.com/densa-rs/densa/main/docs/brand/densa-logo.svg" width="260">
  </picture>
</p>

<p align="center"><b>Dense by design.</b></p>

densa is a Rust toolkit for applications that show a lot of live data: trading terminals,
monitoring consoles, operational dashboards, developer tools. It keeps live data in order as
it changes, and draws it on the GPU at the display's refresh rate, from the data stream to the
pixel.

| Repository | What it is |
|---|---|
| [densa](https://github.com/densa-rs/densa) | The toolkit: live Arrow tables with incrementally maintained views, GPU rendering, widgets (a data grid, charts, docking, menus), real text and editing, wait-free data hand-off |
| [densa-connectors](https://github.com/densa-rs/densa-connectors) | Data sources as Arrow batches: CSV and Parquet files, WebSocket streams, Arrow Flight, SQL with DataFusion |
| [densa-studio](https://github.com/densa-rs/densa-studio) | The flagship application: open files and explore them at once, in grids and with SQL |

- Website and roadmap: [densa.dev](https://densa.dev) · [roadmap](https://densa.dev/roadmap/)
- Contributing: [CONTRIBUTING.md](https://github.com/densa-rs/.github/blob/main/CONTRIBUTING.md)
- License: MIT or Apache-2.0
