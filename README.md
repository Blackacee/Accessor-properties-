# Accessor-properties-

var person = { name: "John", surname: "Doe"};
Object.defineProperty(person, 'fullName', {
 get: function () {
 return this.name + " " + this.surname;
 },
 set: function (value) {
 [this.name, this.surname] = value.split(" ");
 }
