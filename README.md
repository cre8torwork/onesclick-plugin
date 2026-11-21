# OnesClick for Claude

Ask Claude to work with the OnesClick marketing team. In Claude Code and Cowork, the CMO delegates to teammate agents in separate sessions. In Claude chat, the CMO skill and connector give you the same workflow in one conversation.

## Install in Claude Code

Run these commands in a Claude Code session to add the marketplace and install the plugin.

```text
/plugin marketplace add cre8torwork/onesclick-plugin
/plugin install onesclick@onesclick
```

If you have a local OnesClick checkout, you can load the plugin for a single session. Run this from the checkout root.

```sh
claude --plugin-dir ./plugin/onesclick
```

On first use, follow the OnesClick OAuth prompt and sign in in your browser. In Claude Code, use `/mcp` to check the connection and start sign-in if prompted.

## Connect manually

If the plugin connection cannot start sign-in, add a custom connector named **OnesClick** using the URL in the command below. In Claude Code, run:

```sh
claude mcp add --transport http onesclick https://mcp.ones-click.com/mcp
```

Then open `/mcp` to authenticate. The manual connector supports the in-thread CMO workflow. In Claude Code, the plugin agents use the connector supplied by the plugin.

## Work with the team

Give the CMO your marketing goal. The CMO reports back with the result and any approvals waiting for you. Open the OnesClick app to confirm required approvals.
