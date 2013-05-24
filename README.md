laso.js
=======

Simple Local Storage 

This implimentation hasn't been browser tested in anthing other than a modern Chrome and Safari. It's really not doing anything complex, so browser support should be fine, but for now... who knows.

Basic usage:
	
	var ls = new Laso("my_ls");	// this created a new Laso with an id to check if we created any prior data it might find.

	ls.loadFromLocal(); // this will pull in any local storage info, should it exist into an easy to manage object.

	// from this point we can do standard JS object manipulation to ls.data
	// you can always use a few helper functions.
	// ls.get('name'); would attempt to find a name object in our ls
	// ls.set('name','eric'); will set ls.data.name to eric
	// ls.clear(); clears out everything.

	//ls.set('name','eric') == ls.data.name='eric'; 
	// write your code however you want.

	ls.saveToLocal(); // this saves your data to local storage.

Simple.