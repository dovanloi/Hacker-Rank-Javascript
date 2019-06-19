# Giải thuật cơ bản
## Mảng
Giải thuật tính tổng 1 mảng:
``` 
    const counta = (str) => str.split('')
    .filter(c => c == 'a')
    .length
```

Giải thuật ghép đôi:
```
function sockMerchant(n, ar) {
    const colors = {};
    let matches = 0;
    for(let i = 0; i < n; i++) {
        if(colors[ar[i]]) {
            matches++;
            colors[ar[i]] = 0;
        } else {
            colors[ar[i]] = 1;
        }
    }
    return matches;
}
```

Giải thuật tìm vực:
```
function countingValleys(n, s) {
    let v = 0, d = 0;
    let neg = false;
    for (let i = 0; i < n; i++){
        if (s[i] === 'U') {
            d++; 
            if (d >= 0 && neg == true) {
                neg = false;
            }
        } else {
            d--;
            if (d < 0 && neg == false) {
                neg = true;
                v++;
            }
        }
    }
    return v;
}
```

Tìm số lần nhảy nhỏ nhất để đi tới đích có chướng ngại vật (nhảy max 2 ô):
```
function jumpingOnClouds(c) {
    let jumps = 0, i = 0;
    while (i < c.length - 1)
    {
        if (i + 2 < c.length & c[i + 2] != 1)
            i += 1
        jumps += 1
        i += 1
    }
    return jumps
}
```
## Chuỗi
Giải thuật đếm số lượng phần tử trong chuỗi:
``` 
    const counta = (str) => str.split('')
    .filter(c => c == 'a')
    .length
```
