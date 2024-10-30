# TODO

The following list comprises ideas, suggestions, and known issues, all of which are in consideration for possible implementation in future releases.

***This is not a roadmap or a task list.*** Just because something is listed does not necessarily mean it will ever actually get implemented. Some might be bad ideas. Some might be impractical. Some might either not benefit enough users to justify the effort or might negatively impact too many existing users. Or I may not have the time to devote to the task.

* Add namespace
* Add shortcode
* Add block
* Support a `$args`-style argument array rather than numerous explicit arguments (though this is a bit moot with PHP8 features). Obviously, maintain backward-compatibility.
  * Great opportunity to add support for an optional 'echo' arg to control if function echoes.
  * Update all documentation examples to use the new syntax
* Abstract widget class code into generic class shared amongst my Linkify family of plugins.
  * Consider using `c2c-widget.php` if that can be dropped in.
  * Move strings defined in widget class into main plugin file
* Support getting an tag ID via a custom field if on a single page/post?
* Support conditional before and after? (if main content is empty, don't output before/after strings; could just be 'before_none' and 'after_none', but only after argument array support is added)
* List all tags by default if none are specified?
  * Maybe only if explicitly indicated via an 'all' keyword?
* Widget: Indicate that 'tags' is required
  * Ideally, the widget UI should warn until a category is specified and enforce requirement
* Disable support of HTML by default and require its support to be enabled? (though I consider it necessary for most people's use cases)
* Add ability to omit tags if they don't currently have any published posts

Feel free to make your own suggestions or champion for something already on the list (via the [plugin's support forum on WordPress.org](https://wordpress.org/support/plugin/linkify-tags/) or on [GitHub](https://github.com/coffee2code/linkify-tags/) as an issue or PR).