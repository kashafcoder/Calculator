# Calculator
<br>
Simple Calculator
<br>
let inputNumber1 = document.getElementById("input-1");
let inputNumber2 = document.getElementById("input-2");
let result = document.getElementById("result");

function clearInputs() {
  inputNumber1.value = "";
  inputNumber2.value = "";
  result.textContent = "";
}

function modulus() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);
  let resultValue = num1 % num2;
  result.textContent = ` ${num1} % ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function add() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);
  let resultValue = num1 + num2;
  result.textContent = ` ${num1} + ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function subtract() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);

  let resultValue = num1 - num2;
  result.textContent = ` ${num1} - ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function multiply() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);
  let resultValue = num1 * num2;
  result.textContent = ` ${num1} * ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function divide() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);
  let resultValue = num1 / num2;
  result.textContent = ` ${num1} / ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function power() {
  let num1 = parseInt(inputNumber1.value);
  let num2 = parseInt(inputNumber2.value);

  validation(num1, num2);
  let resultValue = Math.pow(num1, num2);
  result.textContent = ` ${num1} ^ ${num2} = ${resultValue}`;
  result.style.fontSize = "24px";
}

function validation(num1, num2) {
  if (isNaN(num1) || isNaN(num2)) {
    result.textContent = "Invalid! Please enter valid numbers.";
    result.style.fontSize = "17px";
    result.style.marginLeft = "15px";
    return;
  }
}
console.log("Changes");