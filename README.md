<div align="center">

## Popup Menu


</div>

### Description

Popup is shown when the user moves the mouse over the link. This colorful popup is a great way toi provide additional info like help or 'tool-tips' regarding any link or image!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mike McGrath](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mike-mcgrath.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mike-mcgrath-popup-menu__2-1783/archive/master.zip)





### Source Code

```
<!-- Script tested on PC platform in IE5.0 and NN4.7 -->
<HTML>
<HEAD>
<TITLE>Popup Link Menu &copy; Mike McGrath 2000</TITLE>
<STYLE TYPE="text/css">
<!--
.lilguydiv {position:absolute;top:100;left:100;width:30;height:21;}
.menudiv {position:absolute;top:80;left:60;width:160;height:106;color:brown;background-color:white;border:solid;border-width:2;border-color:brown;z-index:10;visibility:hidden;}
//-->
</STYLE>
</HEAD>
<BODY BGCOLOR="silver">
Run your Mouse over the Lilguy for a Link Menu ...
<P>
<DIV CLASS="lilguydiv">
<A HREF="javascript:\\" ONMOUSEOVER="menu(1)">
<IMG BORDER="0" SRC="images/lilguy2.gif" WIDTH="30" HEIGHT="21"></A>
</DIV>
<DIV ID="linkmenu" CLASS="menudiv">
<CENTER><B>Select A Link</B></CENTER>
<UL>
<A HREF="javascript:fakelocation(1)"><LI>Link One</LI></A>
<A HREF="javascript:fakelocation(2)"><LI>Link Two</LI></A>
<A HREF="javascript:fakelocation(3)"><LI>Link Three</LI></A>
</UL>
</DIV>
<SCRIPT TYPE="text/javascript">
<!-- Original: Mike McGrath (mike_mcgrath@lineone.net) -->
<!-- Website : http://website.lineone.net/~mike_mcgrath -->
<!--
var nav=(document.layers);
if(nav)document.captureEvents(Event.MOUSEMOVE);
document.onmousemove=track;
function track(e)
{
 var x=(nav)?e.pageX:event.x;
 var y=(nav)?e.pageY:event.y;
 isvis(x,y);
}
function isvis(x,y)
{
 if(nav)
	{
	 if(document.linkmenu.visibility!="hide")
		{
		 if(x<60||x>220||y<80||y>166)document.linkmenu.visibility="hide";
		}
	}
	else if(linkmenu.style.visibility!="hidden")
	{
	 if(x<60||x>220||y<80||y>186)linkmenu.style.visibility="hidden";
	}
}
function menu(n)
{
 if(nav)
	{
  document.linkmenu.visibility=(n!=0)?"visible":"hidden";
	}
	else linkmenu.style.visibility=(n!=0)?"visible":"hidden";
}
function fakelocation(n)
{
 alert("This is target "+n+" ......\nreplace this link with your target URL");
}
// -->
</SCRIPT>
</BODY>
</HTML>
```

