Gnome Private Path Thumbnailer
------------------------------

This simple thumbnailer allows for selecting paths that do not show thumbnails or store them in the cache. Useful for senstive areas where you would not want thumbs leaking image information by mistake.

It works by checking the path against a configured list and when the request matches it sets the default thumb. If no match then it fails and the generic thumbnailer continues to the next available thumbnailer as usual.

The extra options are store in the same file as the usual thumbnailer config as a new section:

[PrivateThumbs]

Dirs=paths separated by semi-colons, default is /tmp/ (which apparently has no effect)

Thumb= path to substitute png (by default a dummy 1 pixel image provided by privatethumbs.png)

If the thumb path has no "/" then it is considered local to the thumbnailer config file.




