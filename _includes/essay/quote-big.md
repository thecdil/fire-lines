{% comment %}
    Bootstrap Alert, https://getbootstrap.com/docs/4.4/components/alerts/
    Options:
    - "text" = text from the quote or source
    - "source" = [optional] who said the quote / where the quoted text is coming from 
    - "source-link" = [optional]  link to the source (center, right, left)
    - "color" = [optional] a Bootstrap color (primary, secondary, success, danger, warning, info, light, dark)
    - "align" = [optional] text alignment (center, right, left)
    {%- endcomment -%}
<div class="epigraph">
<blockquote class="h1 m-5" ><p class="{% if include.color %}text-{{ include.color }}{% endif %} {% if include.align %}text-{{ include.align }}{% endif %}" style="font-size:2.5em !important; line-height:1.4em">{{ include.text |}}</p>
<footer>{% if include.objectid %}{%- assign item = site.data[site.metadata] | where: "objectid", include.objectid | first -%}<a href="{{ '/mapitem.html' | relative_url | append: '?id=' | append: item.objectid }}">{{item.title}}</a>, {% endif %}{% if include.source-link %}<a href="{{include.source-link }}" target="_blank">{{include.source}}</a>{% else %}{
    {include.source}}{% endif %}</footer></blockquote>
</div>  