# sec-technical-test-calculator
Technical Test Azura Labs
<br /><br />
<b>Perintah:</b> <br />
Membuat fungsi kalkulator sederhana dengan input dalam bentuk string yang terdiri dari 3 bagian:
<ol>
  <li>Operand 1 (angka maksimal 1 juta).</li>
  <li>Operator (+, -, *, /).</li>
  <li>Operand 2 (angka maksimal 1 juta).</li>
</ol>

Antar operand dan operator akan dipisahkan oleh spasi. Output dari aplikasi anda adalah hasil kalkulasi dari input yang diberikan.<br />
Method signature dari fungsi yang dibuat adalah sebagai berikut <br />
```function kalkulator(string input) : integer```
<br /><br />
![Screenshot 2022-05-13 091901](https://user-images.githubusercontent.com/70563202/168198417-e9ae74dd-140e-4d07-bf2e-95a313dab103.png)
<br />
![Screenshot 2022-05-13 092005](https://user-images.githubusercontent.com/70563202/168198547-52d70bdd-4f85-4323-a086-42aadda10ee9.png)
<br />
Gambar di atas, merupakan contoh input dan output kalkulator sederhana. Dan apabila operand melebihi angka 1 juta, akan mengeluarkan output sebagai berikut: <br/><br />
![Screenshot 2022-05-13 092242](https://user-images.githubusercontent.com/70563202/168198805-7c0a5b53-c14f-4275-a30f-a898d55a51ac.png)
<br />
![Screenshot 2022-05-13 092333](https://user-images.githubusercontent.com/70563202/168198875-428c52e0-8c9e-4285-adfb-c5fc153a44e8.png)
<br /><br />
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
