# api documentation for  [fstream (v1.0.11)](https://github.com/npm/fstream#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-fstream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fstream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fstream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fstream)
#### Advanced file system stream things

[![NPM](https://nodei.co/npm/fstream.png?downloads=true)](https://www.npmjs.com/package/fstream)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fstream/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fstream_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fstream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fstream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fstream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Isaac Z. Schlueter",
        "email": "i@izs.me",
        "url": "http://blog.izs.me/"
    },
    "bugs": {
        "url": "https://github.com/npm/fstream/issues"
    },
    "dependencies": {
        "graceful-fs": "^4.1.2",
        "inherits": "~2.0.0",
        "mkdirp": ">=0.5 0",
        "rimraf": "2"
    },
    "description": "Advanced file system stream things",
    "devDependencies": {
        "standard": "^4.0.0",
        "tap": "^1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5c1fb1f117477114f0632a0eb4b71b3cb0fd3171",
        "tarball": "https://registry.npmjs.org/fstream/-/fstream-1.0.11.tgz"
    },
    "engines": {
        "node": ">=0.6"
    },
    "gitHead": "1e4527ffe8688d4f5325283d7cf2cf2d61f14c6b",
    "homepage": "https://github.com/npm/fstream#readme",
    "license": "ISC",
    "main": "fstream.js",
    "maintainers": [
        {
            "name": "iarna",
            "email": "me@re-becca.org"
        },
        {
            "name": "isaacs",
            "email": "isaacs@npmjs.com"
        },
        {
            "name": "othiym23",
            "email": "ogd@aoaioxxysz.net"
        },
        {
            "name": "zkat",
            "email": "kat@sykosomatic.org"
        }
    ],
    "name": "fstream",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/npm/fstream.git"
    },
    "scripts": {
        "test": "standard && tap examples/*.js"
    },
    "version": "1.0.11"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fstream](#apidoc.module.fstream)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Abstract ()](#apidoc.element.fstream.Abstract)
1.  [function <span class="apidocSignatureSpan">fstream.</span>DirReader (props)](#apidoc.element.fstream.DirReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>DirWriter (props)](#apidoc.element.fstream.DirWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>FileReader (props)](#apidoc.element.fstream.FileReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>FileWriter (props)](#apidoc.element.fstream.FileWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>LinkReader (props)](#apidoc.element.fstream.LinkReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>LinkWriter (props)](#apidoc.element.fstream.LinkWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>ProxyReader (props)](#apidoc.element.fstream.ProxyReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>ProxyWriter (props)](#apidoc.element.fstream.ProxyWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Reader (props, currentStat)](#apidoc.element.fstream.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Writer (props, current)](#apidoc.element.fstream.Writer)
1.  [function <span class="apidocSignatureSpan">fstream.</span>collect (stream)](#apidoc.element.fstream.collect)
1.  [function <span class="apidocSignatureSpan">fstream.</span>socket_reader (props)](#apidoc.element.fstream.socket_reader)
1.  object <span class="apidocSignatureSpan">fstream.</span>Abstract.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>Dir
1.  object <span class="apidocSignatureSpan">fstream.</span>DirReader.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>DirWriter.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>File
1.  object <span class="apidocSignatureSpan">fstream.</span>FileReader.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>FileWriter.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>Link
1.  object <span class="apidocSignatureSpan">fstream.</span>LinkReader.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>LinkWriter.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>Proxy
1.  object <span class="apidocSignatureSpan">fstream.</span>ProxyReader.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>ProxyWriter.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>Reader.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>Writer.prototype
1.  object <span class="apidocSignatureSpan">fstream.</span>socket_reader.prototype

#### [module fstream.Abstract](#apidoc.module.fstream.Abstract)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Abstract ()](#apidoc.element.fstream.Abstract.Abstract)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.</span>super_ ()](#apidoc.element.fstream.Abstract.super_)

#### [module fstream.Abstract.prototype](#apidoc.module.fstream.Abstract.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>abort ()](#apidoc.element.fstream.Abstract.prototype.abort)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>destroy ()](#apidoc.element.fstream.Abstract.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>error (msg, code, th)](#apidoc.element.fstream.Abstract.prototype.error)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>info (msg, code)](#apidoc.element.fstream.Abstract.prototype.info)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>on (ev, fn)](#apidoc.element.fstream.Abstract.prototype.on)
1.  [function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>warn (msg, code)](#apidoc.element.fstream.Abstract.prototype.warn)

#### [module fstream.Dir](#apidoc.module.fstream.Dir)
1.  [function <span class="apidocSignatureSpan">fstream.Dir.</span>Reader (props)](#apidoc.element.fstream.Dir.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.Dir.</span>Writer (props)](#apidoc.element.fstream.Dir.Writer)

#### [module fstream.DirReader](#apidoc.module.fstream.DirReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>DirReader (props)](#apidoc.element.fstream.DirReader.DirReader)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.DirReader.super_)

#### [module fstream.DirReader.prototype](#apidoc.module.fstream.DirReader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>_getEntries ()](#apidoc.element.fstream.DirReader.prototype._getEntries)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>_read ()](#apidoc.element.fstream.DirReader.prototype._read)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>disown (entry)](#apidoc.element.fstream.DirReader.prototype.disown)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>emitEntry (entry)](#apidoc.element.fstream.DirReader.prototype.emitEntry)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>getChildProps ()](#apidoc.element.fstream.DirReader.prototype.getChildProps)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>pause (who)](#apidoc.element.fstream.DirReader.prototype.pause)
1.  [function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>resume (who)](#apidoc.element.fstream.DirReader.prototype.resume)

#### [module fstream.DirWriter](#apidoc.module.fstream.DirWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>DirWriter (props)](#apidoc.element.fstream.DirWriter.DirWriter)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.</span>super_ (props, current)](#apidoc.element.fstream.DirWriter.super_)

#### [module fstream.DirWriter.prototype](#apidoc.module.fstream.DirWriter.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>_create ()](#apidoc.element.fstream.DirWriter.prototype._create)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>_process ()](#apidoc.element.fstream.DirWriter.prototype._process)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>add (entry)](#apidoc.element.fstream.DirWriter.prototype.add)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>end ()](#apidoc.element.fstream.DirWriter.prototype.end)
1.  [function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>write ()](#apidoc.element.fstream.DirWriter.prototype.write)

#### [module fstream.File](#apidoc.module.fstream.File)
1.  [function <span class="apidocSignatureSpan">fstream.File.</span>Reader (props)](#apidoc.element.fstream.File.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.File.</span>Writer (props)](#apidoc.element.fstream.File.Writer)

#### [module fstream.FileReader](#apidoc.module.fstream.FileReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>FileReader (props)](#apidoc.element.fstream.FileReader.FileReader)
1.  [function <span class="apidocSignatureSpan">fstream.FileReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.FileReader.super_)

#### [module fstream.FileReader.prototype](#apidoc.module.fstream.FileReader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>_getStream ()](#apidoc.element.fstream.FileReader.prototype._getStream)
1.  [function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>_read ()](#apidoc.element.fstream.FileReader.prototype._read)
1.  [function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>pause (who)](#apidoc.element.fstream.FileReader.prototype.pause)
1.  [function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>resume (who)](#apidoc.element.fstream.FileReader.prototype.resume)

#### [module fstream.FileWriter](#apidoc.module.fstream.FileWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>FileWriter (props)](#apidoc.element.fstream.FileWriter.FileWriter)
1.  [function <span class="apidocSignatureSpan">fstream.FileWriter.</span>super_ (props, current)](#apidoc.element.fstream.FileWriter.super_)

#### [module fstream.FileWriter.prototype](#apidoc.module.fstream.FileWriter.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>_create ()](#apidoc.element.fstream.FileWriter.prototype._create)
1.  [function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>_finish ()](#apidoc.element.fstream.FileWriter.prototype._finish)
1.  [function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>end (c)](#apidoc.element.fstream.FileWriter.prototype.end)
1.  [function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>write (c)](#apidoc.element.fstream.FileWriter.prototype.write)

#### [module fstream.Link](#apidoc.module.fstream.Link)
1.  [function <span class="apidocSignatureSpan">fstream.Link.</span>Reader (props)](#apidoc.element.fstream.Link.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.Link.</span>Writer (props)](#apidoc.element.fstream.Link.Writer)

#### [module fstream.LinkReader](#apidoc.module.fstream.LinkReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>LinkReader (props)](#apidoc.element.fstream.LinkReader.LinkReader)
1.  [function <span class="apidocSignatureSpan">fstream.LinkReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.LinkReader.super_)

#### [module fstream.LinkReader.prototype](#apidoc.module.fstream.LinkReader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.LinkReader.prototype.</span>_read ()](#apidoc.element.fstream.LinkReader.prototype._read)
1.  [function <span class="apidocSignatureSpan">fstream.LinkReader.prototype.</span>_stat (currentStat)](#apidoc.element.fstream.LinkReader.prototype._stat)

#### [module fstream.LinkWriter](#apidoc.module.fstream.LinkWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>LinkWriter (props)](#apidoc.element.fstream.LinkWriter.LinkWriter)
1.  [function <span class="apidocSignatureSpan">fstream.LinkWriter.</span>super_ (props, current)](#apidoc.element.fstream.LinkWriter.super_)

#### [module fstream.LinkWriter.prototype](#apidoc.module.fstream.LinkWriter.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.LinkWriter.prototype.</span>_create ()](#apidoc.element.fstream.LinkWriter.prototype._create)
1.  [function <span class="apidocSignatureSpan">fstream.LinkWriter.prototype.</span>end ()](#apidoc.element.fstream.LinkWriter.prototype.end)

#### [module fstream.Proxy](#apidoc.module.fstream.Proxy)
1.  [function <span class="apidocSignatureSpan">fstream.Proxy.</span>Reader (props)](#apidoc.element.fstream.Proxy.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.Proxy.</span>Writer (props)](#apidoc.element.fstream.Proxy.Writer)

#### [module fstream.ProxyReader](#apidoc.module.fstream.ProxyReader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>ProxyReader (props)](#apidoc.element.fstream.ProxyReader.ProxyReader)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.ProxyReader.super_)

#### [module fstream.ProxyReader.prototype](#apidoc.module.fstream.ProxyReader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>_addProxy (proxy)](#apidoc.element.fstream.ProxyReader.prototype._addProxy)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>_stat ()](#apidoc.element.fstream.ProxyReader.prototype._stat)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>pause ()](#apidoc.element.fstream.ProxyReader.prototype.pause)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>resume ()](#apidoc.element.fstream.ProxyReader.prototype.resume)

#### [module fstream.ProxyWriter](#apidoc.module.fstream.ProxyWriter)
1.  [function <span class="apidocSignatureSpan">fstream.</span>ProxyWriter (props)](#apidoc.element.fstream.ProxyWriter.ProxyWriter)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.</span>super_ (props, current)](#apidoc.element.fstream.ProxyWriter.super_)

#### [module fstream.ProxyWriter.prototype](#apidoc.module.fstream.ProxyWriter.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>_addProxy (proxy)](#apidoc.element.fstream.ProxyWriter.prototype._addProxy)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>_stat ()](#apidoc.element.fstream.ProxyWriter.prototype._stat)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>add (entry)](#apidoc.element.fstream.ProxyWriter.prototype.add)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>end (c)](#apidoc.element.fstream.ProxyWriter.prototype.end)
1.  [function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>write (c)](#apidoc.element.fstream.ProxyWriter.prototype.write)

#### [module fstream.Reader](#apidoc.module.fstream.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Reader (props, currentStat)](#apidoc.element.fstream.Reader.Reader)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.</span>Dir (props)](#apidoc.element.fstream.Reader.Dir)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.</span>File (props)](#apidoc.element.fstream.Reader.File)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.</span>Link (props)](#apidoc.element.fstream.Reader.Link)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.</span>Proxy (props)](#apidoc.element.fstream.Reader.Proxy)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.</span>super_ ()](#apidoc.element.fstream.Reader.super_)
1.  object <span class="apidocSignatureSpan">fstream.Reader.</span>hardLinks

#### [module fstream.Reader.prototype](#apidoc.module.fstream.Reader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>_read ()](#apidoc.element.fstream.Reader.prototype._read)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>_stat (currentStat)](#apidoc.element.fstream.Reader.prototype._stat)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>pause (who)](#apidoc.element.fstream.Reader.prototype.pause)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>pipe (dest)](#apidoc.element.fstream.Reader.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>resume (who)](#apidoc.element.fstream.Reader.prototype.resume)

#### [module fstream.Writer](#apidoc.module.fstream.Writer)
1.  [function <span class="apidocSignatureSpan">fstream.</span>Writer (props, current)](#apidoc.element.fstream.Writer.Writer)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.</span>Dir (props)](#apidoc.element.fstream.Writer.Dir)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.</span>File (props)](#apidoc.element.fstream.Writer.File)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.</span>Link (props)](#apidoc.element.fstream.Writer.Link)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.</span>Proxy (props)](#apidoc.element.fstream.Writer.Proxy)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.</span>super_ ()](#apidoc.element.fstream.Writer.super_)
1.  number <span class="apidocSignatureSpan">fstream.Writer.</span>dirmode
1.  number <span class="apidocSignatureSpan">fstream.Writer.</span>filemode

#### [module fstream.Writer.prototype](#apidoc.module.fstream.Writer.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_create ()](#apidoc.element.fstream.Writer.prototype._create)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_finish ()](#apidoc.element.fstream.Writer.prototype._finish)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_stat (current)](#apidoc.element.fstream.Writer.prototype._stat)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>add ()](#apidoc.element.fstream.Writer.prototype.add)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>pipe ()](#apidoc.element.fstream.Writer.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>write ()](#apidoc.element.fstream.Writer.prototype.write)

#### [module fstream.socket_reader](#apidoc.module.fstream.socket_reader)
1.  [function <span class="apidocSignatureSpan">fstream.</span>socket_reader (props)](#apidoc.element.fstream.socket_reader.socket_reader)
1.  [function <span class="apidocSignatureSpan">fstream.socket_reader.</span>super_ (props, currentStat)](#apidoc.element.fstream.socket_reader.super_)

#### [module fstream.socket_reader.prototype](#apidoc.module.fstream.socket_reader.prototype)
1.  [function <span class="apidocSignatureSpan">fstream.socket_reader.prototype.</span>_read ()](#apidoc.element.fstream.socket_reader.prototype._read)



# <a name="apidoc.module.fstream"></a>[module fstream](#apidoc.module.fstream)

#### <a name="apidoc.element.fstream.Abstract"></a>[function <span class="apidocSignatureSpan">fstream.</span>Abstract ()](#apidoc.element.fstream.Abstract)
- description and source-code
```javascript
function Abstract() {
  Stream.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>DirReader (props)](#apidoc.element.fstream.DirReader)
- description and source-code
```javascript
function DirReader(props) {
  var self = this
  if (!(self instanceof DirReader)) {
    throw new Error('DirReader must be called as constructor.')
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    throw new Error('Non-directory type ' + props.type)
  }

  self.entries = null
  self._index = -1
  self._paused = false
  self._length = -1

  if (props.sort) {
    this.sort = props.sort
  }

  Reader.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>DirWriter (props)](#apidoc.element.fstream.DirWriter)
- description and source-code
```javascript
function DirWriter(props) {
  var self = this
  if (!(self instanceof DirWriter)) {
    self.error('DirWriter must be called as constructor.', null, true)
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    self.error('Non-directory type ' + props.type + ' ' +
      JSON.stringify(props), null, true)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>FileReader (props)](#apidoc.element.fstream.FileReader)
- description and source-code
```javascript
function FileReader(props) {
  // console.error("    FR create", props.path, props.size, new Error().stack)
  var self = this
  if (!(self instanceof FileReader)) {
    throw new Error('FileReader must be called as constructor.')
  }

  // should already be established as a File type
  // XXX Todo: preserve hardlinks by tracking dev+inode+nlink,
  // with a HardLinkReader class.
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'File' && props.File))) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesEmitted = 0
  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>FileWriter (props)](#apidoc.element.fstream.FileWriter)
- description and source-code
```javascript
function FileWriter(props) {
  var self = this
  if (!(self instanceof FileWriter)) {
    throw new Error('FileWriter must be called as constructor.')
  }

  // should already be established as a File type
  if (props.type !== 'File' || !props.File) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesWritten = 0

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>LinkReader (props)](#apidoc.element.fstream.LinkReader)
- description and source-code
```javascript
function LinkReader(props) {
  var self = this
  if (!(self instanceof LinkReader)) {
    throw new Error('LinkReader must be called as constructor.')
  }

  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>LinkWriter (props)](#apidoc.element.fstream.LinkWriter)
- description and source-code
```javascript
function LinkWriter(props) {
  var self = this
  if (!(self instanceof LinkWriter)) {
    throw new Error('LinkWriter must be called as constructor.')
  }

  // should already be established as a Link type
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  if (props.linkpath === '') props.linkpath = '.'
  if (!props.linkpath) {
    self.error('Need linkpath property to create ' + props.type)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>ProxyReader (props)](#apidoc.element.fstream.ProxyReader)
- description and source-code
```javascript
function ProxyReader(props) {
  var self = this
  if (!(self instanceof ProxyReader)) {
    throw new Error('ProxyReader must be called as constructor.')
  }

  self.props = props
  self._buffer = []
  self.ready = false

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>ProxyWriter (props)](#apidoc.element.fstream.ProxyWriter)
- description and source-code
```javascript
function ProxyWriter(props) {
  var self = this
  if (!(self instanceof ProxyWriter)) {
    throw new Error('ProxyWriter must be called as constructor.')
  }

  self.props = props
  self._needDrain = false

  Writer.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader"></a>[function <span class="apidocSignatureSpan">fstream.</span>Reader (props, currentStat)](#apidoc.element.fstream.Reader)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.Writer"></a>[function <span class="apidocSignatureSpan">fstream.</span>Writer (props, current)](#apidoc.element.fstream.Writer)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```

#### <a name="apidoc.element.fstream.collect"></a>[function <span class="apidocSignatureSpan">fstream.</span>collect (stream)](#apidoc.element.fstream.collect)
- description and source-code
```javascript
function collect(stream) {
  if (stream._collected) return

  if (stream._paused) return stream.on('resume', collect.bind(null, stream))

  stream._collected = true
  stream.pause()

  stream.on('data', save)
  stream.on('end', save)
  var buf = []
  function save (b) {
    if (typeof b === 'string') b = new Buffer(b)
    if (Buffer.isBuffer(b) && !b.length) return
    buf.push(b)
  }

  stream.on('entry', saveEntry)
  var entryBuffer = []
  function saveEntry (e) {
    collect(e)
    entryBuffer.push(e)
  }

  stream.on('proxy', proxyPause)
  function proxyPause (p) {
    p.pause()
  }

  // replace the pipe method with a new version that will
  // unlock the buffered stuff.  if you just call .pipe()
  // without a destination, then it'll re-play the events.
  stream.pipe = (function (orig) {
    return function (dest) {
      // console.error(' === open the pipes', dest && dest.path)

      // let the entries flow through one at a time.
      // Once they're all done, then we can resume completely.
      var e = 0
      ;(function unblockEntry () {
        var entry = entryBuffer[e++]
        // console.error(" ==== unblock entry", entry && entry.path)
        if (!entry) return resume()
        entry.on('end', unblockEntry)
        if (dest) dest.add(entry)
        else stream.emit('entry', entry)
      })()

      function resume () {
        stream.removeListener('entry', saveEntry)
        stream.removeListener('data', save)
        stream.removeListener('end', save)

        stream.pipe = orig
        if (dest) stream.pipe(dest)

        buf.forEach(function (b) {
          if (b) stream.emit('data', b)
          else stream.emit('end')
        })

        stream.resume()
      }

      return dest
    }
  })(stream.pipe)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.socket_reader"></a>[function <span class="apidocSignatureSpan">fstream.</span>socket_reader (props)](#apidoc.element.fstream.socket_reader)
- description and source-code
```javascript
function SocketReader(props) {
  var self = this
  if (!(self instanceof SocketReader)) {
    throw new Error('SocketReader must be called as constructor.')
  }

  if (!(props.type === 'Socket' && props.Socket)) {
    throw new Error('Non-socket type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.Abstract"></a>[module fstream.Abstract](#apidoc.module.fstream.Abstract)

#### <a name="apidoc.element.fstream.Abstract.Abstract"></a>[function <span class="apidocSignatureSpan">fstream.</span>Abstract ()](#apidoc.element.fstream.Abstract.Abstract)
- description and source-code
```javascript
function Abstract() {
  Stream.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Abstract.super_"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.</span>super_ ()](#apidoc.element.fstream.Abstract.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.Abstract.prototype"></a>[module fstream.Abstract.prototype](#apidoc.module.fstream.Abstract.prototype)

#### <a name="apidoc.element.fstream.Abstract.prototype.abort"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>abort ()](#apidoc.element.fstream.Abstract.prototype.abort)
- description and source-code
```javascript
abort = function () {
  this._aborted = true
  this.emit('abort')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Abstract.prototype.destroy"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>destroy ()](#apidoc.element.fstream.Abstract.prototype.destroy)
- description and source-code
```javascript
destroy = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Abstract.prototype.error"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>error (msg, code, th)](#apidoc.element.fstream.Abstract.prototype.error)
- description and source-code
```javascript
error = function (msg, code, th) {
  var er = decorate(msg, code, this)
  if (th) throw er
  else this.emit('error', er)
}
```
- example usage
```shell
...
  }

  // replace the pipe method with a new version that will
  // unlock the buffered stuff.  if you just call .pipe()
  // without a destination, then it'll re-play the events.
  stream.pipe = (function (orig) {
    return function (dest) {
// console.error(' === open the pipes', dest && dest.path)

// let the entries flow through one at a time.
// Once they're all done, then we can resume completely.
var e = 0
;(function unblockEntry () {
  var entry = entryBuffer[e++]
  // console.error(" ==== unblock entry", entry && entry.path)
...
```

#### <a name="apidoc.element.fstream.Abstract.prototype.info"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>info (msg, code)](#apidoc.element.fstream.Abstract.prototype.info)
- description and source-code
```javascript
info = function (msg, code) {
  this.emit('info', msg, code)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Abstract.prototype.on"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>on (ev, fn)](#apidoc.element.fstream.Abstract.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  if (ev === 'ready' && this.ready) {
    process.nextTick(fn.bind(this))
  } else {
    Stream.prototype.on.call(this, ev, fn)
  }
  return this
}
```
- example usage
```shell
...


module.exports = collect

function collect (stream) {
if (stream._collected) return

if (stream._paused) return stream.on('resume', collect.bind(null, stream))

stream._collected = true
stream.pause()

stream.on('data', save)
stream.on('end', save)
var buf = []
...
```

#### <a name="apidoc.element.fstream.Abstract.prototype.warn"></a>[function <span class="apidocSignatureSpan">fstream.Abstract.prototype.</span>warn (msg, code)](#apidoc.element.fstream.Abstract.prototype.warn)
- description and source-code
```javascript
warn = function (msg, code) {
  var self = this
  var er = decorate(msg, code, self)
  if (!self.listeners('warn')) {
    console.error('%s %s\n' +
    'path = %s\n' +
    'syscall = %s\n' +
    'fstream_type = %s\n' +
    'fstream_path = %s\n' +
    'fstream_unc_path = %s\n' +
    'fstream_class = %s\n' +
    'fstream_stack =\n%s\n',
      code || 'UNKNOWN',
      er.stack,
      er.path,
      er.syscall,
      er.fstream_type,
      er.fstream_path,
      er.fstream_unc_path,
      er.fstream_class,
      er.fstream_stack.join('\n'))
  } else {
    self.emit('warn', er)
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.Dir"></a>[module fstream.Dir](#apidoc.module.fstream.Dir)

#### <a name="apidoc.element.fstream.Dir.Reader"></a>[function <span class="apidocSignatureSpan">fstream.Dir.</span>Reader (props)](#apidoc.element.fstream.Dir.Reader)
- description and source-code
```javascript
function DirReader(props) {
  var self = this
  if (!(self instanceof DirReader)) {
    throw new Error('DirReader must be called as constructor.')
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    throw new Error('Non-directory type ' + props.type)
  }

  self.entries = null
  self._index = -1
  self._paused = false
  self._length = -1

  if (props.sort) {
    this.sort = props.sort
  }

  Reader.call(this, props)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.Dir.Writer"></a>[function <span class="apidocSignatureSpan">fstream.Dir.</span>Writer (props)](#apidoc.element.fstream.Dir.Writer)
- description and source-code
```javascript
function DirWriter(props) {
  var self = this
  if (!(self instanceof DirWriter)) {
    self.error('DirWriter must be called as constructor.', null, true)
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    self.error('Non-directory type ' + props.type + ' ' +
      JSON.stringify(props), null, true)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```



# <a name="apidoc.module.fstream.DirReader"></a>[module fstream.DirReader](#apidoc.module.fstream.DirReader)

#### <a name="apidoc.element.fstream.DirReader.DirReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>DirReader (props)](#apidoc.element.fstream.DirReader.DirReader)
- description and source-code
```javascript
function DirReader(props) {
  var self = this
  if (!(self instanceof DirReader)) {
    throw new Error('DirReader must be called as constructor.')
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    throw new Error('Non-directory type ' + props.type)
  }

  self.entries = null
  self._index = -1
  self._paused = false
  self._length = -1

  if (props.sort) {
    this.sort = props.sort
  }

  Reader.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.super_"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.DirReader.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.DirReader.prototype"></a>[module fstream.DirReader.prototype](#apidoc.module.fstream.DirReader.prototype)

#### <a name="apidoc.element.fstream.DirReader.prototype._getEntries"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>_getEntries ()](#apidoc.element.fstream.DirReader.prototype._getEntries)
- description and source-code
```javascript
_getEntries = function () {
  var self = this

  // race condition.  might pause() before calling _getEntries,
  // and then resume, and try to get them a second time.
  if (self._gotEntries) return
  self._gotEntries = true

  fs.readdir(self._path, function (er, entries) {
    if (er) return self.error(er)

    self.entries = entries

    self.emit('entries', entries)
    if (self._paused) self.once('resume', processEntries)
    else processEntries()

    function processEntries () {
      self._length = self.entries.length
      if (typeof self.sort === 'function') {
        self.entries = self.entries.sort(self.sort.bind(self))
      }
      self._read()
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.prototype._read"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>_read ()](#apidoc.element.fstream.DirReader.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this

  if (!self.entries) return self._getEntries()

  if (self._paused || self._currentEntry || self._aborted) {
    // console.error('DR paused=%j, current=%j, aborted=%j', self._paused, !!self._currentEntry, self._aborted)
    return
  }

  self._index++
  if (self._index >= self.entries.length) {
    if (!self._ended) {
      self._ended = true
      self.emit('end')
      self.emit('close')
    }
    return
  }

  // ok, handle this one, then.

  // save creating a proxy, by stat'ing the thing now.
  var p = path.resolve(self._path, self.entries[self._index])
  assert(p !== self._path)
  assert(self.entries[self._index])

  // set this to prevent trying to _read() again in the stat time.
  self._currentEntry = p
  fs[ self.props.follow ? 'stat' : 'lstat' ](p, function (er, stat) {
    if (er) return self.error(er)

    var who = self._proxy || self

    stat.path = p
    stat.basename = path.basename(p)
    stat.dirname = path.dirname(p)
    var childProps = self.getChildProps.call(who, stat)
    childProps.path = p
    childProps.basename = path.basename(p)
    childProps.dirname = path.dirname(p)

    var entry = Reader(childProps, stat)

    // console.error("DR Entry", p, stat.size)

    self._currentEntry = entry

    // "entry" events are for direct entries in a specific dir.
    // "child" events are for any and all children at all levels.
    // This nomenclature is not completely final.

    entry.on('pause', function (who) {
      if (!self._paused && !entry._disowned) {
        self.pause(who)
      }
    })

    entry.on('resume', function (who) {
      if (self._paused && !entry._disowned) {
        self.resume(who)
      }
    })

    entry.on('stat', function (props) {
      self.emit('_entryStat', entry, props)
      if (entry._aborted) return
      if (entry._paused) {
        entry.once('resume', function () {
          self.emit('entryStat', entry, props)
        })
      } else self.emit('entryStat', entry, props)
    })

    entry.on('ready', function EMITCHILD () {
      // console.error("DR emit child", entry._path)
      if (self._paused) {
        // console.error("  DR emit child - try again later")
        // pause the child, and emit the "entry" event once we drain.
        // console.error("DR pausing child entry")
        entry.pause(self)
        return self.once('resume', EMITCHILD)
      }

      // skip over sockets.  they can't be piped around properly,
      // so there's really no sense even acknowledging them.
      // if someone really wants to see them, they can listen to
      // the "socket" events.
      if (entry.type === 'Socket') {
        self.emit('socket', entry)
      } else {
        self.emitEntry(entry)
      }
    })

    var ended = false
    entry.on('close', onend)
    entry.on('disown', onend)
    function onend () {
      if (ended) return
      ended = true
      self.emit('childEnd', entry)
      self.emit('entryEnd', entry)
      self._currentEntry = null
      if (!self._paused) {
        self._read()
      }
    }

    // XXX Remove this.  Works in node as of 0.6.2 or so.
    // Long filenames should not break stuff.
    entry.on('error', function (er) {
      if (entry._swallowErrors) {
        self.warn(er)
        entry.emit('end')
        entry.emit('close')
      } else {
        self.emit('error', er)
      }
    })

    // proxy up some events.
    ;[
      'child',
      'childEnd',
      'warn'
    ].forEach(function (ev) {
      entry.on(ev, self.emit.bind(self, ev))
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.prototype.disown"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>disown (entry)](#apidoc.element.fstream.DirReader.prototype.disown)
- description and source-code
```javascript
disown = function (entry) {
  entry.emit('beforeDisown')
  entry._disowned = true
  entry.parent = entry.root = null
  if (entry === this._currentEntry) {
    this._currentEntry = null
  }
  entry.emit('disown')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.prototype.emitEntry"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>emitEntry (entry)](#apidoc.element.fstream.DirReader.prototype.emitEntry)
- description and source-code
```javascript
emitEntry = function (entry) {
  this.emit('entry', entry)
  this.emit('child', entry)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.prototype.getChildProps"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>getChildProps ()](#apidoc.element.fstream.DirReader.prototype.getChildProps)
- description and source-code
```javascript
getChildProps = function () {
  return {
    depth: this.depth + 1,
    root: this.root || this,
    parent: this,
    follow: this.follow,
    filter: this.filter,
    sort: this.props.sort,
    hardlinks: this.props.hardlinks
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirReader.prototype.pause"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>pause (who)](#apidoc.element.fstream.DirReader.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  var self = this
  if (self._paused) return
  who = who || self
  self._paused = true
  if (self._currentEntry && self._currentEntry.pause) {
    self._currentEntry.pause(who)
  }
  self.emit('pause', who)
}
```
- example usage
```shell
...

function collect (stream) {
if (stream._collected) return

if (stream._paused) return stream.on('resume', collect.bind(null, stream))

stream._collected = true
stream.pause()

stream.on('data', save)
stream.on('end', save)
var buf = []
function save (b) {
  if (typeof b === 'string') b = new Buffer(b)
  if (Buffer.isBuffer(b) && !b.length) return
...
```

#### <a name="apidoc.element.fstream.DirReader.prototype.resume"></a>[function <span class="apidocSignatureSpan">fstream.DirReader.prototype.</span>resume (who)](#apidoc.element.fstream.DirReader.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  var self = this
  if (!self._paused) return
  who = who || self

  self._paused = false
  // console.error('DR Emit Resume', self._path)
  self.emit('resume', who)
  if (self._paused) {
    // console.error('DR Re-paused', self._path)
    return
  }

  if (self._currentEntry) {
    if (self._currentEntry.resume) self._currentEntry.resume(who)
  } else self._read()
}
```
- example usage
```shell
...
        if (dest) stream.pipe(dest)

        buf.forEach(function (b) {
          if (b) stream.emit('data', b)
          else stream.emit('end')
        })

        stream.resume()
      }

      return dest
    }
  })(stream.pipe)
}
...
```



# <a name="apidoc.module.fstream.DirWriter"></a>[module fstream.DirWriter](#apidoc.module.fstream.DirWriter)

#### <a name="apidoc.element.fstream.DirWriter.DirWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>DirWriter (props)](#apidoc.element.fstream.DirWriter.DirWriter)
- description and source-code
```javascript
function DirWriter(props) {
  var self = this
  if (!(self instanceof DirWriter)) {
    self.error('DirWriter must be called as constructor.', null, true)
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    self.error('Non-directory type ' + props.type + ' ' +
      JSON.stringify(props), null, true)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirWriter.super_"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.</span>super_ (props, current)](#apidoc.element.fstream.DirWriter.super_)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.DirWriter.prototype"></a>[module fstream.DirWriter.prototype](#apidoc.module.fstream.DirWriter.prototype)

#### <a name="apidoc.element.fstream.DirWriter.prototype._create"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>_create ()](#apidoc.element.fstream.DirWriter.prototype._create)
- description and source-code
```javascript
_create = function () {
  var self = this
  mkdir(self._path, Writer.dirmode, function (er) {
    if (er) return self.error(er)
    // ready to start getting entries!
    self.ready = true
    self.emit('ready')
    self._process()
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirWriter.prototype._process"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>_process ()](#apidoc.element.fstream.DirWriter.prototype._process)
- description and source-code
```javascript
_process = function () {
  var self = this

  // console.error('DW Process p=%j', self._processing, self.basename)

  if (self._processing) return

  var entry = self._buffer.shift()
  if (!entry) {
    // console.error("DW Drain")
    self.emit('drain')
    if (self._ended) self._finish()
    return
  }

  self._processing = true
  // console.error("DW Entry", entry._path)

  self.emit('entry', entry)

  // ok, add this entry
  //
  // don't allow recursive copying
  var p = entry
  var pp
  do {
    pp = p._path || p.path
    if (pp === self.root._path || pp === self._path ||
      (pp && pp.indexOf(self._path) === 0)) {
      // console.error('DW Exit (recursive)', entry.basename, self._path)
      self._processing = false
      if (entry._collected) entry.pipe()
      return self._process()
    }
    p = p.parent
  } while (p)

  // console.error("DW not recursive")

  // chop off the entry's root dir, replace with ours
  var props = {
    parent: self,
    root: self.root || self,
    type: entry.type,
    depth: self.depth + 1
  }

  pp = entry._path || entry.path || entry.props.path
  if (entry.parent) {
    pp = pp.substr(entry.parent._path.length + 1)
  }
  // get rid of any ../../ shenanigans
  props.path = path.join(self.path, path.join('/', pp))

  // if i have a filter, the child should inherit it.
  props.filter = self.filter

  // all the rest of the stuff, copy over from the source.
  Object.keys(entry.props).forEach(function (k) {
    if (!props.hasOwnProperty(k)) {
      props[k] = entry.props[k]
    }
  })

  // not sure at this point what kind of writer this is.
  var child = self._currentChild = new Writer(props)
  child.on('ready', function () {
    // console.error("DW Child Ready", child.type, child._path)
    // console.error("  resuming", entry._path)
    entry.pipe(child)
    entry.resume()
  })

  // XXX Make this work in node.
  // Long filenames should not break stuff.
  child.on('error', function (er) {
    if (child._swallowErrors) {
      self.warn(er)
      child.emit('end')
      child.emit('close')
    } else {
      self.emit('error', er)
    }
  })

  // we fire _end internally *after* end, so that we don't move on
  // until any "end" listeners have had their chance to do stuff.
  child.on('close', onend)
  var ended = false
  function onend () {
    if (ended) return
    ended = true
    // console.error("* DW Child end", child.basename)
    self._currentChild = null
    self._processing = false
    self._process()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.DirWriter.prototype.add"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>add (entry)](#apidoc.element.fstream.DirWriter.prototype.add)
- description and source-code
```javascript
add = function (entry) {
  var self = this

  // console.error('\tadd', entry._path, '->', self._path)
  collect(entry)
  if (!self.ready || self._currentEntry) {
    self._buffer.push(entry)
    return false
  }

  // create a new writer, and pipe the incoming entry into it.
  if (self._ended) {
    return self.error('add after end')
  }

  self._buffer.push(entry)
  self._process()

  return this._buffer.length === 0
}
```
- example usage
```shell
...
// Once they're all done, then we can resume completely.
var e = 0
;(function unblockEntry () {
  var entry = entryBuffer[e++]
  // console.error(" ==== unblock entry", entry && entry.path)
  if (!entry) return resume()
  entry.on('end', unblockEntry)
  if (dest) dest.add(entry)
  else stream.emit('entry', entry)
})()

function resume () {
  stream.removeListener('entry', saveEntry)
  stream.removeListener('data', save)
  stream.removeListener('end', save)
...
```

#### <a name="apidoc.element.fstream.DirWriter.prototype.end"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>end ()](#apidoc.element.fstream.DirWriter.prototype.end)
- description and source-code
```javascript
end = function () {
  this._ended = true
  this._process()
}
```
- example usage
```shell
...
'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.

'''javascript
...
```

#### <a name="apidoc.element.fstream.DirWriter.prototype.write"></a>[function <span class="apidocSignatureSpan">fstream.DirWriter.prototype.</span>write ()](#apidoc.element.fstream.DirWriter.prototype.write)
- description and source-code
```javascript
write = function () {
  return true
}
```
- example usage
```shell
...

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.
...
```



# <a name="apidoc.module.fstream.File"></a>[module fstream.File](#apidoc.module.fstream.File)

#### <a name="apidoc.element.fstream.File.Reader"></a>[function <span class="apidocSignatureSpan">fstream.File.</span>Reader (props)](#apidoc.element.fstream.File.Reader)
- description and source-code
```javascript
function FileReader(props) {
  // console.error("    FR create", props.path, props.size, new Error().stack)
  var self = this
  if (!(self instanceof FileReader)) {
    throw new Error('FileReader must be called as constructor.')
  }

  // should already be established as a File type
  // XXX Todo: preserve hardlinks by tracking dev+inode+nlink,
  // with a HardLinkReader class.
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'File' && props.File))) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesEmitted = 0
  Reader.call(self, props)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.File.Writer"></a>[function <span class="apidocSignatureSpan">fstream.File.</span>Writer (props)](#apidoc.element.fstream.File.Writer)
- description and source-code
```javascript
function FileWriter(props) {
  var self = this
  if (!(self instanceof FileWriter)) {
    throw new Error('FileWriter must be called as constructor.')
  }

  // should already be established as a File type
  if (props.type !== 'File' || !props.File) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesWritten = 0

  Writer.call(this, props)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```



# <a name="apidoc.module.fstream.FileReader"></a>[module fstream.FileReader](#apidoc.module.fstream.FileReader)

#### <a name="apidoc.element.fstream.FileReader.FileReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>FileReader (props)](#apidoc.element.fstream.FileReader.FileReader)
- description and source-code
```javascript
function FileReader(props) {
  // console.error("    FR create", props.path, props.size, new Error().stack)
  var self = this
  if (!(self instanceof FileReader)) {
    throw new Error('FileReader must be called as constructor.')
  }

  // should already be established as a File type
  // XXX Todo: preserve hardlinks by tracking dev+inode+nlink,
  // with a HardLinkReader class.
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'File' && props.File))) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesEmitted = 0
  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileReader.super_"></a>[function <span class="apidocSignatureSpan">fstream.FileReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.FileReader.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.FileReader.prototype"></a>[module fstream.FileReader.prototype](#apidoc.module.fstream.FileReader.prototype)

#### <a name="apidoc.element.fstream.FileReader.prototype._getStream"></a>[function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>_getStream ()](#apidoc.element.fstream.FileReader.prototype._getStream)
- description and source-code
```javascript
_getStream = function () {
  var self = this
  var stream = self._stream = fs.createReadStream(self._path, self.props)

  if (self.props.blksize) {
    stream.bufferSize = self.props.blksize
  }

  stream.on('open', self.emit.bind(self, 'open'))

  stream.on('data', function (c) {
    // console.error('\t\t%d %s', c.length, self.basename)
    self._bytesEmitted += c.length
    // no point saving empty chunks
    if (!c.length) {
      return
    } else if (self._paused || self._buffer.length) {
      self._buffer.push(c)
      self._read()
    } else self.emit('data', c)
  })

  stream.on('end', function () {
    if (self._paused || self._buffer.length) {
      // console.error('FR Buffering End', self._path)
      self._buffer.push(EOF)
      self._read()
    } else {
      self.emit('end')
    }

    if (self._bytesEmitted !== self.props.size) {
      self.error("Didn't get expected byte count\n" +
        'expect: ' + self.props.size + '\n' +
        'actual: ' + self._bytesEmitted)
    }
  })

  stream.on('close', function () {
    if (self._paused || self._buffer.length) {
      // console.error('FR Buffering Close', self._path)
      self._buffer.push(CLOSE)
      self._read()
    } else {
      // console.error('FR close 1', self._path)
      self.emit('close')
    }
  })

  stream.on('error', function (e) {
    self.emit('error', e)
  })

  self._read()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileReader.prototype._read"></a>[function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>_read ()](#apidoc.element.fstream.FileReader.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  // console.error('FR _read', self._path)
  if (self._paused) {
    // console.error('FR _read paused', self._path)
    return
  }

  if (!self._stream) {
    // console.error('FR _getStream calling', self._path)
    return self._getStream()
  }

  // clear out the buffer, if there is one.
  if (self._buffer.length) {
    // console.error('FR _read has buffer', self._buffer.length, self._path)
    var buf = self._buffer
    for (var i = 0, l = buf.length; i < l; i++) {
      var c = buf[i]
      if (c === EOF) {
        // console.error('FR Read emitting buffered end', self._path)
        self.emit('end')
      } else if (c === CLOSE) {
        // console.error('FR Read emitting buffered close', self._path)
        self.emit('close')
      } else {
        // console.error('FR Read emitting buffered data', self._path)
        self.emit('data', c)
      }

      if (self._paused) {
        // console.error('FR Read Re-pausing at '+i, self._path)
        self._buffer = buf.slice(i)
        return
      }
    }
    self._buffer.length = 0
  }
// console.error("FR _read done")
// that's about all there is to it.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileReader.prototype.pause"></a>[function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>pause (who)](#apidoc.element.fstream.FileReader.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  var self = this
  // console.error('FR Pause', self._path)
  if (self._paused) return
  who = who || self
  self._paused = true
  if (self._stream) self._stream.pause()
  self.emit('pause', who)
}
```
- example usage
```shell
...

function collect (stream) {
if (stream._collected) return

if (stream._paused) return stream.on('resume', collect.bind(null, stream))

stream._collected = true
stream.pause()

stream.on('data', save)
stream.on('end', save)
var buf = []
function save (b) {
  if (typeof b === 'string') b = new Buffer(b)
  if (Buffer.isBuffer(b) && !b.length) return
...
```

#### <a name="apidoc.element.fstream.FileReader.prototype.resume"></a>[function <span class="apidocSignatureSpan">fstream.FileReader.prototype.</span>resume (who)](#apidoc.element.fstream.FileReader.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  var self = this
  // console.error('FR Resume', self._path)
  if (!self._paused) return
  who = who || self
  self.emit('resume', who)
  self._paused = false
  if (self._stream) self._stream.resume()
  self._read()
}
```
- example usage
```shell
...
        if (dest) stream.pipe(dest)

        buf.forEach(function (b) {
          if (b) stream.emit('data', b)
          else stream.emit('end')
        })

        stream.resume()
      }

      return dest
    }
  })(stream.pipe)
}
...
```



# <a name="apidoc.module.fstream.FileWriter"></a>[module fstream.FileWriter](#apidoc.module.fstream.FileWriter)

#### <a name="apidoc.element.fstream.FileWriter.FileWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>FileWriter (props)](#apidoc.element.fstream.FileWriter.FileWriter)
- description and source-code
```javascript
function FileWriter(props) {
  var self = this
  if (!(self instanceof FileWriter)) {
    throw new Error('FileWriter must be called as constructor.')
  }

  // should already be established as a File type
  if (props.type !== 'File' || !props.File) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesWritten = 0

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileWriter.super_"></a>[function <span class="apidocSignatureSpan">fstream.FileWriter.</span>super_ (props, current)](#apidoc.element.fstream.FileWriter.super_)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.FileWriter.prototype"></a>[module fstream.FileWriter.prototype](#apidoc.module.fstream.FileWriter.prototype)

#### <a name="apidoc.element.fstream.FileWriter.prototype._create"></a>[function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>_create ()](#apidoc.element.fstream.FileWriter.prototype._create)
- description and source-code
```javascript
_create = function () {
  var self = this
  if (self._stream) return

  var so = {}
  if (self.props.flags) so.flags = self.props.flags
  so.mode = Writer.filemode
  if (self._old && self._old.blksize) so.bufferSize = self._old.blksize

  self._stream = fs.createWriteStream(self._path, so)

  self._stream.on('open', function () {
    // console.error("FW open", self._buffer, self._path)
    self.ready = true
    self._buffer.forEach(function (c) {
      if (c === EOF) self._stream.end()
      else self._stream.write(c)
    })
    self.emit('ready')
    // give this a kick just in case it needs it.
    self.emit('drain')
  })

  self._stream.on('error', function (er) { self.emit('error', er) })

  self._stream.on('drain', function () { self.emit('drain') })

  self._stream.on('close', function () {
    // console.error('\n\nFW Stream Close', self._path, self.size)
    self._finish()
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileWriter.prototype._finish"></a>[function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>_finish ()](#apidoc.element.fstream.FileWriter.prototype._finish)
- description and source-code
```javascript
_finish = function () {
  var self = this
  if (typeof self.size === 'number' && self._bytesWritten !== self.size) {
    self.error(
      'Did not get expected byte count.\n' +
      'expect: ' + self.size + '\n' +
      'actual: ' + self._bytesWritten)
  }
  Writer.prototype._finish.call(self)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.FileWriter.prototype.end"></a>[function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>end (c)](#apidoc.element.fstream.FileWriter.prototype.end)
- description and source-code
```javascript
end = function (c) {
  var self = this

  if (c) self.write(c)

  if (!self.ready) {
    self._buffer.push(EOF)
    return false
  }

  return self._stream.end()
}
```
- example usage
```shell
...
'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.

'''javascript
...
```

#### <a name="apidoc.element.fstream.FileWriter.prototype.write"></a>[function <span class="apidocSignatureSpan">fstream.FileWriter.prototype.</span>write (c)](#apidoc.element.fstream.FileWriter.prototype.write)
- description and source-code
```javascript
write = function (c) {
  var self = this

  self._bytesWritten += c.length

  if (!self.ready) {
    if (!Buffer.isBuffer(c) && typeof c !== 'string') {
      throw new Error('invalid write data')
    }
    self._buffer.push(c)
    return false
  }

  var ret = self._stream.write(c)
  // console.error('\t-- fw wrote, _stream says', ret, self._stream._queue.length)

  // allow 2 buffered writes, because otherwise there's just too
  // much stop and go bs.
  if (ret === false && self._stream._queue) {
    return self._stream._queue.length <= 2
  } else {
    return ret
  }
}
```
- example usage
```shell
...

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.
...
```



# <a name="apidoc.module.fstream.Link"></a>[module fstream.Link](#apidoc.module.fstream.Link)

#### <a name="apidoc.element.fstream.Link.Reader"></a>[function <span class="apidocSignatureSpan">fstream.Link.</span>Reader (props)](#apidoc.element.fstream.Link.Reader)
- description and source-code
```javascript
function LinkReader(props) {
  var self = this
  if (!(self instanceof LinkReader)) {
    throw new Error('LinkReader must be called as constructor.')
  }

  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.Link.Writer"></a>[function <span class="apidocSignatureSpan">fstream.Link.</span>Writer (props)](#apidoc.element.fstream.Link.Writer)
- description and source-code
```javascript
function LinkWriter(props) {
  var self = this
  if (!(self instanceof LinkWriter)) {
    throw new Error('LinkWriter must be called as constructor.')
  }

  // should already be established as a Link type
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  if (props.linkpath === '') props.linkpath = '.'
  if (!props.linkpath) {
    self.error('Need linkpath property to create ' + props.type)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```



# <a name="apidoc.module.fstream.LinkReader"></a>[module fstream.LinkReader](#apidoc.module.fstream.LinkReader)

#### <a name="apidoc.element.fstream.LinkReader.LinkReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>LinkReader (props)](#apidoc.element.fstream.LinkReader.LinkReader)
- description and source-code
```javascript
function LinkReader(props) {
  var self = this
  if (!(self instanceof LinkReader)) {
    throw new Error('LinkReader must be called as constructor.')
  }

  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkReader.super_"></a>[function <span class="apidocSignatureSpan">fstream.LinkReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.LinkReader.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.LinkReader.prototype"></a>[module fstream.LinkReader.prototype](#apidoc.module.fstream.LinkReader.prototype)

#### <a name="apidoc.element.fstream.LinkReader.prototype._read"></a>[function <span class="apidocSignatureSpan">fstream.LinkReader.prototype.</span>_read ()](#apidoc.element.fstream.LinkReader.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  if (self._paused) return
  // basically just a no-op, since we got all the info we need
  // from the _stat method
  if (!self._ended) {
    self.emit('end')
    self.emit('close')
    self._ended = true
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkReader.prototype._stat"></a>[function <span class="apidocSignatureSpan">fstream.LinkReader.prototype.</span>_stat (currentStat)](#apidoc.element.fstream.LinkReader.prototype._stat)
- description and source-code
```javascript
_stat = function (currentStat) {
  var self = this
  fs.readlink(self._path, function (er, linkpath) {
    if (er) return self.error(er)
    self.linkpath = self.props.linkpath = linkpath
    self.emit('linkpath', linkpath)
    Reader.prototype._stat.call(self, currentStat)
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.LinkWriter"></a>[module fstream.LinkWriter](#apidoc.module.fstream.LinkWriter)

#### <a name="apidoc.element.fstream.LinkWriter.LinkWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>LinkWriter (props)](#apidoc.element.fstream.LinkWriter.LinkWriter)
- description and source-code
```javascript
function LinkWriter(props) {
  var self = this
  if (!(self instanceof LinkWriter)) {
    throw new Error('LinkWriter must be called as constructor.')
  }

  // should already be established as a Link type
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  if (props.linkpath === '') props.linkpath = '.'
  if (!props.linkpath) {
    self.error('Need linkpath property to create ' + props.type)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkWriter.super_"></a>[function <span class="apidocSignatureSpan">fstream.LinkWriter.</span>super_ (props, current)](#apidoc.element.fstream.LinkWriter.super_)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.LinkWriter.prototype"></a>[module fstream.LinkWriter.prototype](#apidoc.module.fstream.LinkWriter.prototype)

#### <a name="apidoc.element.fstream.LinkWriter.prototype._create"></a>[function <span class="apidocSignatureSpan">fstream.LinkWriter.prototype.</span>_create ()](#apidoc.element.fstream.LinkWriter.prototype._create)
- description and source-code
```javascript
_create = function () {
  // console.error(" LW _create")
  var self = this
  var hard = self.type === 'Link' || process.platform === 'win32'
  var link = hard ? 'link' : 'symlink'
  var lp = hard ? path.resolve(self.dirname, self.linkpath) : self.linkpath

  // can only change the link path by clobbering
  // For hard links, let's just assume that's always the case, since
  // there's no good way to read them if we don't already know.
  if (hard) return clobber(self, lp, link)

  fs.readlink(self._path, function (er, p) {
    // only skip creation if it's exactly the same link
    if (p && p === lp) return finish(self)
    clobber(self, lp, link)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.LinkWriter.prototype.end"></a>[function <span class="apidocSignatureSpan">fstream.LinkWriter.prototype.</span>end ()](#apidoc.element.fstream.LinkWriter.prototype.end)
- description and source-code
```javascript
end = function () {
  // console.error("LW finish in end")
  this._ended = true
  if (this.ready) {
    this._finished = true
    this._finish()
  }
}
```
- example usage
```shell
...
'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.

'''javascript
...
```



# <a name="apidoc.module.fstream.Proxy"></a>[module fstream.Proxy](#apidoc.module.fstream.Proxy)

#### <a name="apidoc.element.fstream.Proxy.Reader"></a>[function <span class="apidocSignatureSpan">fstream.Proxy.</span>Reader (props)](#apidoc.element.fstream.Proxy.Reader)
- description and source-code
```javascript
function ProxyReader(props) {
  var self = this
  if (!(self instanceof ProxyReader)) {
    throw new Error('ProxyReader must be called as constructor.')
  }

  self.props = props
  self._buffer = []
  self.ready = false

  Reader.call(self, props)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.Proxy.Writer"></a>[function <span class="apidocSignatureSpan">fstream.Proxy.</span>Writer (props)](#apidoc.element.fstream.Proxy.Writer)
- description and source-code
```javascript
function ProxyWriter(props) {
  var self = this
  if (!(self instanceof ProxyWriter)) {
    throw new Error('ProxyWriter must be called as constructor.')
  }

  self.props = props
  self._needDrain = false

  Writer.call(self, props)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```



# <a name="apidoc.module.fstream.ProxyReader"></a>[module fstream.ProxyReader](#apidoc.module.fstream.ProxyReader)

#### <a name="apidoc.element.fstream.ProxyReader.ProxyReader"></a>[function <span class="apidocSignatureSpan">fstream.</span>ProxyReader (props)](#apidoc.element.fstream.ProxyReader.ProxyReader)
- description and source-code
```javascript
function ProxyReader(props) {
  var self = this
  if (!(self instanceof ProxyReader)) {
    throw new Error('ProxyReader must be called as constructor.')
  }

  self.props = props
  self._buffer = []
  self.ready = false

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyReader.super_"></a>[function <span class="apidocSignatureSpan">fstream.ProxyReader.</span>super_ (props, currentStat)](#apidoc.element.fstream.ProxyReader.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.ProxyReader.prototype"></a>[module fstream.ProxyReader.prototype](#apidoc.module.fstream.ProxyReader.prototype)

#### <a name="apidoc.element.fstream.ProxyReader.prototype._addProxy"></a>[function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>_addProxy (proxy)](#apidoc.element.fstream.ProxyReader.prototype._addProxy)
- description and source-code
```javascript
_addProxy = function (proxy) {
  var self = this
  if (self._proxyTarget) {
    return self.error('proxy already set')
  }

  self._proxyTarget = proxy
  proxy._proxy = self

  ;[
    'error',
    'data',
    'end',
    'close',
    'linkpath',
    'entry',
    'entryEnd',
    'child',
    'childEnd',
    'warn',
    'stat'
  ].forEach(function (ev) {
    // console.error('~~ proxy event', ev, self.path)
    proxy.on(ev, self.emit.bind(self, ev))
  })

  self.emit('proxy', proxy)

  proxy.on('ready', function () {
    // console.error("~~ proxy is ready!", self.path)
    self.ready = true
    self.emit('ready')
  })

  var calls = self._buffer
  self._buffer.length = 0
  calls.forEach(function (c) {
    proxy[c[0]].apply(proxy, c[1])
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyReader.prototype._stat"></a>[function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>_stat ()](#apidoc.element.fstream.ProxyReader.prototype._stat)
- description and source-code
```javascript
_stat = function () {
  var self = this
  var props = self.props
  // stat the thing to see what the proxy should be.
  var stat = props.follow ? 'stat' : 'lstat'

  fs[stat](props.path, function (er, current) {
    var type
    if (er || !current) {
      type = 'File'
    } else {
      type = getType(current)
    }

    props[type] = true
    props.type = self.type = type

    self._old = current
    self._addProxy(Reader(props, current))
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyReader.prototype.pause"></a>[function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>pause ()](#apidoc.element.fstream.ProxyReader.prototype.pause)
- description and source-code
```javascript
pause = function () {
  return this._proxyTarget ? this._proxyTarget.pause() : false
}
```
- example usage
```shell
...

function collect (stream) {
if (stream._collected) return

if (stream._paused) return stream.on('resume', collect.bind(null, stream))

stream._collected = true
stream.pause()

stream.on('data', save)
stream.on('end', save)
var buf = []
function save (b) {
  if (typeof b === 'string') b = new Buffer(b)
  if (Buffer.isBuffer(b) && !b.length) return
...
```

#### <a name="apidoc.element.fstream.ProxyReader.prototype.resume"></a>[function <span class="apidocSignatureSpan">fstream.ProxyReader.prototype.</span>resume ()](#apidoc.element.fstream.ProxyReader.prototype.resume)
- description and source-code
```javascript
resume = function () {
  return this._proxyTarget ? this._proxyTarget.resume() : false
}
```
- example usage
```shell
...
        if (dest) stream.pipe(dest)

        buf.forEach(function (b) {
          if (b) stream.emit('data', b)
          else stream.emit('end')
        })

        stream.resume()
      }

      return dest
    }
  })(stream.pipe)
}
...
```



# <a name="apidoc.module.fstream.ProxyWriter"></a>[module fstream.ProxyWriter](#apidoc.module.fstream.ProxyWriter)

#### <a name="apidoc.element.fstream.ProxyWriter.ProxyWriter"></a>[function <span class="apidocSignatureSpan">fstream.</span>ProxyWriter (props)](#apidoc.element.fstream.ProxyWriter.ProxyWriter)
- description and source-code
```javascript
function ProxyWriter(props) {
  var self = this
  if (!(self instanceof ProxyWriter)) {
    throw new Error('ProxyWriter must be called as constructor.')
  }

  self.props = props
  self._needDrain = false

  Writer.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyWriter.super_"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.</span>super_ (props, current)](#apidoc.element.fstream.ProxyWriter.super_)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.ProxyWriter.prototype"></a>[module fstream.ProxyWriter.prototype](#apidoc.module.fstream.ProxyWriter.prototype)

#### <a name="apidoc.element.fstream.ProxyWriter.prototype._addProxy"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>_addProxy (proxy)](#apidoc.element.fstream.ProxyWriter.prototype._addProxy)
- description and source-code
```javascript
_addProxy = function (proxy) {
  // console.error("~~ set proxy", this.path)
  var self = this
  if (self._proxy) {
    return self.error('proxy already set')
  }

  self._proxy = proxy
  ;[
    'ready',
    'error',
    'close',
    'pipe',
    'drain',
    'warn'
  ].forEach(function (ev) {
    proxy.on(ev, self.emit.bind(self, ev))
  })

  self.emit('proxy', proxy)

  var calls = self._buffer
  calls.forEach(function (c) {
    // console.error("~~ ~~ proxy buffered call", c[0], c[1])
    proxy[c[0]].apply(proxy, c[1])
  })
  self._buffer.length = 0
  if (self._needsDrain) self.emit('drain')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyWriter.prototype._stat"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>_stat ()](#apidoc.element.fstream.ProxyWriter.prototype._stat)
- description and source-code
```javascript
_stat = function () {
  var self = this
  var props = self.props
  // stat the thing to see what the proxy should be.
  var stat = props.follow ? 'stat' : 'lstat'

  fs[stat](props.path, function (er, current) {
    var type
    if (er || !current) {
      type = 'File'
    } else {
      type = getType(current)
    }

    props[type] = true
    props.type = self.type = type

    self._old = current
    self._addProxy(Writer(props, current))
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.ProxyWriter.prototype.add"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>add (entry)](#apidoc.element.fstream.ProxyWriter.prototype.add)
- description and source-code
```javascript
add = function (entry) {
  // console.error("~~ proxy add")
  collect(entry)

  if (!this._proxy) {
    this._buffer.push(['add', [entry]])
    this._needDrain = true
    return false
  }
  return this._proxy.add(entry)
}
```
- example usage
```shell
...
// Once they're all done, then we can resume completely.
var e = 0
;(function unblockEntry () {
  var entry = entryBuffer[e++]
  // console.error(" ==== unblock entry", entry && entry.path)
  if (!entry) return resume()
  entry.on('end', unblockEntry)
  if (dest) dest.add(entry)
  else stream.emit('entry', entry)
})()

function resume () {
  stream.removeListener('entry', saveEntry)
  stream.removeListener('data', save)
  stream.removeListener('end', save)
...
```

#### <a name="apidoc.element.fstream.ProxyWriter.prototype.end"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>end (c)](#apidoc.element.fstream.ProxyWriter.prototype.end)
- description and source-code
```javascript
end = function (c) {
  // console.error('~~ proxy end')
  if (!this._proxy) {
    this._buffer.push(['end', [c]])
    return false
  }
  return this._proxy.end(c)
}
```
- example usage
```shell
...
'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.

'''javascript
...
```

#### <a name="apidoc.element.fstream.ProxyWriter.prototype.write"></a>[function <span class="apidocSignatureSpan">fstream.ProxyWriter.prototype.</span>write (c)](#apidoc.element.fstream.ProxyWriter.prototype.write)
- description and source-code
```javascript
write = function (c) {
  // console.error('~~ proxy write')
  if (!this._proxy) {
    this._buffer.push(['write', [c]])
    this._needDrain = true
    return false
  }
  return this._proxy.write(c)
}
```
- example usage
```shell
...

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.
...
```



# <a name="apidoc.module.fstream.Reader"></a>[module fstream.Reader](#apidoc.module.fstream.Reader)

#### <a name="apidoc.element.fstream.Reader.Reader"></a>[function <span class="apidocSignatureSpan">fstream.</span>Reader (props, currentStat)](#apidoc.element.fstream.Reader.Reader)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
...

So, for example, you can "write" a directory, and it'll call 'mkdir'.  You
can specify a uid and gid, and it'll call 'chown'.  You can specify a
'mtime' and 'atime', and it'll call 'utimes'.  You can call it a symlink
and provide a 'linkpath' and it'll call 'symlink'.

Note that it won't automatically resolve symbolic links.  So, if you
call 'fstream.Reader('/some/symlink')' then you'll get an object
that stats and then ends immediately (since it has no data).  To follow
symbolic links, do this: 'fstream.Reader({path:'/some/symlink', follow:
true })'.

There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.
...
```

#### <a name="apidoc.element.fstream.Reader.Dir"></a>[function <span class="apidocSignatureSpan">fstream.Reader.</span>Dir (props)](#apidoc.element.fstream.Reader.Dir)
- description and source-code
```javascript
function DirReader(props) {
  var self = this
  if (!(self instanceof DirReader)) {
    throw new Error('DirReader must be called as constructor.')
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    throw new Error('Non-directory type ' + props.type)
  }

  self.entries = null
  self._index = -1
  self._paused = false
  self._length = -1

  if (props.sort) {
    this.sort = props.sort
  }

  Reader.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.File"></a>[function <span class="apidocSignatureSpan">fstream.Reader.</span>File (props)](#apidoc.element.fstream.Reader.File)
- description and source-code
```javascript
function FileReader(props) {
  // console.error("    FR create", props.path, props.size, new Error().stack)
  var self = this
  if (!(self instanceof FileReader)) {
    throw new Error('FileReader must be called as constructor.')
  }

  // should already be established as a File type
  // XXX Todo: preserve hardlinks by tracking dev+inode+nlink,
  // with a HardLinkReader class.
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'File' && props.File))) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesEmitted = 0
  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.Link"></a>[function <span class="apidocSignatureSpan">fstream.Reader.</span>Link (props)](#apidoc.element.fstream.Reader.Link)
- description and source-code
```javascript
function LinkReader(props) {
  var self = this
  if (!(self instanceof LinkReader)) {
    throw new Error('LinkReader must be called as constructor.')
  }

  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.Proxy"></a>[function <span class="apidocSignatureSpan">fstream.Reader.</span>Proxy (props)](#apidoc.element.fstream.Reader.Proxy)
- description and source-code
```javascript
function ProxyReader(props) {
  var self = this
  if (!(self instanceof ProxyReader)) {
    throw new Error('ProxyReader must be called as constructor.')
  }

  self.props = props
  self._buffer = []
  self.ready = false

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.super_"></a>[function <span class="apidocSignatureSpan">fstream.Reader.</span>super_ ()](#apidoc.element.fstream.Reader.super_)
- description and source-code
```javascript
function Abstract() {
  Stream.call(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.Reader.prototype"></a>[module fstream.Reader.prototype](#apidoc.module.fstream.Reader.prototype)

#### <a name="apidoc.element.fstream.Reader.prototype._read"></a>[function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>_read ()](#apidoc.element.fstream.Reader.prototype._read)
- description and source-code
```javascript
_read = function () {
  this.error('Cannot read unknown type: ' + this.type)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.prototype._stat"></a>[function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>_stat (currentStat)](#apidoc.element.fstream.Reader.prototype._stat)
- description and source-code
```javascript
_stat = function (currentStat) {
  var self = this
  var props = self.props
  var stat = props.follow ? 'stat' : 'lstat'
  // console.error("Reader._stat", self._path, currentStat)
  if (currentStat) process.nextTick(statCb.bind(null, null, currentStat))
  else fs[stat](self._path, statCb)

  function statCb (er, props_) {
    // console.error("Reader._stat, statCb", self._path, props_, props_.nlink)
    if (er) return self.error(er)

    Object.keys(props_).forEach(function (k) {
      props[k] = props_[k]
    })

    // if it's not the expected size, then abort here.
    if (undefined !== self.size && props.size !== self.size) {
      return self.error('incorrect size')
    }
    self.size = props.size

    var type = getType(props)
    var handleHardlinks = props.hardlinks !== false

    // special little thing for handling hardlinks.
    if (handleHardlinks && type !== 'Directory' && props.nlink && props.nlink > 1) {
      var k = props.dev + ':' + props.ino
      // console.error("Reader has nlink", self._path, k)
      if (hardLinks[k] === self._path || !hardLinks[k]) {
        hardLinks[k] = self._path
      } else {
        // switch into hardlink mode.
        type = self.type = self.props.type = 'Link'
        self.Link = self.props.Link = true
        self.linkpath = self.props.linkpath = hardLinks[k]
        // console.error("Hardlink detected, switching mode", self._path, self.linkpath)
        // Setting __proto__ would arguably be the "correct"
        // approach here, but that just seems too wrong.
        self._stat = self._read = LinkReader.prototype._read
      }
    }

    if (self.type && self.type !== type) {
      self.error('Unexpected type: ' + type)
    }

    // if the filter doesn't pass, then just skip over this one.
    // still have to emit end so that dir-walking can move on.
    if (self.filter) {
      var who = self._proxy || self
      // special handling for ProxyReaders
      if (!self.filter.call(who, who, props)) {
        if (!self._disowned) {
          self.abort()
          self.emit('end')
          self.emit('close')
        }
        return
      }
    }

    // last chance to abort or disown before the flow starts!
    var events = ['_stat', 'stat', 'ready']
    var e = 0
    ;(function go () {
      if (self._aborted) {
        self.emit('end')
        self.emit('close')
        return
      }

      if (self._paused && self.type !== 'Directory') {
        self.once('resume', go)
        return
      }

      var ev = events[e++]
      if (!ev) {
        return self._read()
      }
      self.emit(ev, props)
      go()
    })()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Reader.prototype.pause"></a>[function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>pause (who)](#apidoc.element.fstream.Reader.prototype.pause)
- description and source-code
```javascript
pause = function (who) {
  this._paused = true
  who = who || this
  this.emit('pause', who)
  if (this._stream) this._stream.pause(who)
}
```
- example usage
```shell
...

function collect (stream) {
if (stream._collected) return

if (stream._paused) return stream.on('resume', collect.bind(null, stream))

stream._collected = true
stream.pause()

stream.on('data', save)
stream.on('end', save)
var buf = []
function save (b) {
  if (typeof b === 'string') b = new Buffer(b)
  if (Buffer.isBuffer(b) && !b.length) return
...
```

#### <a name="apidoc.element.fstream.Reader.prototype.pipe"></a>[function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>pipe (dest)](#apidoc.element.fstream.Reader.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest) {
  var self = this
  if (typeof dest.add === 'function') {
    // piping to a multi-compatible, and we've got directory entries.
    self.on('entry', function (entry) {
      var ret = dest.add(entry)
      if (ret === false) {
        self.pause()
      }
    })
  }

  // console.error("R Pipe apply Stream Pipe")
  return Stream.prototype.pipe.apply(this, arguments)
}
```
- example usage
```shell
...

Note that the linkpath is relative to the symbolic link location, not
the parent dir or cwd.

'''javascript
fstream
  .Reader("path/to/dir")
  .pipe(fstream.Writer("path/to/other/dir"))
'''

This will do like 'cp -Rp path/to/dir path/to/other/dir'.  If the other
dir exists and isn't a directory, then it'll emit an error.  It'll also
set the uid, gid, mode, etc. to be identical.  In this way, it's more
like 'rsync -a' than simply a copy.
...
```

#### <a name="apidoc.element.fstream.Reader.prototype.resume"></a>[function <span class="apidocSignatureSpan">fstream.Reader.prototype.</span>resume (who)](#apidoc.element.fstream.Reader.prototype.resume)
- description and source-code
```javascript
resume = function (who) {
  this._paused = false
  who = who || this
  this.emit('resume', who)
  if (this._stream) this._stream.resume(who)
  this._read()
}
```
- example usage
```shell
...
        if (dest) stream.pipe(dest)

        buf.forEach(function (b) {
          if (b) stream.emit('data', b)
          else stream.emit('end')
        })

        stream.resume()
      }

      return dest
    }
  })(stream.pipe)
}
...
```



# <a name="apidoc.module.fstream.Writer"></a>[module fstream.Writer](#apidoc.module.fstream.Writer)

#### <a name="apidoc.element.fstream.Writer.Writer"></a>[function <span class="apidocSignatureSpan">fstream.</span>Writer (props, current)](#apidoc.element.fstream.Writer.Writer)
- description and source-code
```javascript
function Writer(props, current) {
  var self = this

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Writer(dir) to get a DirWriter object, etc.
  var type = getType(props)
  var ClassType = Writer

  switch (type) {
    case 'Directory':
      ClassType = DirWriter
      break
    case 'File':
      ClassType = FileWriter
      break
    case 'Link':
    case 'SymbolicLink':
      ClassType = LinkWriter
      break
    case null:
    default:
      // Don't know yet what type to create, so we wrap in a proxy.
      ClassType = ProxyWriter
      break
  }

  if (!(self instanceof ClassType)) return new ClassType(props)

  // now get down to business.

  Abstract.call(self)

  if (!props.path) self.error('Must provide a path', null, true)

  // props is what we want to set.
  // set some convenience properties as well.
  self.type = props.type
  self.props = props
  self.depth = props.depth || 0
  self.clobber = props.clobber === false ? props.clobber : true
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      self._swallowErrors = true
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    }
  }
  self.basename = path.basename(props.path)
  self.dirname = path.dirname(props.path)
  self.linkpath = props.linkpath || null

  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size

  if (typeof props.mode === 'string') {
    props.mode = parseInt(props.mode, 8)
  }

  self.readable = false
  self.writable = true

  // buffer until ready, or while handling another entry
  self._buffer = []
  self.ready = false

  self.filter = typeof props.filter === 'function' ? props.filter : null

  // start the ball rolling.
  // this checks what's there already, and then calls
  // self._create() to call the impl-specific creation stuff.
  self._stat(current)
}
```
- example usage
```shell
...
There are various checks to make sure that the bytes emitted are the
same as the intended size, if the size is set.

## Examples

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''
...
```

#### <a name="apidoc.element.fstream.Writer.Dir"></a>[function <span class="apidocSignatureSpan">fstream.Writer.</span>Dir (props)](#apidoc.element.fstream.Writer.Dir)
- description and source-code
```javascript
function DirWriter(props) {
  var self = this
  if (!(self instanceof DirWriter)) {
    self.error('DirWriter must be called as constructor.', null, true)
  }

  // should already be established as a Directory type
  if (props.type !== 'Directory' || !props.Directory) {
    self.error('Non-directory type ' + props.type + ' ' +
      JSON.stringify(props), null, true)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.File"></a>[function <span class="apidocSignatureSpan">fstream.Writer.</span>File (props)](#apidoc.element.fstream.Writer.File)
- description and source-code
```javascript
function FileWriter(props) {
  var self = this
  if (!(self instanceof FileWriter)) {
    throw new Error('FileWriter must be called as constructor.')
  }

  // should already be established as a File type
  if (props.type !== 'File' || !props.File) {
    throw new Error('Non-file type ' + props.type)
  }

  self._buffer = []
  self._bytesWritten = 0

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.Link"></a>[function <span class="apidocSignatureSpan">fstream.Writer.</span>Link (props)](#apidoc.element.fstream.Writer.Link)
- description and source-code
```javascript
function LinkWriter(props) {
  var self = this
  if (!(self instanceof LinkWriter)) {
    throw new Error('LinkWriter must be called as constructor.')
  }

  // should already be established as a Link type
  if (!((props.type === 'Link' && props.Link) ||
    (props.type === 'SymbolicLink' && props.SymbolicLink))) {
    throw new Error('Non-link type ' + props.type)
  }

  if (props.linkpath === '') props.linkpath = '.'
  if (!props.linkpath) {
    self.error('Need linkpath property to create ' + props.type)
  }

  Writer.call(this, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.Proxy"></a>[function <span class="apidocSignatureSpan">fstream.Writer.</span>Proxy (props)](#apidoc.element.fstream.Writer.Proxy)
- description and source-code
```javascript
function ProxyWriter(props) {
  var self = this
  if (!(self instanceof ProxyWriter)) {
    throw new Error('ProxyWriter must be called as constructor.')
  }

  self.props = props
  self._needDrain = false

  Writer.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.super_"></a>[function <span class="apidocSignatureSpan">fstream.Writer.</span>super_ ()](#apidoc.element.fstream.Writer.super_)
- description and source-code
```javascript
function Abstract() {
  Stream.call(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.Writer.prototype"></a>[module fstream.Writer.prototype](#apidoc.module.fstream.Writer.prototype)

#### <a name="apidoc.element.fstream.Writer.prototype._create"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_create ()](#apidoc.element.fstream.Writer.prototype._create)
- description and source-code
```javascript
_create = function () {
  var self = this
  fs[self.props.follow ? 'stat' : 'lstat'](self._path, function (er) {
    if (er) {
      return self.warn('Cannot create ' + self._path + '\n' +
        'Unsupported type: ' + self.type, 'ENOTSUP')
    }
    self._finish()
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.prototype._finish"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_finish ()](#apidoc.element.fstream.Writer.prototype._finish)
- description and source-code
```javascript
_finish = function () {
  var self = this

  if (self._finishing) return
  self._finishing = true

  // console.error(" W Finish", self._path, self.size)

  // set up all the things.
  // At this point, we're already done writing whatever we've gotta write,
  // adding files to the dir, etc.
  var todo = 0
  var errState = null
  var done = false

  if (self._old) {
    // the times will almost *certainly* have changed.
    // adds the utimes syscall, but remove another stat.
    self._old.atime = new Date(0)
    self._old.mtime = new Date(0)
    // console.error(" W Finish Stale Stat", self._path, self.size)
    setProps(self._old)
  } else {
    var stat = self.props.follow ? 'stat' : 'lstat'
    // console.error(" W Finish Stating", self._path, self.size)
    fs[stat](self._path, function (er, current) {
      // console.error(" W Finish Stated", self._path, self.size, current)
      if (er) {
        // if we're in the process of writing out a
        // directory, it's very possible that the thing we're linking to
        // doesn't exist yet (especially if it was intended as a symlink),
        // so swallow ENOENT errors here and just soldier on.
        if (er.code === 'ENOENT' &&
          (self.type === 'Link' || self.type === 'SymbolicLink') &&
          process.platform === 'win32') {
          self.ready = true
          self.emit('ready')
          self.emit('end')
          self.emit('close')
          self.end = self._finish = function () {}
          return
        } else return self.error(er)
      }
      setProps(self._old = current)
    })
  }

  return

  function setProps (current) {
    todo += 3
    endChmod(self, self.props, current, self._path, next('chmod'))
    endChown(self, self.props, current, self._path, next('chown'))
    endUtimes(self, self.props, current, self._path, next('utimes'))
  }

  function next (what) {
    return function (er) {
      // console.error("   W Finish", what, todo)
      if (errState) return
      if (er) {
        er.fstream_finish_call = what
        return self.error(errState = er)
      }
      if (--todo > 0) return
      if (done) return
      done = true

      // we may still need to set the mode/etc. on some parent dirs
      // that were created previously.  delay end/close until then.
      if (!self._madeDir) return end()
      else endMadeDir(self, self._path, end)

      function end (er) {
        if (er) {
          er.fstream_finish_call = 'setupMadeDir'
          return self.error(er)
        }
        // all the props have been set, so we're completely done.
        self.emit('end')
        self.emit('close')
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.prototype._stat"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>_stat (current)](#apidoc.element.fstream.Writer.prototype._stat)
- description and source-code
```javascript
_stat = function (current) {
  var self = this
  var props = self.props
  var stat = props.follow ? 'stat' : 'lstat'
  var who = self._proxy || self

  if (current) statCb(null, current)
  else fs[stat](self._path, statCb)

  function statCb (er, current) {
    if (self.filter && !self.filter.call(who, who, current)) {
      self._aborted = true
      self.emit('end')
      self.emit('close')
      return
    }

    // if it's not there, great.  We'll just create it.
    // if it is there, then we'll need to change whatever differs
    if (er || !current) {
      return create(self)
    }

    self._old = current
    var currentType = getType(current)

    // if it's a type change, then we need to clobber or error.
    // if it's not a type change, then let the impl take care of it.
    if (currentType !== self.type) {
      return rimraf(self._path, function (er) {
        if (er) return self.error(er)
        self._old = null
        create(self)
      })
    }

    // otherwise, just handle in the app-specific way
    // this creates a fs.WriteStream, or mkdir's, or whatever
    create(self)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.Writer.prototype.add"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>add ()](#apidoc.element.fstream.Writer.prototype.add)
- description and source-code
```javascript
add = function () {
  this.error("Can't add to non-Directory type")
}
```
- example usage
```shell
...
// Once they're all done, then we can resume completely.
var e = 0
;(function unblockEntry () {
  var entry = entryBuffer[e++]
  // console.error(" ==== unblock entry", entry && entry.path)
  if (!entry) return resume()
  entry.on('end', unblockEntry)
  if (dest) dest.add(entry)
  else stream.emit('entry', entry)
})()

function resume () {
  stream.removeListener('entry', saveEntry)
  stream.removeListener('data', save)
  stream.removeListener('end', save)
...
```

#### <a name="apidoc.element.fstream.Writer.prototype.pipe"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>pipe ()](#apidoc.element.fstream.Writer.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.error("Can't pipe from writable stream")
}
```
- example usage
```shell
...

Note that the linkpath is relative to the symbolic link location, not
the parent dir or cwd.

'''javascript
fstream
  .Reader("path/to/dir")
  .pipe(fstream.Writer("path/to/other/dir"))
'''

This will do like 'cp -Rp path/to/dir path/to/other/dir'.  If the other
dir exists and isn't a directory, then it'll emit an error.  It'll also
set the uid, gid, mode, etc. to be identical.  In this way, it's more
like 'rsync -a' than simply a copy.
...
```

#### <a name="apidoc.element.fstream.Writer.prototype.write"></a>[function <span class="apidocSignatureSpan">fstream.Writer.prototype.</span>write ()](#apidoc.element.fstream.Writer.prototype.write)
- description and source-code
```javascript
write = function () {
  return true
}
```
- example usage
```shell
...

'''javascript
fstream
  .Writer({ path: "path/to/file"
          , mode: 0755
          , size: 6
          })
  .write("hello\n")
  .end()
'''

This will create the directories if they're missing, and then write
'hello\n' into the file, chmod it to 0755, and assert that 6 bytes have
been written when it's done.
...
```



# <a name="apidoc.module.fstream.socket_reader"></a>[module fstream.socket_reader](#apidoc.module.fstream.socket_reader)

#### <a name="apidoc.element.fstream.socket_reader.socket_reader"></a>[function <span class="apidocSignatureSpan">fstream.</span>socket_reader (props)](#apidoc.element.fstream.socket_reader.socket_reader)
- description and source-code
```javascript
function SocketReader(props) {
  var self = this
  if (!(self instanceof SocketReader)) {
    throw new Error('SocketReader must be called as constructor.')
  }

  if (!(props.type === 'Socket' && props.Socket)) {
    throw new Error('Non-socket type ' + props.type)
  }

  Reader.call(self, props)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fstream.socket_reader.super_"></a>[function <span class="apidocSignatureSpan">fstream.socket_reader.</span>super_ (props, currentStat)](#apidoc.element.fstream.socket_reader.super_)
- description and source-code
```javascript
function Reader(props, currentStat) {
  var self = this
  if (!(self instanceof Reader)) return new Reader(props, currentStat)

  if (typeof props === 'string') {
    props = { path: props }
  }

  // polymorphism.
  // call fstream.Reader(dir) to get a DirReader object, etc.
  // Note that, unlike in the Writer case, ProxyReader is going
  // to be the *normal* state of affairs, since we rarely know
  // the type of a file prior to reading it.

  var type
  var ClassType

  if (props.type && typeof props.type === 'function') {
    type = props.type
    ClassType = type
  } else {
    type = getType(props)
    ClassType = Reader
  }

  if (currentStat && !type) {
    type = getType(currentStat)
    props[type] = true
    props.type = type
  }

  switch (type) {
    case 'Directory':
      ClassType = require('./dir-reader.js')
      break

    case 'Link':
    // XXX hard links are just files.
    // However, it would be good to keep track of files' dev+inode
    // and nlink values, and create a HardLinkReader that emits
    // a linkpath value of the original copy, so that the tar
    // writer can preserve them.
    // ClassType = HardLinkReader
    // break

    case 'File':
      ClassType = require('./file-reader.js')
      break

    case 'SymbolicLink':
      ClassType = LinkReader
      break

    case 'Socket':
      ClassType = require('./socket-reader.js')
      break

    case null:
      ClassType = require('./proxy-reader.js')
      break
  }

  if (!(self instanceof ClassType)) {
    return new ClassType(props)
  }

  Abstract.call(self)

  if (!props.path) {
    self.error('Must provide a path', null, true)
  }

  self.readable = true
  self.writable = false

  self.type = type
  self.props = props
  self.depth = props.depth = props.depth || 0
  self.parent = props.parent || null
  self.root = props.root || (props.parent && props.parent.root) || self

  self._path = self.path = path.resolve(props.path)
  if (process.platform === 'win32') {
    self.path = self._path = self.path.replace(/\?/g, '_')
    if (self._path.length >= 260) {
      // how DOES one create files on the moon?
      // if the path has spaces in it, then UNC will fail.
      self._swallowErrors = true
      // if (self._path.indexOf(" ") === -1) {
      self._path = '\\\\?\\' + self.path.replace(/\//g, '\\')
    // }
    }
  }
  self.basename = props.basename = path.basename(self.path)
  self.dirname = props.dirname = path.dirname(self.path)

  // these have served their purpose, and are now just noisy clutter
  props.parent = props.root = null

  // console.error("\n\n\n%s setting size to", props.path, props.size)
  self.size = props.size
  self.filter = typeof props.filter === 'function' ? props.filter : null
  if (props.sort === 'alpha') props.sort = alphasort

  // start the ball rolling.
  // this will stat the thing, and then call self._read()
  // to start reading whatever it is.
  // console.error("calling stat", props.path, currentStat)
  self._stat(currentStat)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fstream.socket_reader.prototype"></a>[module fstream.socket_reader.prototype](#apidoc.module.fstream.socket_reader.prototype)

#### <a name="apidoc.element.fstream.socket_reader.prototype._read"></a>[function <span class="apidocSignatureSpan">fstream.socket_reader.prototype.</span>_read ()](#apidoc.element.fstream.socket_reader.prototype._read)
- description and source-code
```javascript
_read = function () {
  var self = this
  if (self._paused) return
  // basically just a no-op, since we got all the info we have
  // from the _stat method
  if (!self._ended) {
    self.emit('end')
    self.emit('close')
    self._ended = true
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
