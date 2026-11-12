# documents

Document store for DevArts Lab. Private contents are git-crypt
ciphertext on GitHub; filenames remain visible, so keep them
non-sensitive.

Rendered at https://train.devartslab.com - private docs behind
Cloudflare Access, unmarked docs public.

## Visibility

Docs are public on the site by default. Opt a doc into the gated zone
with frontmatter:

```markdown
---
visibility: private
---
```

## Unlock

```bash
git-crypt unlock <key-path>/documents.git-crypt.key
```

Key lives in the workspace store: `config/projects/documents/secrets/`.
