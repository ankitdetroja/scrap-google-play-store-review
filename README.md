# scrap-google-play-store-review

```javascript

//Get a class name of the review container from inspect and run this code in the console on Google Play console.

const objectData = [];
const data = document.getElementsByClassName(""); // get a classname from inspect

for(let i =0; i< data.length; i++){
    console.log(data[i])
    objectData.push({
        name: data[i].children[0].children[0].children[0].children[1].innerText,
        img: data[i].children[0].children[0].children[0].children[0].src,
        review: data[i].children[1].innerText
    })
}
```
