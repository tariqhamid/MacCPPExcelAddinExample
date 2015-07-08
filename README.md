# MacCPPExcelPluginExample

Mac OSX Excel plugin consisting of three components, the plugin, a main program and an excel spreadsheet using the plugin.

There are three CDT projects in this repo
* MacExampleAddin cpp - uses CDT and clang to build the dylib
* MacExampleMain cpp - uses CDT and clang to build the main and references dylib
* MacExampleExcel excel - an example spreadsheet that uses the addin, via VBA not directly
** The excel absoulute paths need to changed for this to work in your environment

## Install
Clone the repo into an Eclipse CDT workspace and import the projects into Eclipse
cmd-B will build all of the projects

The dylib local to the Excel spreadsheet directory has to be manually copied when the dylib changes

The absoluate paths in the spreadsheet need to be changed to refere to your path in the VBA module
