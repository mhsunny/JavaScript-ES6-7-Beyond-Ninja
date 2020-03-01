# JavaScript ES6, 7 & beyond to become JS Ninja
  

Becoming a JavaScript ninja! In these examples, here you find some codes of the JavaScript from the very beginning, right through to creating fully-fledged, dynamic & interactive web experiences.

Here you find the basics to get you up-and-running quickly, before diving in to some of the really fun stuff like web-page manipulation, creating interactive forms, popups & other cool effects. Along the way we'll be using the latest additions to the JavaScript specification (ES6, 7 & beyond) and maintaining good coding standards to keep our code clean and effective! 

<ul>
<li>Modern JavaScript, from the very beginning to more advanced topics
</li>

<li>OOP (object-oriented programming) with JavaScript, working with prototypes & classes
</li>

<li>create real-world front-end applications with JavaScript (quizes, weather apps, chat rooms etc)
</li>

<li>make useful JavaScript driven UI components like popups, drop-downs, tabs, tool-tips & more.
</li>

<li>modern, cutting-edge JavaScript features today by using a modern workflow (Babel & Webpack)
</li>

<li>use real-time databases to store, retrieve and update application data
</li>

<li>Explore API's to make the most of third-party data (such as weather information) 
</li>
</ul>


<code>
<pre>

//copy events
const copy = document.querySelector('.copy-me');
copy.addEventListener('copy', () =>{
    console.log("my content copyright")
})
const box = document.querySelector('.box');
box.addEventListener('mousemove', e =>{
    //console.log(e);
    //console.log(e.offsetX, e.offsetY);
    box.textContent = `x pos ${e.offsetX} - y pos ${e.offsetY}`;
    box.setAttribute('style', `left:${e.offsetX}px; top: ${e.offsetY}px`)
} )
 
//click events
const ul = document.querySelector('ul');
// items.remove();

const button = document.querySelector('button');
button.addEventListener('click', ()=>{
    //console.log("you clicked me");
    //ul.innerHTML += '<li>Somehing New</li>'
    const li = document.createElement('li');
    li.textContent = 'some new to do';
    // ul.append(li);
    ul.prepend(li);
})

document.addEventListener('scroll', e =>{
    console.log(e );
    console.log(e.pageX, e.pageY);
})



//const items = document.querySelectorAll('.items li'); 

// items.forEach(item =>{
//     item.addEventListener('click', e =>{
//       // console.log("item click" , item);
//        // console.log(e.target)  ;
//        e.stopPropagation();
//        e.target.style.textDecoration = 'line-through';
//        console.log("click li");
//        //e.target.remove();
//     })
   
// });
// console.log(items);

ul.addEventListener('click', e =>{
    console.log( e);
    if(e.target.tagName === 'LI'){
        e.target.remove();
    }
})


//const article = document.querySelector("article");
//console.log(article.children);
// childsOfArticle = Array.from(article.children);

// childsOfArticle.forEach(child =>{
//     child.classList.add('article-element');
//     console.log(child)
// });

//const title =  document.querySelector("article > h2");
// console.log(title.parentElement);
// console.log(title.nextElementSibling);
// console.log(title.previousElementSibling);

//console.log(title.nextElementSibling.parentElement.children);

// const paras = document.querySelectorAll(".content > p")
// console.log(paras);

// paras.forEach(p =>{
//     if(p.textContent.includes("success")){
//         p.classList.add('success')   ;
     
//     }else if(p.textContent.includes("error")){
//         p.classList.add('error')   ;

//     } 
//     console.log(p.textContent)
// });

// const title = document.querySelector('.title');
// title.classList.toggle('test');
// title.classList.toggle('test');
// console.log(title);



// const content = document.querySelector("p");

// content.classList.add('error')
// console.log(content.classList);
//  content.classList.remove('error')
//  content.classList.add('success')
// console.log(content.classList);

// const title = document.querySelector("h1");
// //title.setAttribute('style', 'margin:20px; color:green')



// title.style.border = '1px solid #ccc'
// title.style.padding = '10px'
// title.style.color = 'red'
// title.style.fontSize = '4rem'

// console.log(title.style) 


