## Welcome
This is the landing page for the open source projects by Richard e Collins.

[#appbuild](https://hamandeggs.github.io/appbuild/)
This is an alternative to using make as a tool for creating c/c++ applications in Linux. It uses just one configuration for per project which can reference other projects files to create a solution. The project files are written using [json](http://json.org/) so that IDE's and other editors can use the files with their own customisations without effecting the build process.

* appbuild supports
  * Full **dependacy** checking.
  * Project references and automaic building of these references when needed.
  * Multithread compiling.
  * Builtin build environment defines to help with build time and version generation.
  * Single process used during entire build process that allows for increased speed of dependency checking between source files.
  * Does not create extra files to manage the project and so will not clutter up your repository. Just uses the **one** project file for each project.
  * Resource file support with file API and compression, think something like res folder for Android apps.

