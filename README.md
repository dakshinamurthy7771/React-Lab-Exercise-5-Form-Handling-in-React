# React-Lab-Exercise-5-Form-Handling-in-React
# Name: Dakshinamurthy.v
# Roll no: 2305001006
# Department: CSE
# AIM
To develop a simple Student Registration Form using React and handle form input values using the useState Hook.
# PROGRAM
i) App.jsx
```
import { useState } from "react";
import "./App.css";
function App() {
 const [name, setName] = useState("");
 const [registerNo, setRegisterNo] = useState("");
 const [department, setDepartment] = useState("");
 function handleSubmit(event) {
 event.preventDefault();
 alert(
 "Name: " +
 name +
 "\nRegister Number: " +
 registerNo +
 "\nDepartment: " +
 department
 );
 }
 return (
 <div className="container">
 <h1>Student Registration Form</h1>
 <form onSubmit={handleSubmit}>
 <label>Name</label>
 <input
 type="text"
 placeholder="Enter your name"
 value={name}
 onChange={(event) => setName(event.target.value)}
 />
 <label>Register Number</label>
 <input
 type="text"
 placeholder="Enter register number"
 value={registerNo}
 onChange={(event) => setRegisterNo(event.target.value)}
 />
 <label>Department</label>
 <input
 type="text"
 placeholder="Enter department"
 value={department}
 onChange={(event) => setDepartment(event.target.value)}/>
 <button type="submit">Submit</button>
 </form>
 </div>
 );
}
export default App;
```
ii) App.css
```
.container {
 width: 400px;
 margin: 50px auto;
 padding: 25px;
 border: 1px solid gray;
 border-radius: 10px;
}
h1 {
 text-align: center;
 color: blue;
}
label {
 display: block;
 margin-top: 15px;
 font-weight: bold;
}
input {
 width: 100%;
 padding: 10px;
 margin-top: 5px;
 box-sizing: border-box;
}
button {
 margin-top: 20px;
 padding: 10px 20px;
 background-color: blue;
 color: white;
 border: none;
 border-radius: 5px;
 cursor: pointer;
}
```
# OUTPUT
<img width="1450" height="736" alt="image" src="https://github.com/user-attachments/assets/d4ee5a03-793b-427f-bf20-e4a407290938" />
<img width="1488" height="717" alt="image" src="https://github.com/user-attachments/assets/ba0fe665-6a3c-4a05-8aac-848a6a5363ac" />

# RESULT
Thus, a Student Registration Form was successfully created using React. The form input valueswere managed using the useState() Hook, user input was handled using the onChange event, and form submission was handled using the onSubmit event

