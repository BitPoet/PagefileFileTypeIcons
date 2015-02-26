# PagefileFileTypeIcons
[ProcessWire](http://processwire.com) module that adds file type icons to page files.

Adds a getFileIcon methods to Pagefiles that returns an URL to a 16x16 icon that matches the file's extension (or an empty page icon if none is found).

## Setup

Extract PagefileFileTypeIcons.module and the fileicons directoy into a new directory named "PagefileFileTypeIcons" under site/modules. Click "Modules" -> "Refresh" in the PW backend, then press the green button in the line for PagefileFileTypeIcons to install the module.

## Example Usage

```
foreach( $page->files AS $pagefile ) {
  echo "<li><img src='{$pagefile->getFileIcon()}'> {$pagefile->name}</li>";
}
```
