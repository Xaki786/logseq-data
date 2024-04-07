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
  ```