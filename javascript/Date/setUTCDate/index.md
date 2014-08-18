{{Page_Title}}
{{Flags
|State=Ready to Use
|Editorial notes=
|Checked_Out=No
}}
{{Summary_Section|Sets the numeric day of the month in the Date object using Universal Coordinated Time (UTC).}}
{{JS_Syntax
|Formats={{JS Syntax Format
|Format=dateObj.'''setUTCDate(''' numDate ''')'''
}}
|Values={{JS Syntax Parameter
|Name=dateObj
|Required=Required
|Description=Any Date object.
}}{{JS Syntax Parameter
|Name=numDate
|Required=Required
|Description=A numeric value equal to the day of the month.
}}
}}
{{JS_Return_Value
|Description=
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=JavaScript
|Description=The following example illustrates the use of the '''setUTCDate''' method.
|Code=function SetUTCDateDemo(newdayofmonth){
    var d = new Date();           // Create Date 
    object.d.setUTCDate( newdayofmonth ) ;  // Set UTC day of month.
    var s = "Current setting is ";
    s += d.toUTCString(); 
    return(s);                    // Return new setting.
 }
|LiveURL=
}}
}}
{{Remarks_Section
|Remarks=To set the day of the month using local time, use the '''setDate''' method.

If the value of numDate is greater than the number of days in the month stored in the '''Date''' object or is a negative number, the date is set to a date equal to numDate minus the number of days in the stored month. For example, if the stored date is January 5, 1996, and '''setUTCDate(32)''' is called, the date changes to February 1, 1996. Negative numbers have a similar behavior.

The '''setUTCFullYear''' method can be used to set the year, month, and day of the month.
}}
{{Notes_Section
|Usage=
|Notes=
|Import_Notes=
}}
{{JS Object Listing}}
{{Topics | JS Basic}}
{{See_Also_Section
|Manual_links=* [[javascript/Date/getDate{{!}}getDate Method (Date)]]
* [[javascript/Date/getUTCDate{{!}}getUTCDate Method (Date)]]
* [[javascript/Date/setDate{{!}}setDate Method (Date)]]
|External_links=
|Manual_sections=
}}
{{JS Topics
|JS Page Type=JS Method
|Applies to=Date
}}
{{External_Attribution
|Is_CC-BY-SA=No
|Sources=MSDN
|MDN_link=
|MSDN_link=http://msdn.microsoft.com/en-us/library/ie/xy2a08e6(v=vs.94).aspx
|HTML5Rocks_link=
}}