Challenge #3

We have a nested object, we would like a function that you pass in the object and a key and get back the value. How this is implemented is up to you.

Steps:

As we know we can achieve this with various options, Just keeping one of the solution with nested-loop in JavaScript.


const obj = {"x":{"y":{"z":"a"}}}
const keys = ['x', 'y', 'z']

function nestedLoop(obj) {
    const res = {};
    function recurse(obj, current) {
        for (const key in obj) {
            let value = obj[key];
            if(value != undefined) {
                if (value && typeof value === 'object') {
                    recurse(value, key);
                } else {
                  	// Do your stuff here to var value
                    res[key] = value;
                }
            }
        }
    }
    recurse(obj);
    return res;
}

console.log(nestedLoop(obj));
console.log(nestedLoop(keys));