// const link = document.querySelector("a");
// link.setAttribute('href', 'https://www.mmhsunny.com')
// link.setAttribute('target', '_blank')
// link.innerText = 'this is link to mmhsunny.com'
// link.setAttribute('style', 'color:green')
// console.log(link.getAttribute('class'));



// const content = document.querySelector(".content");

// const peolple = ['sunny', 'kalam', 'jamala'];

// peolple.forEach(person => {
//     content.innerHTML +=`<p>${person} </p>`;
// })

// console.log(content.innerHTML)
 

//const para = document.querySelector("p");

//console.log(para.innerText = 'this is custom')
//para.innerText = 'this is custom';

// const paras = document.querySelectorAll("p");
// paras.forEach(para =>{
//     para.innerText += ' this is custom text';
//     console.log(para.innerText);
// })
// const content = document.querySelector(".content");
// //console.log(content.innerHTML)
// content.innerHTML += '<h2>this is new h2 heading </h2>'



// const title = document.getElementById("page-title");
//  console.log(title);

// const error = document.getElementsByClassName("error");

// console.log(error);
// console.log(error[0]);


//   const paras = document.getElementsByTagName("p");

//   console.log(paras[1]); 



// const paras = document.querySelectorAll('p');
// paras.forEach( para =>{
    // console.log(para);
// })

// const error =  document.querySelectorAll('.error');

// console.log(error);

// const para = document.querySelector('body > p:nth-child(3)');
// console.log(para);


  

//primitive types & reference type

//numer, strings, strings, booleans, undefinds, sysbol
//store in stack, is quicker to access bu tlimited space

//reference type, 
// object, array, functions, date, object literals
// store data in heap , more space than stack, but slow to access
  
// const userOne = {name: 'sunny', age: 30}
// const userTwo = userOne;
// console.log(userOne, userTwo) 
// //userTwo.age = 40;

// userOne.name = 'kamal';

// console.log(userOne, userTwo) 
  


// //Math Object 

// // const area = 7.9;
// // const area2 = 7.2;
// // console.log(Math.round(area)) // 8
// // console.log(Math.round(area2)) // 7 // nearest 

// // console.log('floor',Math.floor(area)) // 7 // lowest nearest
// // //oposite floor 
// // console.log('ceil' , Math.ceil(area2)) // 7 // hightest nearest
// // //oposite trunc 
// // console.log('trunc',Math.trunc(area)) // take away decimal

// //random
// const random = Math.random(); // 1 -100

// console.log('Random 1 - 100:', Math.round(random * 100)) //  


// console.log(Math.PI)
// console.log(Math.E)
// console.log(Math.SQRT2) 
 
//console.log(Math) 

// //Object literal
//   const blogs = [

//     {title : 'Where does cornavirus effect?', like: 50 },
//     {title : 'I love United States', like: 100 },
//     {title : 'New York MTA is goood for communiation', like: 10 }
//   ];

// //console.log(blogs);

// let user = {
//     name : 'sunny',
//     age : 12,
//     email: 'mhsunny@gmil.com',
//     location: 'New Yrok',
//     blogs:  blogs,
//         login(){
//             console.log("the user logged in");
//         },
//         logout(){
//             console.log("the user logged out");
//         },
//         logBogs(){
//             // console.log(this)
//             console.log("this user has written the follwing blogs");
//             this.blogs.forEach(blog=>{
//                 console.log(blog.title, blog.like)
//             })
//         }

//         // login:function(){
//         //     console.log("the user logged in");
//         // },
//         // logout: () => {
//         //     console.log("the user logged out");
//         // },
//         // logBogs: function(){
//         //     // console.log(this)
//         //     console.log("this user has written the follwing blogs");
//         //     this.blogs.forEach(title=>{
//         //         console.log(title)
//         //     })
//         // }
// }
// user.logBogs()

//console.log(this);

//console.log(user.logBogs())


// user.login()

// const name = 'kamal';
// name.toUpperCase();

// user.logout();
 

// console.log(typeof user)

// const key = 'location';
// console.log(user[key]); 

// user.age = 15; // update propery

// console.log(user.age);

// console.log(user['name']);
// user['name'] = 'kamal';
// console.log(user);




// const ul = document.querySelector('.people');


