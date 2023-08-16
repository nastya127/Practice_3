# Practice: Create a very helpful function, use it couple of times

## Завдання 1 

Global Scope: створити змінну в глобальній області видимості, створити функцію і в тілі функції вивести цю змінну в консоль 
Function Scope: створити функцію, оголосити зміну всередині функції, тоді спробувати вивести цю змінну в консоль всередині функції, та за межами функції 

Block Scope: Створити функцію, в функції написати блок {} всередині якого оголосити змінну та вивести її в консоль, тоді вивести в консоль цю змінну за межами блоку, та подивитись на результат

```
// write below code for global scope
 
// write below code for function scope
 
// write below code for block scope
```


## Завдання 2 

В функції showCarInfo вивести в консоль name та model об'єкту car використовуючи контекст через this, викликати функцію showCarInfo використовуючи bind.

```
const car = {
 name : "Tesla",
 model : "X",
};
 
function showCarInfo() {
   // write code here
}
```

## Завдання 3

Дано: код в якому необхідно знайти помилку і виправити її 

Результат: вивести в консоль “meow”

```
const cat = {
 sound: 'meow',
 greet: function() {
   setTimeout(function() {
       console.log(this.sound)
   }, // write fix in this line of code
   0)
 }
};
cat.greet(); // should produce "meow"
```

## Завдання 4 

Дано: об'єкт у якому необхідно переписати існуючу функція на стрілочну, щоб він почав виконуватись коректно

Результат: вивести у консоль “bark”

```
const dog = {
 sound: 'bark',
 greet: function() {
     setTimeout(function () { // fix code in this line
         console.log(this.sound)
     },0)
   }
}
 
dog.greet();
```

## Завдання 5 

Дано: написати Анонімну функцію та присвоїти її значення змінній convert, функція має приймати число, яке є кількістю байтів та повертати стрічку із переведеними байтами в мб, з двома знаками після коми в форматі "100.00 Mb" та викликати цю функцію використовуючи call 

Результат: функція приймає число (байти) та перетворює у стрічку у форматі Мб наприклад: 

10000 -> 0.01 Mb

```
let convert; // write your anonymous function here
```

## Завдання 6 

Дано: написати функцію logPersonNameAndInterests яка прийматиме довільну кількість аргументів стрічок та виводитиме в консоль повне ім'я Person використовуючи виклик getFullName з контекстом Person, а також перелік усіх його інтересів які приходять аргументами цієї функції 

Результат: виклик logPersonNameAndInterests з контекстом Person та переліком інтересів ['sushi', 'hiking'] -> в консолі 'John Doe loves: sushi, hiking'

```
const Person = {
 firstName: 'John',
 lastName: 'Doe',
 getFullName: function () {
     const fullName = this.firstName + ' ' + this.lastName;
     return fullName;
 }
};
 
const testArgs = ['sushi', 'hiking']
 
let logPersonNameAndInterests; // your code here
```
