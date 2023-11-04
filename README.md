# object

var student = {
    name: "John",
    age: 32,
    lang: ["English", "Bengali"]
}

console.log(student.name);


// use of constructor

function Student(name,age,lang){
     this.name= name;
     this.age= age;
     this.lang= lang;
}
var student= new Student("John", 30,["english", "Bengali"]);// here we assaign the value for Student constructor
console.log(student.lang);

// function in constructor

function Student(name,age,lang){
     this.name= name;
     this.age= age;
     this.lang= lang;

     this.display= function(){
        console.log(this.name);
        console.log(this.age);
        console.log(this.lang);
     }
}
var student1= new Student("John", 30,["english", "Bengali"]);
var student2= new Student("Johnii", 33,["english", "Bengali", "Hindi"]);

student1.display();
student2.display();
