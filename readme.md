# netlify-ddns

A stupid-simple, "fake dynamic DNS" script that integrates with Netlify via
their [provided API][netlify-api].

## Dependencies

+ bash
+ curl
+ jq

## Basic Usage

Just run `make` to configure (if your first time) and run.

If you want this to run recurring every 5 minutes, setup a systemd timer for the
current user with `make install-user-timer`. You can revert this by running
`make uninstall-user-timer`.

## Related
- [lukehsiao/netlify-ddns-rs] for a similar client written in [Rust][rust].
- [oscartbeaumont/netlify-dynamic-dns] for a similar client written in [Go][go].
- [skylerwlewis/netlify-ddns] for another similar shell script version.

[netlify-api]: https://open-api.netlify.com
[rust]: https://rust-lang.org/
[go]: https://golang.org/
[skylerwlewis/netlify-ddns]: https://github.com/skylerwlewis/netlify-ddns
[lukehsiao/netlify-ddns-rs]: https://github.com/lukehsiao/netlify-ddns-rs
[oscartbeaumont/netlify-dynamic-dns]: https://github.com/oscartbeaumont/netlify-dynamic-dns
