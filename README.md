# WixToolset-Tutorials

A collection of tutorials for the [Wix Toolset][Wix Toolset], which include a bunch of samples and examples.  

Wix toolset (v3 and v4) is the tool to create:

* Modern `MSI` setups for the Windows Installer
* Boostrapper `EXE` installer to handle prerequisites
* Custom Actions to write your own C# code inside the Windows Installer

Slogan from the official Website:
> THE MOST POWERFUL SET OF TOOLS AVAILABLE TO CREATE YOUR WINDOWS INSTALLATION EXPERIENCE.

A MSI can be inspected by the tool **Orca** from Microsoft ([Orca - Documenation][Orca - Documenation]), which is part of the Windows Installer SDK and installed at `C:\Program Files (x86)\Orca\Orca.exe`. As an Alternative there is also [SuperOrca][SuperOrca] which is **NOT** from Microsoft.

## Wix Toolset Extensions

Wix Toolset Extensions are stored inside `C:\Program Files (x86)\WiX Toolset v3.11\bin` (replace the version v3.11 with your version) as `.dll` and can be used as references inside your project.  

| Name           | Description                                                                                                              |
| -------------- | ------------------------------------------------------------------------------------------------------------------------ |
| [WixUIExtension][GitHub WixUIExtension] | UI Dialoges, [UIRef][Wix Toolset UIRef], e.g. WixUI_Advanced, WixUI_FeatureTree and WixUI_Mondo |

## History

1. Create the project on [GitHub][GitHub WixToolset-Tutorials] inside the "n13.org - Open-Source by [KargWare][KargWare Website]"
1. Change UI sequence [UIRef][Wix Toolset UIRef] from `WixUI_Minimal` to `WixUI_Advanced`
1. Use [Wix-Variables][Wix Toolset Wix-Variables] to avoid repeating your self many times, extract version to separate WXI file
1. Add a customized dialog `PrerequisitesDlg` to the default `WixUI_FeatureTree` UI. It is also shared as a [GitHub Gist][GitHub Gist PrerequisitesDlg]. The branch [features/AddPrerequisitesPage][GitHub WixToolset-Tutorials branch AddPrerequisitesPage] will stay.

[KargWare Website]: https://kargware.com
[KargWare Notes]: https://notes.kargware.com
[GitHub WixToolset-Tutorials]: https://github.com/n13org/WixToolset-Tutorials
[GitHub WixToolset-Tutorials branch AddPrerequisitesPage]: https://github.com/n13org/WixToolset-Tutorials/tree/features/AddPrerequisitesPage
[GitHub Gist PrerequisitesDlg]: https://gist.github.com/N7K4/8b146328db03484a61543c4f612c5dd3
[Wix Toolset]: http://wixtoolset.org/
[Wix Toolset UIRef]: https://wixtoolset.org/documentation/manual/v3/xsd/wix/uiref.html
[Wix Toolset Wix-Variables]: https://wixtoolset.org/documentation/manual/v3/votive/votive_project_references.html
[Orca - Documenation]: https://docs.microsoft.com/en-us/windows/win32/msi/orca-exe
[SuperOrca]: http://www.pantaray.com/msi_super_orca.html
[GitHub WixUIExtension]: https://github.com/wixtoolset/wix3/tree/develop/src/ext/UIExtension/wixlib
