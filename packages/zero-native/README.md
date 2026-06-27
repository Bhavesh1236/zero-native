# zero-native

CLI tools for [zero-native](https://zero-native.dev), a Zig native app framework with secure WebView surfaces, native controls, and OS capabilities.

## Install

```bash
npm install -g zero-native
```

## Usage

```bash
zero-native init my_app --frontend vite
cd my_app
zig build run
```

The first run installs the generated frontend dependencies automatically.

Use WebViews for rich product UI, and add native windows, menus, shortcuts, views, dialogs, clipboard, credentials, and OS services where the platform should own the interaction.

## Commands

| Command | Description |
|---------|-------------|
| `zero-native init [name] --frontend <next\|vite\|react\|svelte\|vue>` | Scaffold a new zero-native project |
| `zero-native dev --binary <path>` | Start the app with a managed frontend dev server |
| `zero-native doctor` | Check host environment, WebView, manifest, and CEF |
| `zero-native validate` | Validate `app.zon` against the manifest schema |
| `zero-native package` | Package the app for distribution |
| `zero-native bundle-assets` | Copy frontend assets into the build output |
| `zero-native automate` | Interact with a running app's automation server |
| `zero-native skills list` | List built-in AI agent skills |
| `zero-native skills get <name>` | Output AI agent skill content |
| `zero-native version` | Print the zero-native version |

## More

See the [full documentation](https://zero-native.dev) for details on the app model, native controls, capabilities, bridge, security, and packaging.
