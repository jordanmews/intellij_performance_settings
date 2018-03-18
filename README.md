# intellij_performance_settings
Intellij IDE configurations for high-performance.
VMoptions and properties files are directly usable in the IDE, assuming your hardware can handle it.
- To add to the IDE: Help -> Edit Custom Properties / Edit Custom VM Options

# More Performance tips: 
## System 
- IDEA is heavily IO-bound 
- Do not store sources, caches or system directories on network drives 
- Disable antivirus scanning for system directory 
- Regularly run disk defragmenter 
- Turn off Windows System Restore 

## JVM 
- In –server mode, increasing –Xmx helps IDEA’s caches live longer 
- Parallel GC helps on multicore machines but may cause stability issues

## IDE 
- Use latest version 
- Disable unused plugins 
- Exclude unneeded folders 
- Set version control to None for generated code 
- Avoid large number of unversioned files 
- Do not disable “Synchronize files on frame activation” 
- Switch Project view to “Project” rather than “Packages” 
- Disable expensive inspections 
- Disable framework-specific validation on Make 
- Do not use method breakpoints 

*source - https://www.slideshare.net/intelliyole/intellij-idea-architecture-and-performance*

## More info and other useful links
- [Automating Sharing of IDE Settings](https://www.jetbrains.com/help/idea/sharing-your-ide-settings.html#settings-repository)
- [Configuring JVM options and platform properties](https://intellij-support.jetbrains.com/hc/en-us/articles/206544869-Configuring-JVM-options-and-platform-properties)
- [Common JVM options used with Intellij and what they do](https://github.com/FoxxMD/intellij-jvm-options-explained)
- [Directories used by the IDE to store settings, caches, plugins and logs ]( https://intellij-support.jetbrains.com/hc/en-us/articles/206544519)
