# bb-file-management-preview

**Unofficial preview.** This repository publishes a GitHub Pages rendering of the
GovStack File Management Building Block specification for review purposes only.
It is not an official GovStack publication; the authoritative specifications live
at <https://specs.govstack.global/>.

- Content: [GovStackWorkingGroup/bb-file-management](https://github.com/GovStackWorkingGroup/bb-file-management),
  branch `v0.4-conformance-profiles`
- Renderer: [jeremi/govstack-specification-site](https://github.com/jeremi/govstack-specification-site),
  pinned to `567eb981cd0c2a1bb9163b2cecbfc12a1b7412fd`, profile `framework`
- Preview: <https://nicolk.github.io/bb-file-management-preview/>

The [workflow](.github/workflows/pages.yml) rebuilds on every push to `main`, on
manual dispatch, and daily so new content commits are picked up. Every page
carries an "Unofficial preview" banner and is marked `noindex, nofollow`.

Known workaround: functionality `contract:` values holding a `govstack:spec:bb:*`
URN are blanked in the build checkout, because the pinned renderer treats
`contract:` as a local file path.
