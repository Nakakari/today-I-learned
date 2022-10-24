# DIY

# Choose three main keywords of Week 2, create questions based on the keywords and answer them!

# Q1.What is naming requirements to create components in react
## A1. 
    When creating a component, the first letter must be capitalized. Folders are written with a camel case that starts with a lowercase letter, and files that create components are named with a camel case that starts with an uppercase letter.

# Q2. What is the Map method and the difference of Map method beside other iteration method in Javascript?. Give example of Map methods too !
## A2
    Map() is a method to iterates across an array and applies a callback on each element, returning the resulting elements in a new array.

    - reduce(): metod to reducing a vector to a scalar (a list of values, to a single one). This can be summing all values in an array,  finding the average, minimum or maximum, or in any other way reducing a longer set of data to a smaller one (stem). Map() method not stem the set of data

    - filter(): Filter out items from a list  with iteration that meets specification/condition. Map method iterate all items in array
        forEach(): The main distinction between these two methods is that the map() function returns a new array, whilst the forEach() method does not - it alters the original array.
        Example : calculating square root of every value in array
        const numbers = [9, 36, 64, 144];
        let squareRoots = numbers.map((number) => {
            return Math.sqrt(number);
        });
        console.log(squareRoots); // Output :  [3,6,8,12]
