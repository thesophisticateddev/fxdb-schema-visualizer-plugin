# FXDB Schema Visualizer Plugin

A plugin for [FXDB](https://github.com/thesophisticateddev/fxdb) that generates ER diagrams from your database connections. Visualize table relationships, primary keys, foreign keys, and column types in an interactive canvas.

## Features

- Auto-layout ER diagrams from any connected database
- Visual foreign key relationship lines between tables
- Color-coded columns (PK, FK, nullable)
- Drag-and-drop table positioning
- Export to PNG/SVG

## Installation

Download the latest JAR from [Releases](https://github.com/thesophisticateddev/fxdb-schema-visualizer-plugin/releases) and place it in `~/.fxdb/plugins/`, or install directly from the FXDB Plugin Manager.

## Building from Source

Requires [fxdb](https://github.com/thesophisticateddev/fxdb) installed locally for the `fxdb-db` dependency:

```bash
git clone https://github.com/thesophisticateddev/fxdb.git /tmp/fxdb
cd /tmp/fxdb
mvn install -pl fxdb-core,fxdb-db -am -DskipTests -q

cd /path/to/fxdb-schema-visualizer-plugin
mvn clean package
```

The plugin JAR will be in `target/fxdb-plugin-visualizer-1.0.0.jar`.

## Development

Built with the [FXDB Plugin SDK](https://github.com/thesophisticateddev/fxdb-plugin-sdk). See the SDK README for the full plugin development guide.

## License

MIT
