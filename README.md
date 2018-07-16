function whoAmI(name, age) {
	if ((name.constructor !== String)){
		console.error('Name is not a string');
    }
	if ((age.constructor !== Number)){
		console.error('Age is not a number');
    }	
	
    if(!name || !age) {
       console.error('Arguments not valid'); 
    }  

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
whoAmI(29, "twenty nine");     
     
