function whoAmI(name, age) {
    let yearOfBirth = calcYearOfBirth(age);
    
    console.log(`Hi, my name is ${name} and I'm ${age} years old.`);

    console.log(`I was born in ${yearOfBirth}`);
}
function calcYearOfBirth(age) {
    return 2018 - age;
}
whoAmI();     
     
