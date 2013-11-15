This is a skeleton for my Wordpress Developments. 

Wordpress is inside a /wordpress folder and it is a submodule to the official WordPress. Just checkout the latest version. 
To do that, just excecute:

cd wordpress
git fetch --tags
git checkout XX.XX (insert wordpress version here)
cd ..
git commit -m "Updated Wordpress to version XX.XX"


And that should do the trick. 

All of the contents are outside the wordpress directory in a folder called wp-contents. This makes theme and plugin development independant of wordpress version. 


The theme skeleton is The roots theme, www.roots.io
It is a great theme with HTML5 Bolerplate & Bootstrap. 

To update the subrepository, execute:

cd wp-content/themes/roots
git checkout master
git pull

Afterwards, copy the "roots" folder and rename it to your theme name (I keep it this way because it is easier for me).If you prefere to use another Theme feel free to do it.

The "roots" theme requires Nodejs and Grunt to work correctly, as it will use grunt watch to automatically compress and minify your javascript and css (LESS) files. 

A tutorial on the roots theme is available at www.roots.io/roots-101




