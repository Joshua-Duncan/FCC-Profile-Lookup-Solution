```
//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
// Only change code below this line


//First we loop through the array looking for a match to 'name' AND 'prop'. If it matches, return the value of the property we are currently on. The loop ends.

//If the first if statement fails, look for a match to 'name' and look to see if 'prop' exists. If it doesn't, return "No such property"

//If the second if statement fails, then there is no match to 'name'. return "No such contact".

for(var i = 0; i < contacts.length; i++){
  if(contacts[i].firstName === name && contacts[i].hasOwnProperty(prop)){
    return contacts[i][prop];
  }else if(contacts[i].firstName === name && !contacts[i].hasOwnProperty(prop)){
    return "No such property";
  }
}
  //If name does not correspond to any contacts then return "No such contact"
  return "No such contact";

// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```
