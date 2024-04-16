- use de-structuring for arrays also
- ```
  const name = "zakria jan";
  const [firstName, lastName] = name.split(" ");
  ```
- use toggle for adding and removing class in vanilla js
- ```
  const elem = document.querySelector("selector-query");
  elem.classList.toggle("class-to-be-added-and-removed")
  ```
- To view which code is changing the specific element in the DOM
- ```
  Inspect Element from dev tools
  right click and move to the option breakon => attribute modification 
  or whatever option suits you in the sub menu
  all are helpful
  ```
- For styling of console use %c in the beginning of the string. It does apply to strings only
- ```
  console.log("%c This is a test statement", "font-size: 20px;")
  ```
- Difference btw ?? and short circuting i.e. || or &&
- ```
  ?? will only move to right side if left side value is either null or undefined e.g.
  0 ?? 5 => 0, 
  null ?? 5 => 5, 
  undefined ?? 5 => 5, 
  {} ?? 5 => {}, 
  "" ?? 5 => "",
  true ?? 5 => true
  false ?? 5 => false
  
  ||, && will try to convert the left side value to boolean
  0 || 5 => 5
  true || 5 => true
  
  ```
-
- Use Number.isFininte(number) to check whether it is infinity or not
- ```
  if(!Number.isFinite(num)){
  	throw new Error("You can not provide infinity")
  }
  ```
- Function definition vs function declaration
- ```
  Below is function definition. We can call this function only after its definition
  
  square(5) => would throw error because it is being used before its definition
  const square = function(x){
  	return x * x
  }
  
  Below is function declaration
  
  cube(2) => would execute successfully without any errors because it has been hoisted
  function cube(x){
  	return x ** 3;
  }
  ```
- use of defer
- ```
  defer is used to tell the browser that continue downloading HTML until script 
  tag is reached. When it is reached, it would download the javascript but won't
  execute it until HTML loading/parsing is finished. This improves performence by loading 
  Javascript and HTML simultaneously. For multiple script tags, they will be downloaded
  and executed in exact order they appeared in the code.
  i.e
  <script src="./script.js" defer></script>
  
  It is used for the js present in external files. It only works for the external 
  js file
  ```
- Difference between onload and DOMContentLoaded events
- ```
  onload is trigerred when whole website is loaded, e.g. 
  - All the primary stuff(layout and structure of the web page)
  - All the secondary stuff(images, videos, audios, stylesheets etc)
  
  DOMContentLoaded is trigerred when all the primary stuff has been loaded.
  It would not wait for secondary stuuf to load. It would load the img tag but the 
  actual image would be painted later
  ```
- Basic difference between var and let
- ```
  ```