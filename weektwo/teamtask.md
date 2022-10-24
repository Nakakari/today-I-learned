# Day Six
So, today we are completing team task. 


# Q1. What’s the differenece between array and array-like object in javascript. How can you change each element in an array-like object?
## Answer
    - The different between array and array-like object in JS can be seen below:
    - When the type of the elements are number, we can use array. But, if the elements have string type, we can use array-like object.
    - The data inside an array is known as Elements. But the data inside array-like object are known as properties which is consist a key and a value.
    - Both of iterating in array and array-like object is possible to use For..in, For..of, and ForEach(). But, we can use For loop in array, not in array-like object.

    For example:
        // Array of objects
        var myObject = {
            jhon: {
                name: 'jhon',
                age: 12,
                gender: 'male'
            },
            rita: {
                name: 'rita',
                age: 32,
                gender: 'male'
            }
        };

        //Array
        var myArr = [1, 2, 3, 4, 5];

    To change each element in an array-like object, we can use:
    - findIndex() method,
        const arr = [
        {id: 1, name: 'Alice'},
        {id: 2, name: 'Bob'},
        ]; //These are objects in an array

        const index = arr.findIndex(object => {
        return object.id === 2;
        }); // findIndex() is the way to get the index of the specific object.

        if (index !== -1) {
        arr[index].name = 'John'; 
        //Access the array at the index and change the  property's value using dot notation.
        } 

        // 👇️ [{id: 1, name: 'Alice'}, {id: 2, name: 'John'}]
        console.log(arr);
    - Array.map() method, 
        const arr = [
        {id: 1, name: 'Alice'},
        {id: 2, name: 'Bob'},
        ];

        const newArr = arr.map(object => {
        if (object.id === 2) {
            //  change value of name property
            return {...object, name: 'John'};
        }
        return object;
        });

        // 👇️ [{id: 1, name: 'Alice'}, {id: 2, name: 'John'}]
        console.log(newArr);

        // 👇️ [{id: 1, name: 'Alice'}, {id: 2, name: 'Bob'}]
        console.log(arr);
    
# Q2 There are parent component A and child component B. Component A has {name: “Sparta"} as its state and pass down the name value to  component B. Then, component B shows the name value on the screen. Please draw the lifecycle of how the value is shown on the screen when component A’s state is changed to {name: "LearningX"}.
## Answer
    const A = () => {
		//Here is parent component
		const  a = {name: “Sparta”}
  		return <div>
  		  <Child name={a}/>
 		 </div>;
    }

    const B = (props) => {
        //Here is child component
        const b = {name: “LearningX”} 
        Return <div>
            {b.name}
    </div>
    }

# Q3. What is two-way binding? Explain What is two-way binding? Explain how the re-rendering is done when using two-way binding. (Assume that there are parent component A and child component B.). (Assume that there are parent component A and child component B.)
## Answer

# Q4. Event listener should be removed when it’s called out. When component is disappered(=unmount) from the screen in class component, event listener is removed in componentWillUnmount. Then, how do you remove event listener in functional component where you can’t use the lifecycle method?
## Answer
    
# Q5. We usually use ref to approach to DOM in react. Why do we use ref instead of document.getElementsByClassName?
## Answer
    