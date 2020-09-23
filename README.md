<div align="center">

## Form in popup targets parent


</div>

### Description

popup window how can I submit a form, close the popup window and target the results of the form into the main window?

Found at: http://www.irt.org
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Found on the Web](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/found-on-the-web.md)
**Level**          |Unknown
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |
**Category**       |[Windows](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows__2-80.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/found-on-the-web-form-in-popup-targets-parent__2-232/archive/master.zip)





### Source Code

```
Use a timer to close the window, and add a TARGET to the form:
<FORM ACTION="apage.html" TARGET="mywindowname" onSubmit="setTimeout('window.close',2000)">
<INPUT TYPE="SUBMIT">
</FORM>
Now make sure that in the main window you set its name (by default the main window has no name):
<SCRIPT LANGUAGE="JavaScript"><!--
window.name="mywindowname"; // will not work in NN2 as name is read only
//--></SCRIPT>
```

