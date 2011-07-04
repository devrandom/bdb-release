# Bitcoin Releases

This directory contains bitcoin Gitian build results, signed by multiple people.

The layout of this directory is:

    <release-name>/
      <signer>/
        bdb-build.assert - the result file produced by the signer's build process
        bdb-build.assert.sig - the signer's signature certifying the result

This directory is created by the Gitian `gsign` command, after a successful `gbuild`.  It can be verified with `gverify`.

The source is db4.7\_4.7.25.orig.tar.gz obtained with `apt-get source db4.7` on Ubuntu Natty.

Normally, all output manifests in the result files should be identical between different signers.

See also:

* [Gitian builder](https://github.com/devrandom/gitian-builder)