// let people = ['sunny', 'yellin', 'kaniz', 'jamal'];
// let html = ``;

// people.forEach((person, index) => {
//     html += `<li style='color:purple'>${index} -  ${person}</li>`
// });
// ul.innerHTML = html;

// console.log(html);

// //callback and foreach

// let people = ['sunny', 'yellin', 'kaniz', 'jamal'];

// const logPerson =  (person, index) =>{
//     console.log(`${index} - hello ${person}`);
// }

// people.forEach(logPerson); // callback

// // people.forEach( (person, index) =>{
// //     console.log(index, person);
// // })


// // people.forEach(function(person){
// //      console.log(person);
// // })






// const myFunc = (callbackFunc) =>{
//     let value = 50;
//     callbackFunc(value);

// }

// // myFunc( function(value){
// //         console.log(value);
// // });
// myFunc( 
//     value => {
//         console.log(value);
//     }
    
// );










//function vs methods
// const greet = () => 'hello';
// let resOne = greet();
// console.log(resOne);

// const name = 'sunny'
// let res2 = name.toUpperCase();

// console.log(res2);









// //Arrow function
// const totalBill = (products, tax ) =>{

//     let total = 0;
//     for(i = 0; i < products.length; i++){
//         total += products[i] + products[i]*tax;
//     }
//     return total; 

// }
// console.log(totalBill([20, 30, 40, 10], .1));

// const bill = function(products, tax){

//     let total = 0;
//     for(i = 0; i < products.length; i++){
//         total += products[i] + products[i]*tax;
//     }
//     return total; 
// }

// console.log(bill([20, 30, 40, 10], .1));
 



// const greet = function(){
//     return ' hello there';
// }

// const greeting = () => 'hello there';
// console.log(   greeting()  );


 


// const clacArea  = (radius, param2) => 3.14 * radius**2 / 2; 
// const area = clacArea(12, 2);
// console.log(`Area ${area}`)




// const clacArea  = (radius, param2) =>{

//     return 3.14 * radius**2 / 2; 
// }

// const area = clacArea(12, 2);
// console.log(`Area ${area}`)



// const clacArea = function(radius){
//      return 3.14 * radius**2; 
// }


// const area = clacArea(12);
// console.log(`Area ${area}`)




// //function expression
// const speak = function(name='yellin', time='Morning'){
//     console.log(`I am from speak ${name} ${time}`)
// };
 
//  speak('sunny', 'afternoon');

// //funtion declaration
// function greet(){
//     console.log("Hello There");
// } 

//greet()






// let age = 30; // globa; scope

// if(true){
//     let age = 50;  //local score
//     console.log(age)

//     if(true){
//         let age = 60;
//         console.log("inside 2nd block ", age)
//         var test = "I am var from inside 2d blokc"
//     }
// }

// console.log(age, test)










// let grade = 'B';
// switch(grade){

//     case 'A':
//         console.log('A')
//     break;
//     case 'B':
//         console.log('B') 
//         break;
//     case 'C':
//         console.log('C') 
//         break;   
//     case 'D':
//         console.log('D') 
//         break;

//     default:
//         console.log('Fail')
//  }


// let i = 5;

// do{
//     console.log('val of i = ', i);
//     i++; 
// }while( i < 5);




// let i = 0;
// while( i < 5){
//     console.log('in loop', i);
//     i++;
// }


// const names = ['sunny', 'kniz', 'yellin'];

// let i = 0;
// while( i < names.length){
//     console.log('in loop', i , names[i]);
//     i++;
// }












// const names = ['sunny', 'kniz', 'yellin'];


// for(let i = 0; i < names.length; i++){

//     console.log('in loop', i , names[i])

// }



 







//let score = '100';

// score = Number(score);

// console.log(score + 1);

// console.log( typeof score);
// let res = Number('heloo');

//let res = String(50)

//let res = Boolean(0)

//let res = Boolean('0')





//console.log(res, typeof res);





// let age = 34;

// // console.log(age ==  34);

// // console.log(age  != '34');

// console.log(age !==  34);

// console.log(age  !== '34');




// let email = 'mhsunny@gail.com';

// let  names = ['kamal', 'jamal', 'jhon'];

