# BRANDING.md: Atelier Vector (based on VectorCraft)

This branch (`academy`) is VectorCraft by the ArtCraft team with **rebranding** and one small
change made by The Agent Factory for Claude Academy: in the browser build, the interface language follows
`?lang=xx` in the page address (set by the Claude Academy tools page), then the browser's preferred
languages (upstream always shows English on the web). Where the app has no French catalog we add
one (`rebrand/apps/<app>/fr.tsv` in the deploy repo). No format or engine code is changed.

| | |
|---|---|
| Upstream | https://github.com/storytold/vectorcraft (tag in `UPSTREAM_TAG` of the deploy repo's versions.env) |
| Licence | MIT OR Apache-2.0, unchanged (`LICENSE-MIT`, `LICENSE-APACHE`, `NOTICE`) |
| Name shown in the app | Atelier Vector (French: Atelier Vecteur) |
| Credit line | "Based on VectorCraft by the ArtCraft team (github.com/storytold/vectorcraft)." |
| Not affiliated | with the ArtCraft team, Adobe or Microsoft |

Why: `docs/brand/LICENSE-brand.txt` of the original says a modified version must remove the
ArtCraft name and marks and must not present itself as an ArtCraft product, while plain-text
credit is allowed. The product name VectorCraft is not covered by that license; we still
show our own name in the title, About box and start screen so nobody thinks the ArtCraft team
runs this copy. Crate names, binaries and file extensions are unchanged.

Every change is made by `rebrand/rebrand.py vectorcraft` in the deploy repo (rules in
`rebrand/apps/vectorcraft.toml`); each changed file starts with a one-line change notice.
In-app links: community -> https://www.skool.com/claudeacademy, website -> https://claudeacademy.ca.

## Files changed by `rebrand.py`

- `apps/vectorcraft-web/index.html`
- `apps/vectorcraft-web/src/web.rs`
- `crates/engine/src/cmd/help.rs`
- `crates/ui-egui/src/community.rs`
- `crates/ui-egui/src/dialogs/about.rs`
- `crates/ui-egui/src/i18n/cs.tsv`
- `crates/ui-egui/src/i18n/es.tsv`
- `crates/ui-egui/src/i18n/fr.tsv`
- `crates/ui-egui/src/i18n/it.tsv`
- `crates/ui-egui/src/i18n/ja.tsv`
- `crates/ui-egui/src/i18n/pt-br.tsv`
- `crates/ui-egui/src/i18n/ru.tsv`
- `crates/ui-egui/src/i18n/uk.tsv`
- `crates/ui-egui/src/i18n/zh-hans.tsv`
- `crates/ui-egui/src/i18n/zh-hant.tsv`
- `crates/ui-egui/src/menus.rs`
- `crates/ui-egui/src/native_menu.rs`
- `crates/ui-egui/src/tests_nativemenu.rs`

## Removed (ArtCraft marks, not licensed to forks)

- `docs/brand`
