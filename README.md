# aosp7.1-dior
Local manifest for building AOSP 7.1 for the Redmi Note 4G

## To use this local manifest:

### If you have _not_ added _any_ other local manifests, it's pretty straightforward.
Assuming you're in your Android source directory(where you see folders like 'art' and 'build'), first do:
`cd .repo`
Next, do this:
`git clone https://github.com/haoyangw/local_manifests.git local_manifests`
And then you're done! Just do a `repo sync` next time and everything will be set up nicely! :)

### If you _have_ added other local manifests, it gets a little more complicated. :(
First, do this in the Android source directory(assuming local_manifests is _not already_ a git repository):
`cd .repo/local_manifests`
Next, do the following:
`git init`
`git remote add why https://github.com/haoyangw/local_manifests.git`
`git fetch why aosp7.1-dior`
And then the next time you do a `repo sync`, everything will be set up nicely! :)
