
## My First Testing With Jest + eslint-plugin-jest

**@types/jest setup**

 1. `npm install --save-dev @types/jest`
 
 3.  adding typescript type checking for js.
	  - *Per file* (adding `// @ts-check` to the top of a file)
	  
	  - *Using a setting*  (To enable type checking for all JavaScript files without changing any code, just add `"js/ts.implicitProjectConfig.checkJs": true` to your workspace or user settings.)
	  
	  - *Using jsconfig or tsconfig* (To enable type checking for JavaScript files that are part of a `jsconfig.json` or `tsconfig.json`, add `"checkJs": true` to the project's compiler options)

        [@types/jest](https://www.npmjs.com/package/@types/jest)
        
        [Ts type checking for vscode (3 ways to add)](https://code.visualstudio.com/docs/nodejs/working-with-javascript#_type-checking-javascript)


**Jest setup**

 5. `npm install jest --save-dev`
 6. Inside package.json
		 

        "scripts": {
	        "test": "jest"
	     }
	    
7. create a `sum.js`  file.
 
 	   function sum(a, b) {
	      return a + b;
	    }
	    module.exports = sum;
8. Then, create a file named `sum.test.js`
	

	    const sum = require('./sum');
	    
	    test('adds 1 + 2 to equal 3', () => {
	      expect(sum(1, 2)).toBe(3);
	    });
9. `npm run test`

   [https://jestjs.io/docs/getting-started](https://jestjs.io/docs/getting-started)


*Extra :- You can use [Jest runner extension](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest&ssr=false#review-details)*

 
