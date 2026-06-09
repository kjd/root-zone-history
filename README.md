# DNS Root Zone History

This is a corpus of published versions of the [DNS root
zone](https://www.iana.org/domains/root). Each commit is produced with a date
derived from the zone serial number, correlating to the date of publication.
i.e.  `YYYYMMDDSS` → `YYYY-MM-DD HH:00:00 UTC`.

## Layout

Each commit's tree contains:

- `root.zone` — the canonical zone at that point in time. Use
  `git log -p root.zone` to walk zone-to-zone diffs.
- `archive/YYYY/root.YYYYMMDDSS.zone` — a frozen per-serial copy,
  never modified after it lands.

## Completeness

This represents the collection of root zone files that IANA has
processed through its automation systems, which began approximately
2008. They have been augmented with additional sources from dates prior,
but it not a complete collection of all published root zones. Be mindful
in any processing that the history becomes sparse as the data becomes
older.

## License

The root zone is in the public domain.

## Contact

IANA Root Zone Management <root-mgmt@iana.org>
