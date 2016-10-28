```VBA
Function GetURL(cell As range, _
Optional default_value As Variant)
'Lists the Hyperlink Address for a Given Cell
'If cell does not contain a hyperlink, return default_value
If (cell.range("A1").Hyperlinks.Count <> 1) Then
GetURL = default_value
Else
GetURL = cell.range("A1").Hyperlinks(1).Address & "#" & cell.range("A1").Hyperlinks(1).SubAddress
End If
End Function
```
