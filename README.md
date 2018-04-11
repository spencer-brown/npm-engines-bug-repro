# `engines` test

It seems that `npm` is not enforcing the `engines` requirement in `package.json`.

To repro, run `npm i` and observe that the installation succeeds without warning, despite
`package.json` requiring that your `npm` version should be `>999` (which is not satisifed by any
available npm version).
