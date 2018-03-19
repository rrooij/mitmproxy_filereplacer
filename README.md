# mitmproxy_filereplacer

mitmproxy_filereplacer is a simple script for mitmproxy that can change a specific URL with a file.

This is made because it is pretty easy to replace pieces of text with mitmproxy, but not whole files.

## Configuration

Files should be defined in the script folder in `files.txt`.

The syntax is the following:

```
http://example.org/|replacement_file.txt
```

`|` is the seperator between the URL and file.

## Running

Clone this script, install [mitmproxy] and run:

```
mitmproxy --anticache -s filereplacer.py
```

