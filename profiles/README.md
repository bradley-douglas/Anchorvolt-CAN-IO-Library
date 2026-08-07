# Protected vehicle profiles

`catalog.json` contains harmless selection metadata used by the Android app.
`packages/` contains authenticated AES-256-GCM `.avp` files created by the
private Anchorvolt publishing tool.

The catalog starts empty because the development repository currently has no
real learned and approved vehicle profile. Placeholder CAN mappings must never
be released as installable profiles.
