# waitused

Run a command waiting until it or one of its subprocessed have opened and closed a given file.

This works around situations like mutt deleting the temporary attachment file
after `run-mailcap` is run, while `run-mailcap` runs a program that backgrounds
before opening its input file.

## Example:

```
waitused file.pdf xdg-open file.pdf
waitused file.pdf run-mailcap file.pdf
```

## License

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
