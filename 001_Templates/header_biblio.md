---
category: literaturenote
tags: {% if allTags %}{{ allTags }}{% endif %}
citekey: {{citekey}}
itemType: {{itemType}}
status: unread  
dateread:  
---

> [!Cite]  
> {{bibliography}}

> [!SYNTHESIS] 
>**Contribution**::
>
>**Related**:: {% for relation in relations | selectattr("citekey") %} [[@{{relation.citekey}}]]{% if not loop.last %}, {% endif%} {% endfor %}
>

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
> {%- if itemType == "journalArticle" %}**Journal**:: *{{publicationTitle}}* {%- endif %}    
> {%- if volume %}**Volume**:: {{volume}} {%- endif %}    
> {%- if issue %}**Issue**:: {{issue}} {%- endif %}     
> {%- if itemType == "bookSection" %}**Book**:: {{publicationTitle}} {%- endif %}    
> {%- if publisher %}**Publisher**:: {{publisher}} {%- endif %}    
> {%- if place %}**Location**:: {{place}} {%- endif %}     
> {%- if pages %} **Pages**:: {{pages}} {%- endif %}    
> {%- if DOI %}**DOI**:: {{DOI}} {%- endif %}    
> {%- if ISBN %}**ISBN**:: {{ISBN}} {%- endif %}

> [!LINK] 
>{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}
> [{{attachment.title}}](file://{{attachment.path | replace(" ", "%20")}})  {%- endfor -%}.

>[!Abstract]
>{%- if abstractNote %}
>{{abstractNote}}
>{%- endif -%}
>


# Notes 

{%- if markdownNotes %}
{{markdownNotes}}
{%- endif -%}

<br>
# Annotations

{%- macro calloutHeader(type, color) -%}
{%- if type == "highlight" -%}
<mark style="background-color: {{color}}">Quote</mark>
{%- endif -%}

{%- if type == "text" -%}
Note
{%- endif -%}
{%- endmacro -%}

{% persist "annotations" %}  
{% set newAnnotations = annotations | filterby("date", "dateafter", lastImportDate) %} 
{% if newAnnotations.length > 0 %} 
  
### Imported: {{importDate | format("YYYY-MM-DD h:mm a")}}  
  
{% for a in newAnnotations %}  
{{calloutHeader(a.type, a.color)}}  
> {{a.annotatedText}}
{% endfor %}  
{% endif %}  
{% endpersist %}