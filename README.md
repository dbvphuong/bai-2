# bai-2  
```
var n=6;
var arr= [];
for(var a=0; a<n; a++){
    arr.push(new Array(a+1).fill(1));
}
for(let i=0; i<n;i++){
    for(let j = 0; j<arr[i].length; j++){
       if(j==0){
           arr[i][j]=1;
           }
       else if(j==arr[i].length-1){
           arr[i][j]=1;
           }
       else if(j!=0 && j!=arr[i].length-1){
           arr[i][j] = arr[i-1][j-1] + arr[i-1][j];
           }
    }
   }

console.log(arr);

```