// //let res = email.includes('com'); // true

// //let res = names.includes('jamal'); //true

// console.log( res ); 





// let age = null;




// let res = age + 3 + ` the age is {$age}`;

//  console.log( res ); 


// // let ninja = ['sunny', 'yellin', 'kaniz'];

// // //let res = ninja.join('-');

// // //let res = ninja.indexOf(ninja[1]);

// // //let res = ninja.concat(['ken', 'den'])

// // let res = ninja.push('Ajele' ) ; // push at last
// //   res = ninja.shift('Kamal' ) ;

// // res = ninja.pop('Ajele' ) // remove last item

// // console.log( res ); 
// // console.log( ninja ); 







// let ninja = ['sunny', 'yellin', 30, 20];
//   console.log( ninja.length); 



// let ninja = ['sunny', 'yellin', 'kaniz'];

// ninja[1] = 'hasan';








// const title = 'Beest read of 2019';
// const author = 'Sunny';
// const likes = 30;

// let out = `The ${title} blog of this of book ${author}
//  has ${likes} likes`;


// let html  = `
// <h2>${title}</h2>
// <p>By  ${author}</p>
// ` ;

// console.log( html ); 









// let radius = 10;
// const pi = 3.14;

// let res = pi * radius **2;
// console.log( res );  

//order operation
//BIDMAS = braket, indecis(power), div, mul, add, subs

// let like = 10;
// like++; // like+1
// like +=10; // like +10
// like *2 
// res = 'this is total' + like + 'like'; 
//  console.log(res);


 

// let full_name = 'mh sunny';

// console.log(full_name[4]); 



//slice 
// let email = 'mhsunny@gmail.com';
// let res =  email.slice(2, 5); //from, to
// console.log(res);

//slice 
// let email = 'mhsunny@gmail.com';
// let res =  email.substr(8, 2); //from, how many
// console.log(res);


//replace 
// let email = 'mhsunny@gmail.com';
// let res =  email.replace('m', 'k' ); //m, with k // replace only frst
// console.log(res);


// const button = document.querySelector('button');
// const close = document.querySelector('.pop-close');

// const popup = document.querySelector('.pouup-wrapper');

// button.addEventListener('click', () =>{
//     console.log('click');
//     popup.style.display = 'block'
// })
// close.addEventListener('click', () =>{
//     console.log('click');
//     popup.style.display = 'none'
// })

// // //copy events
// // const copy = document.querySelector('.copy-me');
// // copy.addEventListener('copy', () =>{
// //     console.log("my content copyright")
// // })
// // const box = document.querySelector('.box');
// // box.addEventListener('mousemove', e =>{
// //     //console.log(e);
// //     //console.log(e.offsetX, e.offsetY);
// //     box.textContent = `x pos ${e.offsetX} - y pos ${e.offsetY}`;
// //     box.setAttribute('style', `left:${e.offsetX}px; top: ${e.offsetY}px`)
// // } )
 
// // //click events
// // const ul = document.querySelector('ul');
// // // items.remove();

// // const button = document.querySelector('button');
// // button.addEventListener('click', ()=>{
// //     //console.log("you clicked me");
// //     //ul.innerHTML += '<li>Somehing New</li>'
// //     const li = document.createElement('li');
// //     li.textContent = 'some new to do';
// //     // ul.append(li);
// //     ul.prepend(li);
// // })

// // document.addEventListener('scroll', e =>{
// //     console.log(e );
// //     console.log(e.pageX, e.pageY);
// // })



// //const items = document.querySelectorAll('.items li'); 

// // items.forEach(item =>{
// //     item.addEventListener('click', e =>{
// //       // console.log("item click" , item);
// //        // console.log(e.target)  ;
// //        e.stopPropagation();
// //        e.target.style.textDecoration = 'line-through';
// //        console.log("click li");
// //        //e.target.remove();
// //     })
   
// // });
// // console.log(items);

// ul.addEventListener('click', e =>{
//     console.log( e);
//     if(e.target.tagName === 'LI'){
//         e.target.remove();
//     }
// })


// //const article = document.querySelector("article");
// //console.log(article.children);
// // childsOfArticle = Array.from(article.children);

