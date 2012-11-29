Sublime Text 2 Config
=====================

Snippets and configuration for Sublime Text 2

Install (Mac OS X)
------------------

Copy directories to `~/Library/Application Support/Sublime Text 2/Packages/` and overwrite.

Javascript snippets
-------------------

### [log] Console log

Shortcut: `super+alt+l`

```javascript
console.log(${0:$TM_SELECTED_TEXT})
```

### [fun] Function

```javascript
function ${1:function_name}( ${2:argument} ) {
    ${0:// I'll do it...}
}
```

### [afn] Anoynmous Function

```javascript
function ( ${1:arguments} ) {
    ${0:// I'll do it...}
}
```

### [$.ajax] jQuery AJAX call

```javascript
$.ajax({
    url: '${1}',
    type: '${2:post}',
    data: ${3:\{\}},
    success: function(${4:data}) {
        ${100:${4:data}}$0
    }
}
```

Edited Default snippets
-----------------------

### [ife] if … else

```javascript
if ( ${1:true} ) {
    ${0:$TM_SELECTED_TEXT}
}
else {
    ${2:// Now what}
}
```

### [if] if

```javascript
if ( ${1:true} ) {
    ${0:$TM_SELECTED_TEXT}
}
```

### [for] Native For-Loop

```javascript
for (var ${20:i} = ${1:Things}.length - 1; ${20:i} >= 0; ${20:i}--) {
	${100:${1:Things}[${20:i}]}$0
}
```

### [while] Native While-Loop

```javascript
while (${1:true}) {
    ${2:// I'll loop it...}
}
```

### [:] Object key — key: "value"

```javascript
${1:key}: ${2:"${3:value}"}${4:, }
```

### [:f] Object Method

```javascript
${1:method_name}: function ( ${3:attribute} ) {
	$0
}${10:,}
```
### [proto] Prototype

```javascript
${1:class_name}.prototype.${2:method_name} = function ( ${3:first_argument} ) {
	${0:// body...}
};
```



