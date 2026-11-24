<div align="center">
  <img src="https://raw.githubusercontent.com/KaadzOS/.github/main/assets/kaadzoslogo.png" alt="KaadzOS" width="100%">
</div>

<p align="center">
  <sub>DECLARATIVE PACKS &nbsp;·&nbsp; KEY=VALUE &nbsp;·&nbsp; SIGNED ARCHIVE</sub>
</p>

<p align="center">
  <strong>Packs are promises, not payloads.</strong><br>
  Sixteen files. One CLI. Install only what you mean.
</p>

<p align="center">
  <a href="https://github.com/KaadzOS/KaadzOS/tree/main/packs">Pack definitions</a> &nbsp;·&nbsp;
  <a href="https://kaadzos.pages.dev/docs/">Manual</a> &nbsp;·&nbsp;
  <a href="https://iso.kaadzos.pages.dev/apt/">APT archive</a> &nbsp;·&nbsp;
  <a href="https://kaadzos.pages.dev">Website</a>
</p>

## Skeleton, on purpose

The canonical `key=value` pack files live in [`packs/`](https://github.com/KaadzOS/KaadzOS/tree/main/packs) in the main monorepo. That tree is published as the `kaadzos-pack-defs` package in the signed APT archive. This repository is the stable address for that package; it holds no competing copy.

| Piece | Where it actually lives |
| --- | --- |
| Pack files | [`packs/`](https://github.com/KaadzOS/KaadzOS/tree/main/packs) |
| Pack hooks | [`packs/hooks/`](https://github.com/KaadzOS/KaadzOS/tree/main/packs/hooks) |
| Pack manager | [`kaadzos`](https://github.com/KaadzOS/KaadzOS/blob/main/config/includes.chroot/usr/local/bin/kaadzos) |
| APT builder | [`ci/build-pack-defs.sh`](https://github.com/KaadzOS/KaadzOS/blob/main/ci/build-pack-defs.sh) |

## The shape of a pack

`name`, `description`, `size`, `requires`, `apt`, `repo-*`, `hook`. That is the whole language. No interpreter, no daemon, no surprise.

## Licence

MIT; see [`LICENSE`](LICENSE).

<sub>Debian is a registered trademark of Software in the Public Interest, Inc. KaadzOS is an independent project.</sub>
