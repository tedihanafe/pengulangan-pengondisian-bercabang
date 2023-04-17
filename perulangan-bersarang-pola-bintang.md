# Membuat Perulangan Bersarang Dengan Javascript
Ini merupkan hasil experimen saya dalam membuat perulangan bersarang dengan membentuk Pola Bintang Berurut.

## 1. Pola bintang 1
```bash
var s = "";

for (var i = 0; i < 5; i++) {
  for (var j = 0; j <= i; j++) {
    s += "*";
  }
  s += "\n";
}
console.log(s);
```
hasil :
```bash
*
**
***
****
*****
```
## 2. Pola Bintang 2
```bash
var s = "";
for (var i = 5; i > 0; i--) {
  for (var j = 0; j < i; j++) {
    s += "*";
  }
  s += "\n";
}
console.log(s)
```
hasil :
```bash
*****
****
***
**
*
```
## 3. Pola Bintang ke 3
```bash
var s = "";
for (i = 5; i > 0; i--) {
  for (j = 0; j <= 5; j++) {
    if (j >= i) {
      s += "* ";
    } else {
      s += " ";
    }
  }
  s += "\n";
}
console.log(s);
```
hasil :
```bash
    *
   **
  ***
 ****
*****
```

## 4. Pola bintang ke 4
```bash
var s ="";
for (var i = 5; i > 0; i--) {
  for (var j = 5; j > 0; j--) {
    if (j <= i) {
      s += "*";
    } else {
      s += " ";
    }
  }
  s += "\n";
}

console.log(s);
```
hasil :
```bash
  *****
   ****
    ***
     **
      *
```

## 5. Pola # Genap/Ganjil
```bash
var s = "";
for (var i = 0; i < 6; i++) {
  if (i % 2 == 0) {
    for (var j = 0; j < 6; j++) {
      if (j % 2 == 0) {
        s += "#";
      } else {
        s += " ";
      }
    }
    s += "\n";
  } else {
    for (var j = 0; j < 6; j++) {
      if (j % 2 == 0) {
        s += " ";
      } else {
        s += "#";
      }
    }
    s += "\n";
  }
}

console.log(s);
```
hasil: 
```bash
# # #
 # # #
# # #
 # # #
# # #
 # # #
 ```