// // childsOfArticle.forEach(child =>{
// //     child.classList.add('article-element');
// //     console.log(child)
// // });

// //const title =  document.querySelector("article > h2");
// // console.log(title.parentElement);
// // console.log(title.nextElementSibling);
// // console.log(title.previousElementSibling);

// //console.log(title.nextElementSibling.parentElement.children);

// // const paras = document.querySelectorAll(".content > p")
// // console.log(paras);

// // paras.forEach(p =>{
// //     if(p.textContent.includes("success")){
// //         p.classList.add('success')   ;
     
// //     }else if(p.textContent.includes("error")){
// //         p.classList.add('error')   ;

// //     } 
// //     console.log(p.textContent)
// // });

// // const title = document.querySelector('.title');
// // title.classList.toggle('test');
// // title.classList.toggle('test');
// // console.log(title);



// // const content = document.querySelector("p");

// // content.classList.add('error')
// // console.log(content.classList);
// //  content.classList.remove('error')
// //  content.classList.add('success')
// // console.log(content.classList);

// // const title = document.querySelector("h1");
// // //title.setAttribute('style', 'margin:20px; color:green')



// // title.style.border = '1px solid #ccc'
// // title.style.padding = '10px'
// // title.style.color = 'red'
// // title.style.fontSize = '4rem'

// // console.log(title.style) 


// // const link = document.querySelector("a");
// // link.setAttribute('href', 'https://www.mmhsunny.com')
// // link.setAttribute('target', '_blank')
// // link.innerText = 'this is link to mmhsunny.com'
// // link.setAttribute('style', 'color:green')
// // console.log(link.getAttribute('class'));



// // const content = document.querySelector(".content");

// // const peolple = ['sunny', 'kalam', 'jamala'];

// // peolple.forEach(person => {
// //     content.innerHTML +=`<p>${person} </p>`;
// // })

// // console.log(content.innerHTML)
 

// //const para = document.querySelector("p");

// //console.log(para.innerText = 'this is custom')
// //para.innerText = 'this is custom';

// // const paras = document.querySelectorAll("p");
// // paras.forEach(para =>{
// //     para.innerText += ' this is custom text';
// //     console.log(para.innerText);
// // })
// // const content = document.querySelector(".content");
// // //console.log(content.innerHTML)
// // content.innerHTML += '<h2>this is new h2 heading </h2>'



// // const title = document.getElementById("page-title");
// //  console.log(title);

// // const error = document.getElementsByClassName("error");

// // console.log(error);
// // console.log(error[0]);


// //   const paras = document.getElementsByTagName("p");

// //   console.log(paras[1]); 



// // const paras = document.querySelectorAll('p');
// // paras.forEach( para =>{
//     // console.log(para);
// // })

// // const error =  document.querySelectorAll('.error');

// // console.log(error);

// // const para = document.querySelector('body > p:nth-child(3)');
// // console.log(para);


  

// //primitive types & reference type

// //numer, strings, strings, booleans, undefinds, sysbol
// //store in stack, is quicker to access bu tlimited space

// //reference type, 
// // object, array, functions, date, object literals
// // store data in heap , more space than stack, but slow to access
  
// // const userOne = {name: 'sunny', age: 30}
// // const userTwo = userOne;
// // console.log(userOne, userTwo) 
// // //userTwo.age = 40;

// // userOne.name = 'kamal';

// // console.log(userOne, userTwo) 
  


// // //Math Object 

// // // const area = 7.9;
// // // const area2 = 7.2;
// // // console.log(Math.round(area)) // 8
// // // console.log(Math.round(area2)) // 7 // nearest 

// // // console.log('floor',Math.floor(area)) // 7 // lowest nearest
// // // //oposite floor 
// // // console.log('ceil' , Math.ceil(area2)) // 7 // hightest nearest
// // // //oposite trunc 
// // // console.log('trunc',Math.trunc(area)) // take away decimal

// // //random
// // const random = Math.random(); // 1 -100

// // console.log('Random 1 - 100:', Math.round(random * 100)) //  


// // console.log(Math.PI)
// // console.log(Math.E)
// // console.log(Math.SQRT2) 
 
// //console.log(Math) 

// // //Object literal
// //   const blogs = [

