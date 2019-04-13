## Welcome
This is the landing page for the open source projects by Richard e Collins.

[#appbuild](https://hamandeggs.github.io/appbuild/)
This is an alternative to using make as a tool for creating c/c++ applications in Linux. It uses just one configuration for per project which can reference other projects files to create a solution. The project files are written using [json](http://json.org/) so that IDE's and other editors can use the files with their own customisations without effecting the build process.

* appbuild supports
    * Targets applications and static libraries.
    * Full dependency checking.
    * Project references, if an app refers to a library and the source of that library has changed it will build that library before continuing with building the application, just as you would expect. 
    * Multithread compiling.
    * Builtin build environment defines to help with build time and version generation.
    * Single process used during entire build process that allows for increased speed of dependency checking between source files.
    * Does not create extra files to manage the project and so will not clutter up your repository. Just uses the **one** project file for each project.
    * Resource file support with file API and compression, think something like res folder for Android apps.
    * Json file format allowing intergration with external editors where the editor can add it’s own values to the file and the tool will ignore them.
    * Can be used as a shebang in a c/c++ file so that this source file is now execuatable. As if it was a shell script.
