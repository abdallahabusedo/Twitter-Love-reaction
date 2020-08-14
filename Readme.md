# Twitter Love reaction 

this is a simple code that have the animation of the twitter love animation 

### 😎 How to make it 
first of all make a span that have a class name `heart`
 ```
    <div class="container">
      <span class="heart" id="heart"></span>
    </div>
 ```
 
 in the CSS code we will center the container 
 ```
 .container {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
 ```
 
 then style the heart 
  - give the image the width 
  - background image without repeat 
  - then focus  on one part of the image 
 ```
 .heart {
    float:left;
    width: 90px;
    height: 90px;
    background: url("img.png") no-repeat;
    background-size: 2900%;
    background-position: left;
}
 ```
 
 then i make another class of what will happend when i click on the heart 
 
```
.hearts {
    background-position: right;
    animation: animate 0.8s steps(28) 1;
}

@keyframes animate {
    0% {
        background-position: left;
    }

    100% {
        background-postion: right;
    }
}

```
then i make the script by adding a event listener click then toggle the class name
```
 let love = document.getElementById("heart");
    love.addEventListener("click", function () {
      document.getElementById("heart").classList.toggle("hearts");
    });
```

# ScreenShots
![image](https://user-images.githubusercontent.com/42722816/90199625-92ddbf80-ddd5-11ea-93cd-9dc6c11ef39e.png)
![ezgif com-crop](https://user-images.githubusercontent.com/42722816/90199848-1eefe700-ddd6-11ea-95f8-97ea5c96cd64.gif)