// //     {title : 'Where does cornavirus effect?', like: 50 },
// //     {title : 'I love United States', like: 100 },
// //     {title : 'New York MTA is goood for communiation', like: 10 }
// //   ];

// // //console.log(blogs);

// // let user = {
// //     name : 'sunny',
// //     age : 12,
// //     email: 'mhsunny@gmil.com',
// //     location: 'New Yrok',
// //     blogs:  blogs,
// //         login(){
// //             console.log("the user logged in");
// //         },
// //         logout(){
// //             console.log("the user logged out");
// //         },
// //         logBogs(){
// //             // console.log(this)
// //             console.log("this user has written the follwing blogs");
// //             this.blogs.forEach(blog=>{
// //                 console.log(blog.title, blog.like)
// //             })
// //         }

// //         // login:function(){
// //         //     console.log("the user logged in");
// //         // },
// //         // logout: () => {
// //         //     console.log("the user logged out");
// //         // },
// //         // logBogs: function(){
// //         //     // console.log(this)
// //         //     console.log("this user has written the follwing blogs");
// //         //     this.blogs.forEach(title=>{
// //         //         console.log(title)
// //         //     })
// //         // }
// // }
// // user.logBogs()

// //console.log(this);

// //console.log(user.logBogs())


// // user.login()

// // const name = 'kamal';
// // name.toUpperCase();

// // user.logout();
 

// // console.log(typeof user)

// // const key = 'location';
// // console.log(user[key]); 

// // user.age = 15; // update propery

// // console.log(user.age);

// // console.log(user['name']);
// // user['name'] = 'kamal';
// // console.log(user);




// // const ul = document.querySelector('.people');


// // let people = ['sunny', 'yellin', 'kaniz', 'jamal'];
// // let html = ``;

// // people.forEach((person, index) => {
// //     html += `<li style='color:purple'>${index} -  ${person}</li>`
// // });
// // ul.innerHTML = html;

// // console.log(html);

// // //callback and foreach

// // let people = ['sunny', 'yellin', 'kaniz', 'jamal'];

// // const logPerson =  (person, index) =>{
// //     console.log(`${index} - hello ${person}`);
// // }

// // people.forEach(logPerson); // callback

// // // people.forEach( (person, index) =>{
// // //     console.log(index, person);
// // // })


// // // people.forEach(function(person){
// // //      console.log(person);
// // // })






// // const myFunc = (callbackFunc) =>{
// //     let value = 50;
// //     callbackFunc(value);

// // }

// // // myFunc( function(value){
// // //         console.log(value);
// // // });
// // myFunc( 
// //     value => {
// //         console.log(value);
// //     }
    
// // );










// //function vs methods
// // const greet = () => 'hello';
// // let resOne = greet();
// // console.log(resOne);

// // const name = 'sunny'
// // let res2 = name.toUpperCase();

// // console.log(res2);









// // //Arrow function
// // const totalBill = (products, tax ) =>{

// //     let total = 0;
// //     for(i = 0; i < products.length; i++){
// //         total += products[i] + products[i]*tax;
// //     }
// //     return total; 

// // }
// // console.log(totalBill([20, 30, 40, 10], .1));

// // const bill = function(products, tax){

// //     let total = 0;
// //     for(i = 0; i < products.length; i++){
// //         total += products[i] + products[i]*tax;
// //     }
// //     return total; 
// // }

// // console.log(bill([20, 30, 40, 10], .1));
 



// // const greet = function(){
// //     return ' hello there';
// // }

// // const greeting = () => 'hello there';
// // console.log(   greeting()  );


 


// // const clacArea  = (radius, param2) => 3.14 * radius**2 / 2; 
// // const area = clacArea(12, 2);
// // console.log(`Area ${area}`)




// // const clacArea  = (radius, param2) =>{

// //     return 3.14 * radius**2 / 2; 
// // }

// // const area = clacArea(12, 2);
// // console.log(`Area ${area}`)



// // const clacArea = function(radius){
// //      return 3.14 * radius**2; 
// // }


// // const area = clacArea(12);
// // console.log(`Area ${area}`)




// // //function expression
// // const speak = function(name='yellin', time='Morning'){
// //     console.log(`I am from speak ${name} ${time}`)
// // };
 
