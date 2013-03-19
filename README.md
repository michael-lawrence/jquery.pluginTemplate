#jquery.pluginTemplate

Simple jQuery plugin template with CommonJS and AMD support.

* * *

###Configuration

```javascript
{
	'name' : 'myPlugin',
	'isStatic' : false,
    'deps' : ['jquery'],
	'factory' : function ($) {
		return function () {
			// implementation
		};
	}
}
```

#####name
This is simply the name of the plugin.

#####isStatic
A value of true will result in a static plugin that is referenced via $.myPlugin(), where a value of false will result in a plugin that expects a valid jQuery object. For example, $('#myElement').myPlugin().

#####deps
An array of AMD dependencies the plugin needs. By default only jQuery is included.

#####factory
Just replace the "// implementation" comment with your plugin code.


### Bower installation

	bower install jquery.pluginTemplate