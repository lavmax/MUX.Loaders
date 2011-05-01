MUX is a Mootools UX libraries family that provides UI objects and add-ons for Mootools for better working with user experience.

##MUX Loaders
is a library with ajax loaders animated icons made with html+css and without any graphic files. It was tested on IE 7+, Firefos 3+, Opera 11, Safari, Chrome, Mobile Safari 4+ and Android 2.3. In some old browsers gradients and borders radius don't work - it's normal. In IE 9 borders radius doesn't work too because of a bug (or feature) in IE.

You can see demo here http://lavmax.github.com/mux/loaders.html

###MUX.Loader
basic class that doesn't use by itself but it provides some basic attributes and methods. It also provides animation garbage collector for lost elements.

####Syntax
<pre>
var loader = new MUX.Loader.Bar([options]);
</pre>

####Common Options
* <code>display</code> - (_string_, defaults to <code>block</code>) CSS display value for visible loader.
* <code>delay</code> - (_int_, default value differs for each loader and suits to loader's animation and size, if you change loader's size you should tune delay empirically) Delay in ms for the animation. The less delay the faster animation.
* <code>id</code> - (_string_, optional) HTML element's id.
* <code>classes</code> - (_string_, optional) HTML element's additional classes. Every loader has also class <code>mux-loader</code>.

####Instance Properties
* <code>elem</code> - Loader's HTML element.

####Instance Methods
* <code>start()</code> - Displays a loader and starts animation. This method is also allowed for <code>elem</code> property.
* <code>stop()</code> - Stops animation and hides a loader. This method is also allowed for <code>elem</code> property.

####General Examples
<pre>
// Creating a simplest loader
var loader = new MUX.Loader.Bar();
loader.start(); // Starts and shows loader
loader.stop(); // Stops and hides loader

// You can also use start() and stop() on html element
$('my-loader-id').start();
$('my-loader-id').stop();

// You can get loader's element using $
$(loader).inject(document.body);
// is the same as
loader.elem.inject(document.body);
</pre>