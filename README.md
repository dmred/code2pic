# code2pic

Let **code2pic** make beautiful pics of your beautiful (or not;) code.


## how2install

You can install this package using **npm** or something really usable - **yarn**.

    npm install code2pic --save-dev
    //or
    yarn add code2pic
    
## how2use

**code2pic** has 2 (as in its name) methods: 

 - callback based method (legacy just for those who are from 2008)
 - Promise based method (for modern guys)
 
 If you are a modern guy thats your example of use:
 

    const code2pic = require('code2pic').renderSync;
    
    //some async func bellow
	(async () => {
	
		const someObj = {
			lol: 23,
			kek: 'not kek',
			last: true,
		}
		
		await code2pic(someObj, `./screens/testScreen.png}`)
	})()

or right :) way:

    var code2pic = require('code2pic');
    var fromCodeToPicture = code2pic.render;

	var someObject = {
		lol: 23,
		kek: 'not kek',
		last: true,
	}
	
	fromCodeToPicture(someObject, "./screens/testScreen.png",function(){})
