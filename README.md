# sec-calculator

Kalkulator sederhana dikerjakan menggunakan Javascript method eval() dan pengondisian if else.
<br />
```bash
function Calculator() {
  while (true) {
    var a, group;
    a = prompt("Simple Calculator");
    group = a.split(" ");

    switch (group[1].charAt(0)) {
      case "+":
        if ((Number.parseInt(group[0]) | Number.parseInt(group[2])) > 1000000) {
          alert("Maksimal angka 1 juta");
        } else {
          alert(Number.parseInt(group[0]) + Number.parseInt(group[2]));
        }
        break;
      case "-":
        if ((Number.parseInt(group[0]) | Number.parseInt(group[2])) > 1000000) {
          alert("Maksimal angka 1 juta");
        } else {
          alert(Number.parseInt(group[0]) - Number.parseInt(group[2]));
        }
        break;
      case "*":
        if ((Number.parseInt(group[0]) | Number.parseInt(group[2])) > 1000000) {
          alert("Maksimal angka 1 juta");
        } else {
          alert(Number.parseInt(group[0]) * Number.parseInt(group[2]));
        }
        break;
      case "/":
        if ((Number.parseInt(group[0]) | Number.parseInt(group[2])) > 1000000) {
          alert("Maksimal angka 1 juta");
        } else {
          alert(Number.parseInt(group[0]) / Number.parseInt(group[2]));
        }
    }
  }
}

Calculator();

```
