# Go Beam

this is a simple wordcount program using the apache beam go examples.

## Notes:
- Was initially unable to `go install` using the original command in the beam getting started documentation
- - needed to run `go get -u github.com/apache/beam/sdks/v2/go/pkg/beam/io/filesystem/gcs@v2.37.0` first
- Visual Studio Code will throw errors on both go files, this is due to both files using package main and containing a main function. Go is designed for one project per folder, so you are expected to run `go build` in the root folder. Attempting to do so will throw a main redeclaration error. If you want to build these files, you *must* specify which file to build by using `go build [file]`.
