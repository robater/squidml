# squidml
@echo off

title Computer Search

IF NOT EXIST %userprofile%\Desktop\Results mkdir %userprofile%\Desktop\Results
dir C:\ /A:D /A:A /O:-D /Q /R /S /T:C /4 | find "2015" | find "BUILTIN" > %userprofile%\Desktop\Results\ProgramFilesSearch.txt
dir C:\ /A:D /A:A /O:-D /Q /R /S /T:C /4 | find "2015" | find "..." >> %userprofile%\Desktop\Results\ProgramFilesSearch.txt
echo Results have been sucessfully saved, these are the results:
dir C:\ /A:D /A:A /O:-D /Q /R /S /T:C /4 | find "2015" | find "BUILTIN"
dir C:\ /A:D /A:A /O:-D /Q /R /S /T:C /4 | find "2015" | find "..."
pause 
