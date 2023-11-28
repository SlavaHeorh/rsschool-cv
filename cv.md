# Kazliakouski Viachaslau

---

---

## **Contact information:**

[e-mail: slava.georg.k@gmail.com](mailto:slava.georg.k@gmail.com "gmail.com") <br>
[GitHub account: SlavaHeorh](https://github.com/SlavaHeorh "GitHub") <br>
[LinkedIn: Viachaslau Kazliakouski](https://www.linkedin.com/in/ViachaslauKazliakouski/ "LinkedIn") <br>

---

## **About Me**

+ Purposefulness, perseverance, friendly.
+ Experience in training new employees.
+ Easy to get along with team.
+ The desire to learn and develop in this direction.
+ I can work as a team or alone.

## **My Skills**

+ HTML
+ JS basic
+ CSS(SCSS)
+ React
+ Next.js

---

## **Work Experience**

*  "Kenfordbel" 2013-2017
    + Mobile device repair and maintenance engineer
*  "Kenfordbel" 2017-2019
    + Lead engineer
*  "Bank Processing Center" 2020-2022
    + Electronics engineer
*  "Taqtile" 2022
    + Junior front-end developer 

---

## **Code Examples**

```js
// slider

let widthCon = 0;
const sliderLine = document.querySelector(".second_content_slider_track")
const pointColorOne = document.querySelector('.second_content_one')
const pointColorTwo = document.querySelector('.second_content_two')
const pointColorThree = document.querySelector('.second_content_three')
pointColorOne.style.backgroundColor = "#665F55"

document.querySelector('.second_content_next').addEventListener("click", function (){
    pointColorOne.style.backgroundColor = "#665F55"

    if ( widthCon === 0 ) {
        pointColorOne.style.backgroundColor = "#C1B6AD"
        pointColorTwo.style.backgroundColor = "#665F55"
        pointColorThree.style.backgroundColor = "#C1B6AD"
    } else if (widthCon === 480) {
        pointColorOne.style.backgroundColor = "#C1B6AD"
        pointColorTwo.style.backgroundColor = "#C1B6AD"
        pointColorThree.style.backgroundColor = "#665F55"
    } else if (widthCon === 960) {
        pointColorOne.style.backgroundColor = "#665F55"
        pointColorTwo.style.backgroundColor = "#C1B6AD"
        pointColorThree.style.backgroundColor = "#C1B6AD"
    }

    widthCon = widthCon + 480;

    if (widthCon > 960) {
        widthCon = 0;
    }
    sliderLine.style.left = -widthCon + "px";

})

document.querySelector('.second_content_prev').addEventListener("click", function (){
    pointColorOne.style.backgroundColor = "#665F55"

    if ( widthCon === 0 ) {
        pointColorOne.style.backgroundColor = "#C1B6AD"
        pointColorTwo.style.backgroundColor = "#C1B6AD"
        pointColorThree.style.backgroundColor = "#665F55"
    } else if (widthCon === 960) {
        pointColorOne.style.backgroundColor = "#C1B6AD"
        pointColorTwo.style.backgroundColor = "#665F55"
        pointColorThree.style.backgroundColor = "#C1B6AD"
    } else if (widthCon === 480) {
        pointColorOne.style.backgroundColor = "#665F55"
        pointColorTwo.style.backgroundColor = "#C1B6AD"
        pointColorThree.style.backgroundColor = "#C1B6AD"
    }

    widthCon = widthCon - 480;

    if (widthCon < 0) {
        widthCon = 960;
    }
    sliderLine.style.left = -widthCon + "px";
})

// slider

```