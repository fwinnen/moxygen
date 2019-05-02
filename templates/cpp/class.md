title: {{name}}

# {{kind}} `{{name}}` {{anchor refid}}

{{#if basecompoundref}}
```
{{kind}} {{name}}
  {{#each basecompoundref}}
  : {{prot}} {{name}}
  {{/each}}
```  
{{/if}}

{{briefdescription}}

{{detaileddescription}}

## Members

| Members |                                              
|-----------------------------------------------------------------------------|
{{#each filtered.compounds}}|<code><b>{{cell proto_text_nospace}}</b></code><div style="margin-top=4px; margin-left: 16px; font-style=italic;">{{cell summary}}</div>||
{{/each}}{{#each filtered.members}}|<code><b>{{cell proto_text_nospace}}</b></code><div style="margin-top=4px; margin-left: 16px; font-style=italic;">{{cell summary}}</div>|
{{/each}}

{{#each filtered.compounds}}

---

### {{title proto}} {{anchor refid}}

{{briefdescription}}

{{detaileddescription}}

{{/each}}

{{#each filtered.members}}

---

### <code><b>{{title proto_text}}</b></code> { #{{refid}} data-toc-label='{{proto_text_only}}' }

{{#if enumvalue}}
 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
{{#each enumvalue}}{{cell name}}            | {{cell summary}}
{{/each}}
{{/if}}

{{briefdescription}}

{{detaileddescription}}

{{/each}}
