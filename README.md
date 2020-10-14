# Stone-paper-scissor
A time killing stone paper scissor game right from your Browser console. 
Just open dev tools on your browser, select console, copy paste the code and hit the ENTER with LOVE

The Code: 
```
let score1 = 0;
let score2 = 0;
let st = 1;
let p = 2;
let s = 3;
function play() {
    let sign = +prompt("stone: 1, paper: 2, scissor: 3");
    if(!sign) {
        alert(`Your score: ${score1} \nComputer score: ${score2}`);
        return;
    }
    let k = 1 + Math.floor(Math.random()*2);
    if(sign == k) {}
    else {
        if(sign == st && k == s) score1++;
        else if(sign == st && k == p) score2++;
        
        else if(sign == p && k == st) score1++;
        else if(sign == p && k == s) score2++;

        else if(sign == s && k == st) score2++;
        else if(sign == s && k == p) score1++;
    }
    alert(k);
    play();
}
play();
```
