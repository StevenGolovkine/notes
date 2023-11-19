---
category: postsnote
tags: {% if allTags %}{{ allTags }}{% endif %}
citekey: {{citekey}}
itemType: {{itemType}}
status: unread  
dateread:  
---

> [!SYNTHESIS] 
>**Contribution**::

> [!METADATA]  
> {%- for creator in creators %}
{%- if creator.name == null %}
**{{creator.creatorType | capitalize}}**:: {{creator.lastName}}, {{creator.firstName}}
{%- endif -%} 
{%- if creator.name %}
**{{creator.creatorType | capitalize}}**:: {{creator.name}}
{%- endif -%}
{%- endfor %}<br>
> **Title**:: {{title}}    
> **Year**:: {{date | format("YYYY")}}     
> **Citekey**:: @{{citekey}}    
> {%- if blogTitle %}**Blog Title**:: {{blogTitle}} {%- endif %}   
>  {%- if dateAdded %}**Accessed**:: {{dateAdded | format("YYYY-MM-DD")}} {%- endif %}   
> 

> [!LINK] 
>{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}
> [{{attachment.title}}](file://{{attachment.path | replace(" ", "%20")}})  {%- endfor -%}.

> [!Cite]  
> {{bibliography}}
