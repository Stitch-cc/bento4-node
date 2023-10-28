# bento4-node
This is a simple bento4 installer node module. The bento4 binaries is installed with the module and provides paths to them.

This package is an updated version of [bento4-installer](https://www.npmjs.com/package/bento4-installer). It was created because the author of bento4-installer has not updated the package or attended to pull request for a while.

## Installation
```js
npm i --save bento4-node
```

## Usage
When the `bento4-installer` is required, as seen below, it returns an object that has the paths to the platform specific executables.

```js
const bento4 = require('bento4-node')
```
The bento4 object returned has the following properties:

```
{
  /* The path to the bento4 bin folder */
  binPath,

  /* The path to the executables */
  aac2mp4,
  mp42avc,
  mp42hevc,
  mp42hls,
  mp42ts,
  mp4compact,
  mp4dash,
  mp4dashclone,
  mp4dcfpackager
  mp4decrypt,
  mp4dump,
  mp4edit,
  mp4encrypt,
  mp4extract,
  mp4fragment,
  mp4hls,
  mp4info,
  mp4mux,
  mp4rtphintinfo,
  mp4split,
  mp4tag,

  /* The current version of this module */
  version,

  /* Is set to true if the OS platform and architecture is supported */
  isPlatformSupported,

  /* Is set to a string with the OS platform and architecture in the following format: <platform>-<architecture>, for example, 'darwin-x64' */
  platform
}
```
See [bento4.com](https://www.bento4.com/) for information on how to use the bento4 executables.