// //  speak('sunny', 'afternoon');

// // //funtion declaration
// // function greet(){
// //     console.log("Hello There");
// // } 

// //greet()






// // let age = 30; // globa; scope

// // if(true){
// //     let age = 50;  //local score
// //     console.log(age)

// //     if(true){
// //         let age = 60;
// //         console.log("inside 2nd block ", age)
// //         var test = "I am var from inside 2d blokc"
// //     }
// // }

// // console.log(age, test)










// // let grade = 'B';
// // switch(grade){

// //     case 'A':
// //         console.log('A')
// //     break;
// //     case 'B':
// //         console.log('B') 
// //         break;
// //     case 'C':
// //         console.log('C') 
// //         break;   
// //     case 'D':
// //         console.log('D') 
// //         break;

// //     default:
// //         console.log('Fail')
// //  }


// // let i = 5;

// // do{
// //     console.log('val of i = ', i);
// //     i++; 
// // }while( i < 5);




// // let i = 0;
// // while( i < 5){
// //     console.log('in loop', i);
// //     i++;
// // }


// // const names = ['sunny', 'kniz', 'yellin'];

// // let i = 0;
// // while( i < names.length){
// //     console.log('in loop', i , names[i]);
// //     i++;
// // }












// // const names = ['sunny', 'kniz', 'yellin'];


// // for(let i = 0; i < names.length; i++){

// //     console.log('in loop', i , names[i])

// // }



 







// //let score = '100';

// // score = Number(score);

// // console.log(score + 1);

// // console.log( typeof score);
// // let res = Number('heloo');

// //let res = String(50)

// //let res = Boolean(0)

// //let res = Boolean('0')





// //console.log(res, typeof res);





// // let age = 34;

// // // console.log(age ==  34);

// // // console.log(age  != '34');

// // console.log(age !==  34);

// // console.log(age  !== '34');




// // let email = 'mhsunny@gail.com';

// // let  names = ['kamal', 'jamal', 'jhon'];

// // //let res = email.includes('com'); // true

// // //let res = names.includes('jamal'); //true

// // console.log( res ); 





// // let age = null;




// // let res = age + 3 + ` the age is {$age}`;

// //  console.log( res ); 


// // // let ninja = ['sunny', 'yellin', 'kaniz'];

// // // //let res = ninja.join('-');

// // // //let res = ninja.indexOf(ninja[1]);

// // // //let res = ninja.concat(['ken', 'den'])

// // // let res = ninja.push('Ajele' ) ; // push at last
// // //   res = ninja.shift('Kamal' ) ;

// // // res = ninja.pop('Ajele' ) // remove last item

// // // console.log( res ); 
// // // console.log( ninja ); 







// // let ninja = ['sunny', 'yellin', 30, 20];
// //   console.log( ninja.length); 



// // let ninja = ['sunny', 'yellin', 'kaniz'];

// // ninja[1] = 'hasan';








// // const title = 'Beest read of 2019';
// // const author = 'Sunny';
// // const likes = 30;

// // let out = `The ${title} blog of this of book ${author}
// //  has ${likes} likes`;


// // let html  = `
// // <h2>${title}</h2>
// // <p>By  ${author}</p>
// // ` ;

// // console.log( html ); 









// // let radius = 10;
// // const pi = 3.14;

// // let res = pi * radius **2;
// // console.log( res );  

// //order operation
// //BIDMAS = braket, indecis(power), div, mul, add, subs

// // let like = 10;
// // like++; // like+1
// // like +=10; // like +10
// // like *2 
// // res = 'this is total' + like + 'like'; 
// //  console.log(res);


 

// // let full_name = 'mh sunny';

// // console.log(full_name[4]); 



// //slice 
// // let email = 'mhsunny@gmail.com';
// // let res =  email.slice(2, 5); //from, to
// // console.log(res);

// //slice 
// // let email = 'mhsunny@gmail.com';
// // let res =  email.substr(8, 2); //from, how many
// // console.log(res);


// //replace 
// // let email = 'mhsunny@gmail.com';
// // let res =  email.replace('m', 'k' ); //m, with k // replace only frst
// // console.log(res);


</pre>
</code>


 
