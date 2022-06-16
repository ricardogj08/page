# page

A simple password manager using `age` written in POSIX `sh`.

> A pash gpg fork to age.

## Dependencies

* sh, bash, zsh or other shell like UNIX.
* GNU Coreutils, BusyBox, Toybox, sbase or other UNIX utilities.
* [age >= 1.0.0 - a simple, modern and secure file encryption tool, format, and Go library.](https://github.com/FiloSottile/age)
* [wayclip (optional) -  Wayland clipboard utility.](https://github.com/noocsharp/wayclip)

## Installation

    git clone https://github.com/ricardogj08/page.git
    cd page
    sudo cp page /usr/local/bin

## Usage

Show help message:

    page

First, generate a master encryption key:

    page -g

Save a password:

    page -a foo@example.com

Or save a password with category:

    page -a email/foo@example.com

Show a password:

    page -s foo@example.com

Or show a password with category:

    page -s email/foo@example.com

List all passwords:

    page -l

Copy a password to the clipboard:

    page -c foo@example.com

Or copy a password with category to the clipboard:

    page -c email/foo@example.com

Delete a password:

    page -d foo@example.com

Or delete a password with category:

    page -d email/foo@example.com

## References

* [A simple password manager using GPG written in POSIX sh.](https://github.com/dylanaraps/pash)
* [A collection of pure POSIX sh alternatives to external processes.](https://github.com/dylanaraps/pure-sh-bible)
* [POSIX.1-2017](https://pubs.opengroup.org/onlinepubs/9699919799/utilities/contents.html)
* [XDG Base Directory Specification.](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
* [Manual de Referencia de Bash, para Bash, Version 5.1](https://freakspot.net/programas/docs/bash/manual-de-referencia-de-Bash_5.1.html)
* [Advanced Bash-Scripting Guide.](https://tldp.org/LDP/abs/html/)
* [Korn shell.](https://www.ibm.com/docs/en/aix/7.3?topic=shells-korn-shell)
* [When using <<-, you can only indent with tabs.](https://github.com/koalaman/shellcheck/wiki/SC1040)

## License

    page - A simple password manager using age written in POSIX sh.

    Copyright (C) 2020-2022 - Dylan Araps <dylan.araps@gmail.com>,
                              Ricardo García Jiménez <ricardogj08@riseup.net>

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this software except in compliance with the License.
    You may obtain a copy of the License at:

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
