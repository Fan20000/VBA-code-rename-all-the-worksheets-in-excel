# VBA-code-rename-all-the-worksheets-in-excel

Sub ChangeWorkSheetName()
'Updateby20140624
Dim Rng As Range
Dim WorkRng As Range
On Error Resume Next
xTitleId = "KutoolsforExcel"
newName = Application.InputBox("Name", xTitleId, "", Type:=2)
For i = 1 To Application.Sheets.Count
Application.Sheets(i).Name = newName & i
Next
End Sub
