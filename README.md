#StyleCop.MSBuild Bug

This project will fail to compile on Mono because the StyleCop.MSBuild target cannot resolve the relative path:

``..\packages\StyleCop.MSBuild.4.7.49.1\build\StyleCop.MSBuild.Targets

The packages folder is one level above the project folder and it was created by checking the option "Create Solution folder" in Visual Studio.