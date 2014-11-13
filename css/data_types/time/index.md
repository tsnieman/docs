{{Page_Title|&lt;time&gt;}}
{{Flags
|State=Ready to Use
|Checked_Out=No
}}
{{Standardization_Status|W3C Candidate Recommendation}}
{{Summary_Section|The <code>&lt;time></code> CSS data type specifies a duration in time, expressed as a number followed (without whitespace) by one of the time unit abbreviations: '''s''' or '''ms'''.}}
{{Data_Type_Page
|Content=In CSS3, time units must be either seconds ('''s''') or milliseconds ('''ms'''); milliseconds are
one-thousandth of a second. Time values can be used to measure the duration of
animation effects, in which case the numeric value must be greater than or
equal to zero.
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=CSS
|Code=.changeable {
    background-color: #fff;
    transition-property: background-color;
    /* transition takes half a second to complete */
    transition-duration: 0.5s;
}
.changeable:hover {
    background-color: #ff4; 
    /* transition to yellow on mouseover */
}
}}
}}
{{Notes_Section}}
{{Related_Specifications_Section
|Specifications={{Related Specification
|Name=CSS Values and Units Module Level 3
|URL=http://www.w3.org/TR/css3-values/
|Status=Candidate Recommendation
}}
}}
{{Compatibility_Section
|Not_required=No
|Imported_tables=
|Desktop_rows=
|Mobile_rows=
|Notes_rows=
}}
{{See_Also_Section}}
{{Topics|CSS}}
{{External_Attribution
|Is_CC-BY-SA=No
|MDN_link=
|MSDN_link=
|HTML5Rocks_link=
}}
{{API_Name}}