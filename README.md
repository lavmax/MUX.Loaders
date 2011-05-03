MUX.Loaders
===========

MUX.Loaders is a lightweight Mootools plugin to show styled animated AJAX loaders made with html+css and without any graphic files. Each file weights not more than common gif file. You have full control above styles, sizes and speed. Some loaders allow you to create 'in' and 'out' animation which is useful for 'GET' and 'POST' requests.

Demo is here <a href="http://lavmax.github.com/MUX.Loaders">http://lavmax.github.com/MUX.Loaders</a>

![Screenshot](http://lavmax.github.com/MUX.Loaders/loaders.png)


How to Use
----------

The best description is an example.

	// Creating a simplest loader
	var loader = new MUX.Loader.Bar();
	loader.start(); // Starts and shows the loader
	loader.stop(); // Stops and hides the loader
	
	// You can also use start() and stop() for html element
	$('my-loaders-id').start();
	$('my-loaders-id').stop();
	
	// You can get loader's element using $
	$(loader).inject(document.body);
	// is the same as
	loader.elem.inject(document.body);
	

For full documentation see [Docs/MUX.Loaders.md](https://github.com/lavmax/MUX.Loaders/blob/master/Docs/MUX.Loaders.md).