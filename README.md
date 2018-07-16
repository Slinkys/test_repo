function whoAmI(name, age) {
    let yearOfBirth;
    try {
        let yearOfBirth = calcYearOfBirth(age);
    }
    catch(e) {
        console.error(e.message);
    }
    console.log(`Hi, my name is ${name} and I'm ${age} years old.`);
    console.log(`I was born in ${yearOfBirth}`);
}
function calcYearOfBirth(age) {
    if (age <= 0) { 
       throw new Error('Age cannot be negative'); 
    }    
    return 2018 - age;
}   
whoAmI();     
     
