title: {{name}}

# {{kind}} `{{name}}` {{anchor refid}}

{{briefdescription}}

{{detaileddescription}}

## Members

| Members |                                              
|-----------------------------------------------------------------------------|
{{#each filtered.members}}|<code><b>{{cell proto_text_nospace}}</b></code><div style="margin-top=4px; margin-left: 16px; font-style=italic;">{{cell summary}}</div>|
{{/each}}{{#each filtered.compounds}}|<code><b>{{cell proto_text_nospace}}</b></code><div style="margin-top=4px; margin-left: 16px; font-style=italic;">{{cell summary}}</div>|
{{/each}}

{{#each filtered.members}}
### {{title proto}} {{anchor refid}}

---

{{#if enumvalue}}
 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
{{#each enumvalue}}{{cell name}}            | {{cell summary}}
{{/each}}
{{/if}}

{{briefdescription}}

{{detaileddescription}}

{{/each}}
