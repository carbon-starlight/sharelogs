# View &amp; share system logs online

Sharing your system logs online may be annoying: you either upload a bunch of screenshots or pipe them to a text file using complex terminal commands (coloring and metadata not preserved). This tool aims to make uploading logs without loosing highlighting and metadata as easy as possible for any non-tech savvy user.

> [!WARNING]
> This tool is in public alpha phase. Don't expect generated URLs to be compatible with future versions.

Try it online: https://raw.githack.com/carbon-starlight/sharelogs/main/journalview.html | short link: https://tinyurl.com/y874d745


## TODO: 
* I'm working on a switch to a better compressing algorithm called Kanzi: it will make permanent URLs 30-50% smaller than the one currenly utilized.
  - I actually need help with figuring out how to run the `kanzi.wasm` compressor from client-side JS: in particular, I can't figure out a way to pass files/byte arrays to it. If you know your way around wasm, your contribution is welcome.
* Seveal visual themes, including 70s retro and Y2K.
* More logging systems supported: not only UNIX's syslog, but Windows as well.
* Pick charset for compressed data encoding that does not break most non-standard, yet common highlighting engines.
* More options for forum administrators: more ability to set sharing properties in URL parameters.
* Server for getting temporal short URLs, termbin style.
* Ability to password-protect contents of a short URL?
