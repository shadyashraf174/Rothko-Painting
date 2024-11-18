# **Rothko Painting** 
#### learned it from [freeCodeCamp](https://www.freecodecamp.org/) || See it Live at [CodePen](https://codepen.io/shady-ashraf/pen/PoMvYMd)
###### Every HTML element is its own box – with its own spacing and a border. This is called the Box Model. In this course, you'll use CSS and the Box Model to create your own Rothko-style rectangular art pieces.
---
### **Overview**  
The **Rothko Painting Project** is an artistic recreation inspired by the abstract works of Mark Rothko. This project demonstrates the use of HTML and CSS to build a layered design that mimics the appearance of Rothko’s iconic paintings. It focuses on layout structuring, color blending, and subtle visual effects like blur and shadows.

---

### **Table of Contents**
1. [Project Structure](#project-structure)
2. [HTML Details](#html-details)
3. [CSS Details](#css-details)
4. [How to Use](#how-to-use)
5. [Summary of Selectors Used](#summary-of-selectors-used)

---

### **Project Structure**  
The project consists of two main files:  

- **`index.html`**: Defines the structure and content of the artwork.  
- **`styles.css`**: Contains the styles, colors, and effects applied to the elements.  

**File structure:**  
```
/
├── index.html
├── styles.css
```

---

### **HTML Details**  
The `index.html` file provides the structure for the project.  

#### Key Elements:
1. **Title and Linking**:
   - `<title>`: Sets the page title as *Rothko Painting*.  
   - `<link>`: Connects the external CSS file.

2. **Main Structure**:
   - **`<div class="frame">`**: Creates the outer frame of the painting.  
   - **`<div class="canvas">`**: Represents the canvas background where the layers are displayed.  
   - **`<div class="one">`, `<div class="two">`, `<div class="three">`**: Adds the individual abstract layers.  

**Example:**
```html
<div class="frame">
    <div class="canvas">
        <div class="one"></div>
        <div class="two"></div>
        <div class="three"></div>
    </div>
</div>
```

---

### **CSS Details**  
The `styles.css` file is responsible for the artistic styling of the painting.

#### **General Styles:**
1. **Frame**:
   - The `.frame` element acts as the outer boundary, styled to resemble a traditional picture frame.  
   - Black border with padding centers the canvas.  
   ```css
   .frame {
       border: 50px solid black;
       width: 500px;
       padding: 50px;
       margin: 20px auto;
   }
   ```

2. **Canvas**:
   - The `.canvas` is styled with a dark maroon background color and a subtle blur effect to add depth.  
   ```css
   .canvas {
       width: 500px;
       height: 600px;
       background-color: #4d0f00;
       filter: blur(2px);
   }
   ```

---

#### **Specific Styles:**
1. **Layer One (`.one`)**:
   - A light orange rectangle with soft shadows and slight rotation.  
   ```css
   .one {
       width: 425px;
       height: 150px;
       background-color: #efb762;
       margin: 20px auto;
       box-shadow: 0 0 3px 3px #efb762;
       border-radius: 9px;
       transform: rotate(-0.6deg);
       filter: blur(1px);
   }
   ```

2. **Layer Two (`.two`)**:
   - A deeper red rectangle with rounded edges and a slightly different rotation.  
   ```css
   .two {
       width: 475px;
       height: 200px;
       background-color: #8f0401;
       margin: 0 auto 20px;
       box-shadow: 0 0 3px 3px #8f0401;
       border-radius: 8px 10px;
       transform: rotate(0.4deg);
       filter: blur(1px);
   }
   ```

3. **Layer Three (`.three`)**:
   - A smaller, darker red rectangle with irregularly rounded corners and a more pronounced blur effect.  
   ```css
   .three {
       width: 91%;
       height: 28%;
       background-color: #b20403;
       margin: auto;
       box-shadow: 0 0 5px 5px #b20403;
       border-radius: 30px 25px 60px 12px;
       transform: rotate(-0.2deg);
       filter: blur(2px);
   }
   ```

---

### **How to Use**

1. **Clone the Project**:
   ```bash
   git clone https://github.com/shadyashraf174/Rothko-Painting
   cd Rothko-Painting
   ```

2. **Run the Project**:
   Open the `index.html` file in any browser to view the painting.

3. **Customization**:
   - Modify colors in `styles.css` for a personalized palette.  
   - Adjust `transform` and `border-radius` to experiment with shapes.  
   - Tweak `filter: blur()` for different texture effects.  

---

### **Summary of Selectors Used**

#### **Tag Selectors**
- `div`: Used as containers for different elements of the painting.

#### **Class Selectors**
- `.frame`: Styles the border and layout for the frame.  
- `.canvas`: Adds the blurred background and defines the canvas dimensions.  
- `.one`, `.two`, `.three`: Styles each of the painting’s layers with unique properties like size, color, and rotation.  

#### **Pseudo-Classes**
- `filter: blur()` adds visual depth.  
- `box-shadow` highlights each layer's edges.  
- `transform: rotate()` creates asymmetry.  

--- 

![image](https://github.com/user-attachments/assets/5bea1822-769b-4086-9250-ffb6670e2a53)

---
This project is a simple and creative way to explore CSS effects and layouts, inspired by Rothko’s iconic abstract art style.
