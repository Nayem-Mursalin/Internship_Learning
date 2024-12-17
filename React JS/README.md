ReactJS Learning:
Basics of React,

Component
Custom Component
Props
State
State (in Details)


15-12-2024
Learn State Management
	UseState:			const [value, setvalue] = React.useState([])
	use state return an array, first one is a value/string, second one is a function f(). So, we are destructuring it by [value, setvalue].


17-12-2024
Learn: React Form
	-If we declear an object with has a key multiple time then it will not throw an error, it will take only last key. 
	-Our Project Uses React Hook Form. So, I've started React Form 
	-In Form we Have to use  <label htmlFor=""></label> on top off any form element. it help screen reader to read the screen.
	-For Button, if we use this inside a form it's default type is "submit", if we use outside then it's default type is 'button'. <button type="button"></button>
	-In Form the default method is GET request. Or <form method="GET"></form> == <form></form>
	-I can use <fieldset> for making a separate portion (box) for any portion if form.
	-radio Button has a default value of on and null. So we have to use value property to get a value. ex: value="first-time"
	-defaultChecked={true} is used to mark a radio/box by default when we render the page or start the page.
	-For getting every field value of a form we can use "Object.fromEntries()". It will collect all of our data. Ex: const data = Object.fromEntries(formData);
	But it will not recieve multiple checkbox's data, only return a single value of the check box, for gettting all checked item of chk box we have to do, 
	'
	const data = Object.fromEntries(formData)
    const dietaryRestrictions = formData.getAll("dietaryRestrictions")
    const allData = {
      ...data,
      dietaryRestrictions
    }
    console.log(allData)
	'
