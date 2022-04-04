# Shinobi RWD Guide
Shows how to implement RWD and Fix bug.

## HTML
```
    <div class="row">
        <div class="image-wrapper">
            <img src="./img/shinobi.png" alt="shinobi">
        </div>
        <div class="text-wrapper">
            <h1>
                This is Shinobi CSS trick
            </h1>
            <p>
                How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.How to make good CSS like Shinobi.
            </p>
        </div>
    </div>
 ```
 ```
 @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
*{
  font-family: Poppins;
}
.row{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
}
img{
  max-width: 100%;
  height: auto;
}
.text-wrapper{
  flex: 1 1;
}
.container{
  max-width: 80rem;
}

@media screen and (max-width:1024px) {
    .row{
      flex-direction: column;
      align-items: center;
    }
    h1{
      text-align: center;
    }
}
 ```
 
 As you can see, it is very easy to write CSS code for RWD implementation for developers who have solid knowledge of CSS.
However, some non-Senior developers often forget to add the following and encounter unexpected bugs as a result.

```
    <meta name="viewport" content="width=device-width, initial-scale=1">
```

## BUG
![BUG](https://user-images.githubusercontent.com/92864027/161470189-4fb8982c-fdf3-4050-8296-cde1a2ce7adb.jpg)
## Correct
![result](https://user-images.githubusercontent.com/92864027/161470205-67a0c11f-0dc4-46c9-ba5c-c9099d8d8c52.jpg)

As you can see in over picture, CSS is correct, but RWD is not implemented because it is not scaled to the device width.
You can check it directly:
```
bug.html
correct.html
```
Thank you
Shinobi Developers
