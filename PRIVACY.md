# ChatAssistantX Privacy Policy

Effective date: September 12, 2026

ChatAssistantX is provided by **Developing Future & Solutions** ("we", "us"). This
policy explains what the plugin processes, where information is stored, and when data is
sent to third parties.

## Data processed by the plugin

Depending on the features you use, ChatAssistantX may process:

- Prompts and chat messages you submit.
- Source code, file contents, paths, editor selections, open-file metadata, images, and
  other context you explicitly attach or authorize the plugin to read.
- Commands, patches, tool arguments, approval decisions, model choices, and operational
  status needed to perform a request.
- Codex account and rate-limit information returned by the locally installed Codex App
  Server when that integration is used.
- Configuration such as provider, model, API base URL, excluded paths, and interaction or
  approval mode.

The plugin does not add advertising or independent analytics and does not intentionally
collect telemetry for the vendor.

## Local storage

Conversation data and related artifacts are stored on your device under
`~/.chatassistantx`, separated by session UUID. This can include messages, plans, context
manifests, images, approval metadata, and agent definitions. The plugin creates this
storage directly on first initialization and preserves data already present there. Project
and application preferences may also be stored by the JetBrains Platform.

OpenAI API keys are stored using the JetBrains PasswordSafe. Codex CLI authentication is
managed by Codex CLI and is not copied into the conversation history. The plugin is
designed not to persist complete credentials, access tokens, or private keys in session
files or traces.

## Data sent to providers

When you submit a request, the plugin sends the prompt and the context required for that
request to the provider you selected:

- Codex CLI / Codex App Server installed on your computer; or
- OpenAI Responses API, or another OpenAI-compatible base URL that you configure.

Provider processing is governed by the provider's own terms and privacy policy. If you
configure a custom endpoint, you are responsible for evaluating its operator and data
practices. Web search and other network-backed tools are used only when enabled and
available for the selected mode and provider.

## Approvals and sensitive content

Approval modes control whether available operations require confirmation. `Trust project`
can allow operations and data access without a separate prompt, including outside the
project, as explained by the warning shown before it is enabled. You should select an
approval mode appropriate for the sensitivity of your project.

Excluded-path and sensitive-file protections reduce unintended access but cannot replace
your own access controls or review. Do not submit content that you are not authorized to
process.

## Retention and deletion

Local data remains until you delete the related session or remove the files. Deleting a
session in the plugin may move it to `~/.chatassistantx/trash` so that it can be recovered
manually. You can permanently delete that directory using your operating-system tools.
Provider retention is controlled by the provider and your account settings.

## Security

The plugin uses platform facilities such as PasswordSafe, path validation, sandbox and
approval settings where available. No software or transmission method is completely
secure. Keep the IDE, plugin, Codex CLI, and operating system updated and protect access to
your user account and filesystem.

## Children's privacy

ChatAssistantX is a developer tool and is not directed to children. Do not use it if you
cannot lawfully consent to the processing described here.

## Changes

This policy may be updated when the plugin's processing changes. Material changes will be
described in release notes or the Marketplace listing, and the effective date above will
be updated.

## Contact

For privacy questions or requests, contact:

- **Developing Future & Solutions**
- Email: vtsppinho@gmail.com
- Website: https://github.com/vtspp
