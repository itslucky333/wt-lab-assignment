# LAB-6 java script
JavaScript, often abbreviated JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS. As of 2022, 98% of websites use JavaScript on the client side for web page behavior, often incorporating third-party libraries.
### Ascending and Decending code

```<!DOCTYPE html>
<html>
<head>
 <title>Document</title>
</head>
<body>
    
</body>
<script>
    let array1=[],string;
    array1=prompt("Enter 4 number");
    a=array1.split("")
    string=prompt("Enter asc or desc");
    let swap;
    if (string=="asc"){
        for(let i=0;i<=string.length;i++){
            for(let j=j+1;j<=string.length-1;j++){
                if (a[i]>a[j]){
                    swap=a[i];
                    a[i]=a[j];
                    a[j]=swap;
                }
            }
        } 
        console.log(a);    
    }else{
        for(let i=0;i<=string.length;i++){
            for(let j=i+1;j<=string.length-1;j++){
                if (a[i]<a[j]){
                    swap=a[i];
                    a[i]=a[j];
                    a[j]=swap;
                }
            }
        } 
        console.log(a);
    }
</script>
</html> 
```

### Palindrome or  not
```
<!DOCTYPE html>
<html>
<body>

<p>enter the number to check weather it is palindrome or not</p>


<p id="here"></p>

<script>
    let a,b;
    a=prompt("Enter a number");
    palindrome();
    function palindrome(){
        b=a.split("").reverse().join("");
        if (a==b){
          document.getElementById("here").innerHTML="It is a palindrome";
        }else{
            document.getElementById("here").innerHTML="It is not a palindrome";
        }
    }
</script>

</body>
</html>
```
### Reversing the string
```
<!DOCTYPE html>
<html>
<body>

<p>To print the string in reverse order</p>


<p id="here"></p>

<script>
    let a,b;
    a=prompt("Enter a string");
    reverse();
    function reverse(){
        b=a.split("").reverse().join("");
        document.getElementById("here").innerHTML=b;
    }
</script>

</body>
</html>
```
### Reversing the array
```
<!DOCTYPE html>
<head>
<title>reversing the array provided</title>
</head>
<body>
<p> we are reversing the array provided</p>
<p id="input"></p> <br>
<p id="output"></p>

<script>
const arr=["apple","ball","cat","dog"];
document.getElementById("input").innerHTML=arr + " is the order we input the values in array";
document.getElementById("output").innerHTML="the reverse order is " + arr.reverse();
</script>
</body>
</html>
```
### Sum of Prime
```
<!DOCTYPE html>
<html>
    <body>
        <script type="text/javascript">
            let sum=0,a=0;
            for(let i=1;i<=50;i++){
                for(let j=1;j<=i;j++){
                    if (i%j==0){
                        a=a+1;
                    }
                }
                if (a<=2){
                    sum=sum+i;
                }
                a=0;
            }
            console.log("the sum is ",sum);
        
        </script>
    </body>
</html>
```