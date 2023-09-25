# General Collaboration with ChatGPT 3.5

## README
Current README status is purposed to outline the process to create a live site for viewing.

## My personal process of collaborating with ChatGPT creating Generative Art.
Out of bordem I was curious about Generative Art and its flow works.  Before actually visiting any forums, sites, tutorials over the topic, I wanted to visually see some code so I could interpret it before having any other aide.  Who better to help than our good Old ChatGPT 3.5 to offer an example of which I know nothing about.  I did not create an interface with Chat but rather used the typical login @ [chat.openai.com](https://chat.openai.com). So we'll just section off each of the questions and example outputs of these typical changes I asked for.

## Here we Go!
### 1.  
- **zMag33z** - can you show me a example of a generative art project with javascript so i can visually interpret it before actually reading about it and/or watching videos?

- **Chat** - Certainly! Here's a simple example of a generative art project using JavaScript and HTML5 canvas. This code creates a basic generative pattern of colored circles on a canvas:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Generative Art Example</title>
</head>
<body>
    <canvas id="canvas"></canvas>

    <script>
        const canvas = document.getElementById('canvas');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        function randomColor() {
            const r = Math.floor(Math.random() * 

```

***Not sure if I confused it but it got to the middle of selecting a random color function and just stopped.  LOL***

### Try Again.
- **zMaG33z** - you got to the middle of the randomColor function and stopped generating without any closing tags.

- **Chat** - I apologize for the incomplete response. Let's continue the example and provide the missing closing tags. Here's the complete code for a generative art project with JavaScript using HTML5 canvas:<br><br>
***live example:*** fixed.html (*replace with image*)<br><br>
This code sets up an HTML canvas and uses JavaScript to generate a pattern of randomly colored circles on the canvas. You can customize the number of circles and their sizes by adjusting the for loop and the radius value in the drawCircle function. This is a basic example, and generative art can become much more complex and creative as you explore further.

## 
### 2.
- **zMaG33z** - in java i know how to do this but using the generative art example you gave to me how would i move the circles about the x and y coordinates?

- **Chat** - To move the circles about the x and y coordinates in the generative art example using JavaScript and HTML5 canvas, you can introduce animation by continuously updating the positions of the circles in a loop. Here's a modified version of the example that adds animation to move the circles around:<br><br>
***live example:*** movement.html (*replace with image*)<br><br>
In this version, we create an array called circles to store information about each circle, including its x and y coordinates and velocity in both horizontal and vertical directions. The update function is responsible for moving the circles and continuously updating their positions in an animation loop.<br><br>
The circles will now move around the canvas, and when they reach the canvas edges, they will wrap around to the opposite side, creating a seamless animation. This demonstrates how you can add animation and motion to your generative art projects in JavaScript.

***Then I seen this***

```javascript
requestAnimationFrame(update);
```

***It wasn't specifically scoped out.***

- **zMaG33z** - is the requestAnimationFrame function a built in function?

- **Chat** - Yes, the requestAnimationFrame function is a built-in function in JavaScript, specifically designed for handling animations in web applications. It's commonly used to create smooth and efficient animations by synchronizing with the browser's rendering cycle.

*note: of course it further went into detail with an example of its own.

## 
### 3.

- **zMaG33z** - let's take our generative art a step further.  create a class for the random circles and provide movement.  but we're going to have a class of random squares and for each circles movement let's move a square in the opposite direction.

- **Chat** - Certainly, we can create a class for random circles and random squares with opposite movements to make the generative art more interesting. Here's an updated example:<br><br>
***live example:*** classy.html (*replace with image*)<br><br>
In this updated example, we've created two classes, RandomCircle and RandomSquare, which inherit from the RandomShape class. Each class has its own properties and methods for drawing and updating.<br><br>
The shapes array contains instances of both RandomCircle and RandomSquare, and they move in opposite directions. The animate function is responsible for updating and drawing each shape in the animation loop.<br><br>
This creates a generative art piece with random circles and squares that move around the canvas in opposite directions, creating an interesting visual effect. You can further customize and extend this concept to create more complex generative art compositions.

***Chat actually forgot to add the function for color that was being called within the constructor of the square class.  But its all good.  It corrected itself when given the typeError and line number.***

### The End.
This pretty much sums up my conclusion to the basics of generative art.  Now I am off and to watch some videos and read some articles.  I'll be back to create a more complex generative art piece.  I'll be sure to post it here to my Github [zMag33z](https://github.com/zMag33z).  Thanks for reading.

## Resources:
- [ChatGPT 3.5](https://chat.openai.com/)
- [HTML5 Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)


## License:
None.  Fair use.  

zMaG33z 2023