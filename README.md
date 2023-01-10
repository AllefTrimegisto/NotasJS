# NotasJS

Crie dois códigos de sistema de notas para uma escola. O primeiro código deve ser um programa que informa se o aluno reprovou, ou não, com base nas três notas que ele adicionou ao programa. Utilize, no mínimo, um operador de atribuição e um operador ternário. 
O segundo código é um programa que o aluno deve escrever duas notas e o retorno informa a nota mínima que ele deve tirar na próxima prova para poder passar com nota sete.

Código 1: Programa que informa se o aluno reprovou ou não com base nas três notas:

function checkGrades(grade1, grade2, grade3) {
  // Calcula a média das três notas
  let average = (grade1 + grade2 + grade3) / 3;

  // Usa um operador ternário para determinar se o aluno passou ou não
  let result = average >= 7 ? "Passou" : "Reprovou";

  console.log(result);
}

// Testa o programa com alguns exemplos
checkGrades(8, 9, 7); // Passou
checkGrades(6, 6, 6); // Reprovou
checkGrades(5, 4, 3); // Reprovou

Código 2: Programa que informa a nota mínima que o aluno deve tirar na próxima prova para passar com nota 7:

function minimumGrade(grade1, grade2) {
  // Calcula a média das duas notas
  let average = (grade1 + grade2) / 2;

  // Usa uma operação de atribuição para determinar a nota mínima necessária na próxima prova
  let result = (7 - average) * 2;

  console.log(`Você precisa tirar pelo menos ${result} na próxima prova para passar com nota 7.`);
}

// Testa o programa com alguns exemplos
minimumGrade(6, 8); // Você precisa tirar pelo menos 3 na próxima prova para passar com nota 7.
minimumGrade(5, 5); // Você precisa tirar pelo menos 6 na próxima prova para passar com nota 7.
minimumGrade(9, 7); // Você precisa tirar pelo menos 1 na próxima prova para passar com nota 7.
