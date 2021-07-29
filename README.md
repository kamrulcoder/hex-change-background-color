# Hex color Change Backgroound vinilla javascript prject 
## This is project is very simple and straightforward. but  I can learn something through this project. <br>  
> That,s what I am learnig  new javascript content  here..........
1. **Math.random();**
1. **Parsefloat()***
1. For Loop 

<br> 

> 
> Project Code here 

### Html Code Here........ 
```
 <div class="background-area">
        <div class="container">
            <div class="background-wrapper">
                <div class="row">
                    <div class="col-lg-8  offset-lg-2">
                        <div class="box  d-flex justify-content-center align-items-center border border-primary  rounded"  style="width: 100%; height: 60vh; margin: 100px 0; background-color: pink;">
                            <button  class="btn btn-danger click-btn ">#ffc0cb </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

```
<br>
###  Javascript Code Here 

```
        let btn = document.querySelector(".click-btn")
        let box = document.querySelector(".box");
        let colors = [0,1,2,3,4,5,6,7,8,9,'a','b','c','d','e','f'];
        btn.addEventListener("click", function(){
            let hex = "#"
            for (let i = 0; i < 6; i++) {
                let colorIndex = Math.floor(Math.random() * colors.length);
                hex+=colors[colorIndex]                
            }
            box.style.background = hex;
            btn.textContent = hex;    
        })
```



