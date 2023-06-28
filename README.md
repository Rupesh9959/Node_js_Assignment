<!-- 2 Question -->

SELECT t.customerId, t.name, lower(Subjects.subjectName) AS subjects FROM ( customers INNER JOIN Subject_student_mapping ON customers.customerId = Subject_student_mapping.customerId ) AS t INNER JOIN Subjects ON Subjects.subjectId = t.subjectId ORDER BY Subjects.subjectName;

<!-- 4 Question -->

const person = { id : 2 , gender : 'mail' }; const student = { name : "ravi" , email :"ravi11@yopmail.com" };

const newObj = {...person, ...student};

<!-- 5 Question -->

const url = "http://www.google.com"; let responsePromise = fetch(url);

responsePromise .then((response) =>{ return response.json(); }) .then((jsonData) =>{ console.log(jsonData); }).catch((error) =>{ console.log(error); });

<!-- 6 Question -->

let num_Ayyay = []; for (let i = 1 ; i <= 100; i++){ num_Ayyay.push(i); } num_Ayyay.pop();

for (let j = 1 ; j <= 100; j++){ if(num_Ayyay.includes(j) === false){ console.log(j); break; } }
