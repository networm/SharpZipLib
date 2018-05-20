# SharpZipLib

This is a modified version just for Unity .NET 2.0. Newer version has used C# 6.0 which not supported by C# 3.0 in .NET 2.0.

As 2018/05/20 the latest version [Release 0.86.0.518 · icsharpcode/SharpZipLib](https://github.com/icsharpcode/SharpZipLib/releases/tag/0.86.0.518) didn't work with newer zip version files.

It will throw an ZipException:

```
ZipException: Version required to extract this entry not supported (778)
```

sharpziplib-unity/20180520 has been tested on

1. Unity 2017.4.2f2
2. IL2CPP on Android

Recommend copy folder `src/ICSharpCode.SharpZipLib` to Unity project.

------------

The SharpZipLib project is looking for a new maintainer - please read [State of the Union August 2017](https://github.com/icsharpcode/SharpZipLib/issues/187)

Introduction
------------

SharpZipLib (\#ziplib, formerly NZipLib) is a compression library that supports Zip files using both stored and deflate compression methods, PKZIP 2.0 style and AES encryption, tar with GNU long filename extensions, GZip, zlib and raw deflate, as well as BZip2. Zip64 is supported while Deflate64 is not yet supported. It is implemented as an assembly (installable in the GAC), and thus can easily be incorporated into other projects (in any .NET language). The creator of SharpZipLib put it this way: "I've ported the zip library over to C\# because I needed gzip/zip compression and I didn't want to use libzip.dll or something like this. I want all in pure C\#."

SharpZipLib was originally ported from the [GNU Classpath](http://www.gnu.org/software/classpath/) java.util.zip library for use with [SharpDevelop](http://www.icsharpcode.net/OpenSource/SD), which needed gzip/zip compression. bzip2 compression and tar archiving were added later due to popular demand.

The [SharpZipLib homepage](http://icsharpcode.github.io/SharpZipLib/) has precompiled libraries available for download, [a link to the forum for support](http://community.sharpdevelop.net/forums/12/ShowForum.aspx), [release history](https://github.com/icsharpcode/SharpZipLib/wiki/Release-History), samples and more.

License
-------

This software is now released under the [MIT License](https://opensource.org/licenses/MIT). Please see [issue #103](https://github.com/icsharpcode/SharpZipLib/issues/103) for more information on the relicensing effort.

Previous versions were released under the [GNU General Public License, version 2](http://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html) with an [exception](http://www.gnu.org/software/classpath/license.html) which allowed linking with non-GPL programs.

Namespace layout
----------------

| Module | Namespace |
|:----------------:|:-----------------------------|
|BZip2 implementation|ICSharpCode.SharpZipLib.BZip2.\*|
|Checksum implementation|ICSharpCode.SharpZipLib.Checksums.\*|
|Core utilities / interfaces|ICSharpCode.SharpZipLib.Core.\*|
|Encryption implementation|ICSharpCode.SharpZipLib.Encryption.\*|
|GZip implementation|ICSharpCode.SharpZipLib.GZip.\*|
|LZW implementation|ICSharpCode.SharpZipLib.Lzw.\*|
|Tar implementation|ICSharpCode.SharpZipLib.Tar.\*|
|ZIP implementation|ICSharpCode.SharpZipLib.Zip.\*|
|Inflater/Deflater|ICSharpCode.SharpZipLib.Zip.Compression.\*|
|Inflater/Deflater streams|ICSharpCode.SharpZipLib.Zip.Compression.Streams.\*|

Credits
-------

SharpZipLib was initially developed by [Mike Krüger](http://www.icsharpcode.net/pub/relations/krueger.aspx). Past maintainers are John Reilly, David Pierson and Neil McNeight. 

And thanks to all the people that contributed features, bug fixes and issue reports.

