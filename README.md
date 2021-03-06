# ptpimg-uploader

Upload image file or image URL to the ptpimg.me image hosting.

## Installation

1. Install python3 package requests (usually apt-get install python3-requests or pip3 install requests).

2. Optionally: export your ptpimg.me API key (usually in .bashrc or .zshenv):

    export PTPIMG_API_KEY=<your hex key>

  or use the -k / --api-key command-line switch.

## How to use:

To upload an image file:

    python3 ptpimg-uploader.py ~/seed/mytorrent/folder.jpg

To rehost an imgur image:

    python3 ptpimg-uploader.py https://i.imgur.com/eaT6j3X.jpg

An uploaded URL will be printed to the console.

If pyperclip python package is installed, the URL will be additionally copied to the clipboard.

You can specify multiple files and URLs on the command line:

    python3 ptpimg-uploader.py ~/seed/mytorrent/folder.jpg https://i.imgur.com/eaT6j3X.jpg

The resulting URLs are printed each on separate line, and copied to your
clipboard with newlines in between.
